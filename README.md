## Week 16 Homework Submission File: Penetration Testing 1

#### Step 1: Google Dorking


- Using Google, can you identify who the Chief Executive Officer of Altoro Mutual is:
**Ans** :- Use the command **site:demo.testfire.net intext:chief executive officer**
- How can this information be helpful to an attacker:
**Ans :-** This information would serve as OSINT and can be used as by an attacker for impersonating attacks.
Also attackers attempt to gain unauthorized access to executive’s accounts as C-level executives are often privy to sensitive information that is highly valued in the darkweb.
Cybercriminals target executives using well thought out and tailored spear phishing messages to trick the executive into divulging passwords and other sensitive information.

#### Step 2: DNS and Domain Discovery

Enter the IP address for `demo.testfire.net` into Domain Dossier and answer the following questions based on the results:

  1. Where is the company located: 
**Ans :- Sunnyvale, CA**
  2. What is the NetRange IP address:
**Ans : - 65.61.137.64 - 65.61.137.127**
  3. What is the company they use to store their infrastructure:
 **Ans :- Rackspace Backbone Engineering**

  4. What is the IP address of the DNS server:
**Ans :- 65.61.137.117**
#### Step 3: Shodan

- What open ports and running services did Shodan find:
**Ans :- 80, 443, 8080**
**Running Services - TCP, SSL & HTTPS, HTTP**

#### Step 4: Recon-ng

- Install the Recon module `xssed`. 
- Set the source to `demo.testfire.net`. 
- Run the module. 
**Ans:- commands to be used**
1) recon-ng
2) keys add shodan_api [key to be added]
3) marketplace install xssed
4) modules load recon/domains-vulnerabilities/xssed
5) options set SOURCE demo.testfire.net
6) run
Is Altoro Mutual vulnerable to XSS: **Yes, Altoro Mutual is vulnerable to XSS**

### Step 5: Zenmap

Your client has asked that you help identify any vulnerabilities with their file-sharing server. Using the Metasploitable machine to act as your client's server, complete the following:

- Command for Zenmap to run a service scan against the Metasploitable machine: 
 
- Bonus command to output results into a new text file named `zenmapscan.txt`:

- Zenmap vulnerability script command: 

- Once you have identified this vulnerability, answer the following questions for your client:
  1. What is the vulnerability:

  2. Why is it dangerous:

  3. What mitigation strategies can you recommendations for the client to protect their server:

---
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.  