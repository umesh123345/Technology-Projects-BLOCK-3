# Exploring the CIA Triad

## Objective

Understand the **Confidentiality, Integrity and Availability (CIA)** principles using practical tasks on a Raspberry Pi.

---

# Part 1 – Confidentiality

1. Create a confidential file.

    ```bash
    nano secrets.txt
    ```

1. Write some confidential information.

1. Save the file.

1. Now restrict access:
    ```bash
    chmod 600 secrets.txt
    ```
1. Check permissions:
    ```bash
    ls -l secrets.txt
    ```

**Questions**
- Who can read this file?
- only the owner of the file can read it because the permission is set to 600.Group members and other users cannot read the file.
- How does file permission protect confidentiality?
- File permissions protect confidentiality by restricting access to sensitive information . Using chmod 600 allows only the owner to read and write the file. Other users cannot acess its contents helping prevent unauthorised acess.

## Part 2 – Integrity

1. Create a hash of the file.
    ```bash
    sha256sum secrets.txt
    ```
    _What does "hash" do?

1. Save the output.

1. Modify the file.
    ```bash
    nano secrets.txt
    ```

1. Run the hash again.


** Questions**
- Did the hash change?
- Yes the hash change because contain of the file were modified.
- 
- Why do security systems use hashing?
security system use hashing to check data integrity detect unauthorised changes and verify the information has not been modified.

# Part 3 – Availability

1. Check system uptime:
    ```bash
    uptime
    ```

1. List running processes:
    ```bash
    top
    ```

**Questions**
- Why is system uptime important?
- System uptime is important because it ensures that computers, servers and services remain available and accessible to users.
- What happens if a system is unavailable?
- If a system is unavailable users cannot acess its services or information. This can interrupt daily activities, reduce productivity, cause financial losses and affect customer satisfaction.
-  

## Deliverables
Include:
- Screenshot of file permissions
- Screenshot of hash results
- Answers to questions
- Reflection
    >Explain how this activity demonstrated the CIA triad.
