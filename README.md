# Port Scanner
<h2>Description</h2>
This lab demonstrates how to build a Python-based port scanner that checks for open TCP ports on a given target host. Port scanning is one of the most common techniques used in penetration testing to discover active services and potential vulnerabilities. By implementing this tool, students gain practical experience with:

  - Automating scans across multiple ports.
  - Understanding the importance of port scanning in the reconnaissance phases of ethical hacking.

The lab reinforces both programming skills and fundamental cybersecurity knowledge about network enumeration.  

<h2>Enviroments and Utilities</h2>

<b>Enviroment:</b>
  - <b>Operating System:</b> Any OS with Python 3.13 installed (Windows, Linux, or macOS).
  - <b>Execution Setup:</b> Local computer or a virtual machine (for safe testing).
  - <b>Target Systems:</b> A safe, external test server (e.g., scanme.nmap.org, provided by the Nmap project).

<b>Utilities and Tools:</b>
  - <b>Programming Language:</b> Python 3.13.
  - <b>Libraries/Modules:</b> NMAP.
  - <b>Text Editor/IDE:</b> VS Code.
  - <b>Command-Line Terminal:</b> To run script and observe results.

<h2>Project Setup</h2>

1. <b>Create the Python Script</b>
  - Open your text editor and create a file named Python-Nmap.py.
  - Right-click and open the integrated terminal, then start a bash terminal.

2. <b>Import Nmap</b>
  - Import the Python libraries for networking, threading, and input handling.

<img src="https://i.imgur.com/ZJVGx9d.png" height="80%" width="80%" alt="AzureSiemLab"/>

3. <b>Create an instance of the nmap.portscanner class</b>
  - Assign it to the variable “nm”.

<img src="https://i.imgur.com/gLigtUk.png" height="80%" width="80%" alt="PortScanner"/>

4. <b>Create two variables. One labeled “target" and the other labeled “options”</b>
  - “options” indicates the switches used. The “-sV” switch is used to return version info about the services found on that port. The “-sC” switch is used to run a standard nmap script.
  - “target” is the IP address of the target host.

<img src="https://i.imgur.com/F57SXGn.png" height="80%" width="80%" alt="PortScanner"/>

5. <b>Call the scan method on the created instance of the nmap.portscanner class.</b>
  - The scan method is being used to perform a network scan using nmap.
  - The scan method takes two arguments: the first is “target”, so it knows where to scan, and then arguments, which I made equal to “options”, so it knows what to return.

<img src="https://i.imgur.com/t0hKu6W.png" height="80%" width="80%" alt="PortScanner"/>

6. <b>Create a nested loop structure with 3 loops</b>
  - To iterate through the results of the namp scan.
  - To print info about each host protocol and port discovered.

<img src="https://i.imgur.com/oBZxj50.png" height="80%" width="80%" alt="PortScanner"/>

7. <b>Run the Python script</b>
  - Run python Python-Nmap.py.
  - Go through the returned info and start active reconnaissance on open ports.

<img src="https://i.imgur.com/yROeEwo.png" height="80%" width="80%" alt="PortScanner"/>
