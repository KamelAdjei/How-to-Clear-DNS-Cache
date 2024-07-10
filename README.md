# View-and-Clear-DNS-Cache

## Objectives:
1. View and clear DNS Cache using Command Prompt.
2. View and clear DNS cache using Windows PowerShell.

### What is DNS Cache?
A DNS cache is a record of all the queries made to a DNS server by your browser. When you enter a URL in your browser, it sends a request to the DNS server to obtain the IP address associated with the URL. Once your browser receives the IP address, it then proceeds to load the corresponding website in your window. The next time you try to access the same website, the cache utilizes the stored data to quickly load the site, resulting in reduced server response times and improved loading speed. If you encounter Internet connectivity problems, a common solution is to flush or clear the DNS cache.

## Objective 1: Command Prompt
•	Click on start menu → type in **cmd** → _right click_ on Command Prompt → **Run as administrator**
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/1eebcc29-e464-4b25-b51a-03542cb53d2e" alt="commandprompt" />
  <p align="center">
    <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/0de73ffd-5a09-4816-8ada-87509be724e2" alt="commandprompt" />
  </p>
</p>

•	Type in the command _ipconfig /displaydns_ and hit **Enter**

•	The results displayed include _Record name, Record Type, Time to Live, Data length, Section, CNAME record_ and so on
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/c8f82aea-31a7-4055-84a7-967d6996aae6" alt="commandprompt" />
</p>

•	To clear the DNS cache, type the following command in the prompt and hit Enter _ipconfig/flushdns_
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/03809f8e-d667-407b-9f07-b3ac57c5297a" alt="commandprompt" />
</p>
•	You should see a message that the cache has been _successfully flushed_

•	Now **Run** the **command** _ipconfig /displaydns_ to **verify** the cache has been cleared. [Optional]
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/ef970883-874a-4b23-9033-05b1122b015f" alt="commandprompt" />
</p>


## Objective 2: PowerShell

•	Navigate to the Start menu, type **PowerShell**, right click on windows PowerShell app and **Run as administrator**
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/86dc405c-4f03-4415-8cbf-8c44f2c61925" alt="powershell"/>
</p>

•	Type in the command **Get-DnsClientCache** and hit **Enter**
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/12ea6107-dc4a-4f6e-9a77-76732ef80225" alt="powershell"/>
</p>

•	The Output shows various parameters like **RecordName, Record Type, Status, Data length, Data** and so on
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/af5f42bc-38a1-4568-8389-0935ac16fda0" alt="powershell"/>
</p>

•	To clear the DNS cache type in the command **Clear-DnsClientCache** and press **Enter**

•	To see a description of what this command does, use the parameter _verbose._
<p align="center">
  <img src="https://github.com/KamelAdjei/How-to-Clear-DNS-Cache/assets/34016698/cdf905d6-dacb-4851-b403-e3872d2028dd" alt="powershell"/>
</p>

•	The DNS Cache has successfully been cleared!
