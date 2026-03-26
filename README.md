# Cybersecurity-Lab-1
# LAB 1: Virtual Lab Environment & Initial Network Reconnaissance
## Project goal: To establish a controlled, virtualised environment using Kali Linux and VirtualBox for penetration testing and vulnerability assessment. The objective was to deploy a service (a simple web server) and perform service and version discovery using Nmap.
### Tools Used:
Kali Linux is the primary operating system for network security tools.
Oracle VM VirtualBox: As the hypervisor to run the virtual environment.
Nmap (Network Mapper): For service and version discovery.
Python (http.server): To rapidly deploy a temporary web server for testing.
Firefox: For validating service availability.

## Service Deployment & Initial Nmap Scan. 

[Nmap scan result for Lab 1](https://github.com/user-attachments/assets/1c079a6d-a2e1-4b01-aaef-6c3e84a682e2)
This image displays two active terminal windows. In the background (left), a temporary web server is running using Python (python3 -m http.server 8080). In the foreground (right), an Nmap scan (sudo nmap -sV -p 8080 localhost) has successfully identified the port as open and accurately determined the service version (Python http.server 3.11.x). This demonstrates a successful configuration of the target environment and the use of basic network-scanning techniques.

[Validation of Service Availability scan](https://github.com/user-attachments/assets/386364d1-cc98-4a3f-af3f-8e13fd9b1af5)
Validation of Service Availability. This screenshot confirms that the deployed web server is reachable and functioning correctly. Firefox is browsing http://localhost:8080, displaying the local directory listing. This front-end interaction triggers HTTP GET requests, which are clearly visible in the terminal logs (showing '200' OK status codes). This step is essential for confirming that the discovered service is fully operational.

## Conclusion & Key Learnings: 
This lab successfully established a baseline for ethical hacking and vulnerability assessment. Key learnings include:
Navigating the Kali Linux environment.
Configuring and managing virtual machines via VirtualBox.
Understanding the relationship between a server (Python) and a client (Firefox).
Utilising Nmap to perform essential service and version discovery (-sV) is a critical first step in identifying potential vulnerabilities in a system.


