# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/6e744529-5c6d-41be-a4dc-b11cc4d9ad55" />


### Questions

1.  How many users exist on the system?
2.  There are 29 user accounts shown in the /etc/passwd file in the screenshot.
3.  Which accounts appear to be system accounts?
4.  System accounts are accounts created for operating system services and background processes.
5.  Why do operating systems create system accounts?
6.  Operating systems create system accounts to run services and background processes securely.

### Reflection

Explain why understanding system users is important for cybersecurity.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/c4d7d72f-39c8-4b51-9c46-77d9cea50114" />


### Questions

1.  Which processes are running as `root`?
2.  Many processes are running as root, including ;
3.  /sbin/init splash
4.  [kthread]
5.  
6.  Why can processes running as root be dangerous?
7.  Process running as root have very high privileges and can access  or modify almost any file or system resource. If a process has a security vulnerability,attackers may exploit it to gain full control of the system. 
8.  What could happen if a malicious program ran with root privileges?
Amaicious program running as root could:
Delete or modify important system file.
steal personal data and password
### Reflection

What did you learn about system processes and security?
I learned that linux runs many background processes to manage the operating system.
------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/da3c8555-a0da-4f72-9c66-619436f1dbd1" />


### Questions

1.  Which ports are open?
2.  Which services appear to be listening?
3.  Why might open ports represent a security risk?

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
