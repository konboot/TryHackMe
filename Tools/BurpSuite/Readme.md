<h1 align="center">
<image src="https://github.com/konboot/TryHackMe/assets/53315283/5f1c611e-b87f-44e4-ab61-e86d1ebd566d" height=300>
<br>Burp Suite: The Basics
</h1>
<p align="center"> Burp Suite is a Java-based framework designed to serve as a comprehensive solution for conducting web application penetration testing. 
It has become the industry standard tool for hands-on security assessments of web and mobile applications, including those that rely on application programming interfaces (APIs).
Simply put, Burp Suite captures and enables manipulation of all the HTTP/HTTPS traffic between a browser and a web server. </p>
<div align="center">
  
![Screenshot_2024-03-09_185546-removebg-preview](https://github.com/konboot/TryHackMe/assets/53315283/4b9c792a-822a-4bfc-9758-5ae3b0607186)
</div>


<h2 align="center">Key features:</h3>
<p>
<b>1. Proxy:</b> The Burp Proxy is the most renowned aspect of Burp Suite. It enables interception and modification of requests and responses while interacting with web applications.
<br><br><b>2. Repeater:</b> Another well-known feature. Repeater allows for capturing, modifying, and resending the same request multiple times. This functionality is particularly useful when crafting payloads through trial and error (e.g., in SQLi - Structured Query Language Injection) or testing the functionality of an endpoint for vulnerabilities.
<br><br><b>3. Intruder:</b> Despite rate limitations in Burp Suite Community, Intruder allows for spraying endpoints with requests. It is commonly utilized for brute-force attacks or fuzzing endpoints.
<br><br><b>4. Decoder:</b> Decoder offers a valuable service for data transformation. It can decode captured information or encode payloads before sending them to the target. While alternative services exist for this purpose, leveraging Decoder within Burp Suite can be highly efficient.
<br><br><b>5. Comparer:</b> As the name suggests, Comparer enables the comparison of two pieces of data at either the word or byte level. While not exclusive to Burp Suite, the ability to send potentially large data segments directly to a comparison tool with a single keyboard shortcut significantly accelerates the process.
<br><br><b>6. Sequencer:</b> Sequencer is typically employed when assessing the randomness of tokens, such as session cookie values or other supposedly randomly generated data. If the algorithm used for generating these values lacks secure randomness, it can expose avenues for devastating attacks.</p>

<h2 align="center">BurpSuite Dashboard</h2>
<br>

![image](https://github.com/konboot/TryHackMe/assets/53315283/d6adf6f8-fd04-40a8-bfe1-9f60a737f689)
<br><br>
<b>1. Tasks:</b> The Tasks menu allows you to define background tasks that Burp Suite will perform while you use the application. In Burp Suite Community, the default “Live Passive Crawl” task, which automatically logs the pages visited, is sufficient for our purposes in this module. Burp Suite Professional offers additional features like on-demand scans.
<br><br>
<b>2. Event log:</b> The Event log provides information about the actions performed by Burp Suite, such as starting the proxy, as well as details about connections made through Burp.
<br><br>
<b>3. Issue Activity:</b> This section is specific to Burp Suite Professional. It displays the vulnerabilities identified by the automated scanner, ranked by severity and filterable based on the certainty of the vulnerability.
<br><br>
<b>4. Advisory:</b> The Advisory section provides more detailed information about the identified vulnerabilities, including references and suggested remediations. This information can be exported into a report. In Burp Suite Community, this section may not show any vulnerabilities.

<h2 align="center">Keyboard shortcuts</h2>
<br>
<div align="center">

| Shortcut        | Tab          |
|-----------------|--------------|
| Ctrl + Shift + D | Dashboard    |
| Ctrl + Shift + T | Target       |
| Ctrl + Shift + P | Proxy        |
| Ctrl + Shift + I | Intruder     |
| Ctrl + Shift + R | Repeater     |

</div>


