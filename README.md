# nessus_scanner
Scanning Vulnerabilities with Nesssus

Set up windows vm:

Download oracle virtual box

https://www.virtualbox.org/wiki/Downloads

Download microsoft windows iso file

https://www.microsoft.com/en-us/software-download/windows10ISO

start up windows VM in Virtual Box

Windows VM settings:

4096 ram

50gb ssd

4 cpu

network settings: adapter 1, Bridged network

Take down firewalls in windows vm
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/92334a9d-7ec2-46cd-891d-0617d77eed5c)

Check if you can ping VM through host machine
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/4184451e-3dc4-4f57-b5cb-41b8247d786d)

Download nessus

https://www.tenable.com/products/nessus/nessus-essentials

Create nessus account

check email for nessus registration key

create new scan in nessus 
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/a7f95d0a-7420-40e8-8d32-ee4bf5a0fe4a)

basic network scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/28a59913-b8ca-4fd1-b229-d49d7e6a57e2)

run the scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/50aab9c3-c9a8-4e1a-addf-22aedfd8f414)
pre scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/756b6c7a-a831-4554-9f5a-a29932088ad7)
pro scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/37298e6a-8ffc-4934-a768-8d2772fb1648)
pro scan, vulnerabilties tab under windows single host scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/f22e13a8-b402-41f2-9726-a572baa61087)



In Windows VM: 
Remote Registry>Stat Up Type: Automatic
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/643ec37e-9e1d-4b5d-be4f-bf6d7f231f68)

Advance Sharing Settings>Turn on file and printer sharing 
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/dc4e0969-7287-488d-81be-5c861c2fd477)

User Account Control>Never Notify
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/c057180f-e54c-429e-8fd7-b30cff15cf38)

Registry Edit>Computer>HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System
Create new DWORD file named LocalAccountTokenFilterPolicy and modify binary value to 1
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/78ac9427-cf6f-4935-b750-441f52e21607)

Configure creditentials 
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/370eb025-bbf7-44ff-8c14-c4a1d2b72ba8)
Restart scan
![image](https://github.com/ccafer/nessus_scanner/assets/61919465/3e988754-85e6-4e27-9691-15f818208f4f)







