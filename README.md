# View-and-Clear-DNS-Cache

## Objectives:
1. View and clear DNS Cache using Command Prompt.
2. View and clear DNS cache using Windows PowerShell.

### What is DNS Cache?
A DNS cache is a record of all the queries made to a DNS server by your browser. When you enter a URL in your browser, it sends a request to the DNS server to obtain the IP address associated with the URL. Once your browser receives the IP address, it then proceeds to load the corresponding website in your window. The next time you try to access the same website, the cache utilizes the stored data to quickly load the site, resulting in reduced server response times and improved loading speed. If you encounter Internet connectivity problems, a common solution is to flush or clear the DNS cache.

## Objective 1: Command Prompt
•	Click on start menu → type in cmd → right click on Command Prompt → Run as administrator
![command prompt 1 1](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/0de73ffd-5a09-4816-8ada-87509be724e2)
![command prompt 1](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/1eebcc29-e464-4b25-b51a-03542cb53d2e)

•	Type in the command ipconfig /displaydns and hit enter

![command prompt](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/c8f82aea-31a7-4055-84a7-967d6996aae6)

•	The results displayed include Record name, Record Type, Time to Live, Data length, Section, CNAME record and so on

![command prompt2](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/03809f8e-d667-407b-9f07-b3ac57c5297a)

•	To clear the DNS cache, type the following command in the prompt and hit Enter ipconfig/flushdns

![command prompt3](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/ef970883-874a-4b23-9033-05b1122b015f)
•	You should see a message that the cache has been successfully flushed.













## Objective 2: PowerShell

•	Click on the start menu, type PowerShell, right click on windows PowerShell app and run as administrator
•	Type in the command Get-DnsClientCache and hit enter
•	The output shows various parameters like RecordName, Record Type, Status, Data length, Data and so on
•	To clear the DNS cache type in the command Clear-DnsClientCache and press enter
•	To see a description of what this command does, use the parameter verbose. Type in Clear-DnsClientCache -verbose and press enter


![powershell 5](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/93a74f58-2ca9-49a8-b773-ea96b103661c)

![powershell4](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/cdf905d6-dacb-4851-b403-e3872d2028dd)
![powershell3](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/af5f42bc-38a1-4568-8389-0935ac16fda0)
![powershell2](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/86dc405c-4f03-4415-8cbf-8c44f2c61925)
![powershell](https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/12ea6107-dc4a-4f6e-9a77-76732ef80225)



