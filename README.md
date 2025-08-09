# PENETRATION-TESTING-TOOLKIT

*Company*: CODTECH IT SOLUTIONS

*NAME*: Sree venkat Ramanujula

*INTERN ID*:CT06DH1414

*DOMAIN*: CYBER SECURITY & ETHICAL HACKING

*DURACTION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH

---

### Description of the Penetration Testing Toolkit Script

This Python script is a basic penetration testing toolkit that includes two essential modules: a **Port Scanner** and an **SSH Brute Forcer**. These modules help users identify open network ports and test SSH credentials, which are common tasks in network security assessments.

---

### Key Modules and Functionality

#### Port Scanner

The port scanner checks specified ports on a target host to determine which are open. It uses Python’s `socket` library to attempt TCP connections to each port:

* If a connection is successful, the port is marked as **open**.
* If the connection fails or times out, it is marked **closed**.

Scanning ports helps discover running services that could be potential entry points for attackers. This module is useful for network reconnaissance during penetration tests.

#### SSH Brute Forcer

The SSH brute forcer tries to access an SSH server by attempting passwords from a user-provided wordlist. Using the `paramiko` library, it connects to the SSH server repeatedly with different passwords until:

* It finds the correct password and reports success.
* It exhausts the wordlist without success.

This tool demonstrates the risk of weak passwords on SSH servers and underscores the need for strong authentication mechanisms.

---

### How the Toolkit Works

When the script runs, it shows a simple menu allowing users to pick a tool:

* For the port scanner, users enter the target hostname/IP and a list of ports to scan.
* For the brute forcer, users input the SSH target, username, and a password file path.

After each operation, the menu reappears, allowing multiple tests during a single run. The modular design makes it easy to add more tools in the future.

---

### Usage and Ethical Guidelines

This toolkit is suited for beginners learning penetration testing techniques or for educational purposes. It is ideal for testing in controlled environments, such as local machines or virtual labs like Metasploitable or OWASP Juice Shop.

**Important:** Always obtain permission before scanning or brute forcing any network or system. Unauthorized testing is illegal and unethical.

---

### Limitations and Possible Enhancements

The current toolkit is a simple implementation:

* Port scanning is sequential and may be slow for many ports.
* The brute forcer handles only SSH and basic password guessing without throttling.
* No logging or detailed reporting features are included.
* It lacks support for other services or attack methods.

Future improvements could add multithreading for faster scans, support for more protocols (FTP, HTTP), enhanced brute forcing options, and better user input validation and error handling.

---

### Summary

This Python penetration testing toolkit provides foundational tools for network reconnaissance and credential testing. Its easy-to-use interface and modular structure make it a great learning tool. By practicing in legal and safe environments, users can better understand vulnerabilities related to open ports and weak SSH passwords. With additional features, this toolkit can evolve into a more comprehensive security testing utility.

---

#output

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4ce06d57-c1ac-4578-ba8b-1d91b66102bd" />
