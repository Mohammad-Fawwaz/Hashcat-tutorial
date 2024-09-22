# Hashcat-tutorial
## Objective
The objective of this project is to provide a comprehensive tutorial on using Hashcat, a powerful password-cracking tool, for performing various types of hash-based attacks. This project aims to demonstrate how to efficiently crack password hashes using techniques like brute-force, dictionary, and mask attacks, while also exploring the ethical implications, legal boundaries, and best practices for protecting sensitive data through strong password hashing algorithms and salting methods.

### Skills Learned
- Understanding of Hashing Algorithms:In-depth knowledge of different hashing algorithms like MD5, SHA-1, SHA-256, bcrypt, and their vulnerabilities.Understanding how hashes are used in securing passwords.
- Password Cracking Techniques:Proficiency in cracking hashes using various methods such as brute-force, dictionary, hybrid, and mask attacks.Ability to optimize attacks based on hash type and system specifications.
- Efficient Use of Hashcat:Hands-on experience using Hashcat for different types of hash-based attacks.Understanding Hashcat modes, rule-based attacks, and advanced features for complex password cracking.
- Password List Creation and Customization:Knowledge of creating or using custom wordlists, such as rockyou.txt, and refining them for specific attacks.Understanding how to manipulate and enhance wordlists for efficient password cracking.
- Penetration Testing and Ethical Hacking:Practical skills in testing password security within a controlled and ethical environment.Understanding the ethical and legal considerations of password cracking, ensuring compliance with penetration testing standards.
- Security Best Practices:Awareness of strong password policies, hashing best practices, and salting techniques to mitigate the risk of password cracking.Understanding the importance of using modern, secure hashing algorithms.

### Tools Used
- Hashcat is an advanced password recovery tool that utilizes brute-force, dictionary, and hybrid attacks to efficiently crack password hashes using CPU and GPU acceleration.
- Kali Linux is a Debian-based operating system designed specifically for penetration testing, digital forensics, and security research, offering a wide range of pre-installed security tools.

## Steps
- open kali linux
- then open terminal
- create a wordlist type nano wordist.txt
- ![Screenshot 2024-09-22 213625](https://github.com/user-attachments/assets/fc246e5e-c3d3-44c6-a23b-91c666ba399a)
- Taking hacking from the wordlist and generating hashvalue of that word
- ![Screenshot 2024-09-22 213805](https://github.com/user-attachments/assets/befafb27-06c4-4c70-9504-4da639050017)
- We are taking MD5 hash value
- We can identify the hash type by running hash-identifier and giving the hash value
- ![Screenshot 2024-09-22 213930](https://github.com/user-attachments/assets/8fc3d3da-88f2-466a-a65d-4d33d314d0eb)
- Hash identifier helps us to identify the hash type
- create MD5.txt file and add the hash value
- ![Screenshot 2024-09-22 214210](https://github.com/user-attachments/assets/8011467c-0fc9-48f8-b606-eedbd02c993a)
- Now there are many modes in Hashcat so use Hashcat --help | grep MD5
- here we are searching for modes with only MD5 as we have identified that the tye of hash is MD5
- ![Screenshot 2024-09-22 214312](https://github.com/user-attachments/assets/08818f25-e3b1-483a-bcea-35979bee1b4c)
- using mode 0
- Use the following command and press enter
- hashcat -m 0 MD5.txt wordlist.txt
-  ![Screenshot 2024-09-22 214517](https://github.com/user-attachments/assets/ab65774f-4b8b-47a0-80a7-ab63d61acb15)
-  Boom the hash is cracked!!!!













