# NETWORKWALKS-NGOR-B083-WK3-PASSWORD-CRACKING
🔓 PASSWORD CRACKING WITH JTR AND NW TOOLS

Password Cracking Assessment Using John the Ripper and Networkwalks Tools
1. Executive Summary
This report documents a structured security lab exercise focused on password auditing and recovery methodologies. The objective was to evaluate credential robustness by testing weak artifacts against offline and online tools. Specifically, we used John the Ripper (JtR) (along with its graphical frontend, Johnny) and the web-based utilities provided by Networkwalks (Hash Calculator and Password Cracker). The engagement highlighted key vulnerabilities associated with weak keyspaces, poor password creation habits, and the efficacy of dictionary and brute-force cracking routines.

2. Objectives & Scope
Assess Password Complexity: Evaluate how easily weak or predictable passwords (e.g., standard words, short numeric strings) can be compromised.

Compare Methodologies: Contrast command-line/desktop offline utilities (John the Ripper / Johnny) with browser-based online helper utilities (Networkwalks).

Demonstrate Remediation Paths: Provide findings to advocate for robust password policies, appropriate length constraints, and modern hashing/salting implementations.

3. Methodology & Environment
Environment: Kali Linux (Virtual Machine / Local Environment)

Primary Tools:

🔗 John the Ripper (JtR): High-performance offline password recovery and auditing tool supporting multiple hashing algorithms.

Johnny GUI: Graphical interface wrapper for John the Ripper to simplify hash import and visualization.

🗝️ Networkwalks Tools: Suite of browser-based utilities (Hash Calculator and Password Cracker) used for lightweight, client-side/online hash generation and extraction workflows.

4. Implementation Steps & Workflows
  
  ## Project Module 1: Offline Assessment via John the Ripper / Johnny ##
Target Identification: Gathered sample protected files (such as locked PDF files or target hash snippets).

Hash Extraction / Preparation: Extracted the core security representations required by JtR.

Execution (Wordlist & Incremental Modes):

Performed dictionary-based attacks using standard wordlists (e.g., rockyou.txt).

Executed brute-force incremental passes to check shorter character strings.

## Evidences ##

<img width="764" height="267" alt="image" src="https://github.com/user-attachments/assets/16414228-a2d6-4948-8b07-764e199bcc87" />

<img width="764" height="284" alt="image" src="https://github.com/user-attachments/assets/11d1bef7-c91e-4231-a176-08934c1f24ff" />

<img width="436" height="350" alt="image" src="https://github.com/user-attachments/assets/1c35de6f-62ed-4ade-a76b-149139e27026" />

<img width="401" height="124" alt="image" src="https://github.com/user-attachments/assets/39a20e3b-e3c6-46b8-b05c-9239f7142297" />

<img width="348" height="489" alt="image" src="https://github.com/user-attachments/assets/58d70db2-d409-44db-9e85-52a37733c7bb" />

## Project Module 2: Lightweight Assessment via Networkwalks Tools ##
Hash Calculation: Uploaded target files (such as a restricted PDF) into the Networkwalks Hash Calculator to programmatically extract internal structural checksums/hashes.

Browser-Based Cracking: Passed the extracted data into the Networkwalks Password Cracker tool utilizing targeted dictionary collections to recover access without installing local deep-tier cracking utilities.

## STEPS TAKEN ##

1. Open Hash Calculator and upload the Pdf file.

<img width="731" height="326" alt="image" src="https://github.com/user-attachments/assets/ffe64d5f-57e7-4e68-a531-e2d441b99b3f" />

2. Open Password Cracker on Networkwalks Browser page.

<img width="767" height="415" alt="image" src="https://github.com/user-attachments/assets/f4011885-f63a-4725-b887-553a1c850ce7" />

3. Copy the Password Shown

<img width="710" height="403" alt="image" src="https://github.com/user-attachments/assets/dba3899b-4fd4-44af-9cb6-5a6bfb826ad5" />

4. Unlock the PDF file and see the results.

   <img width="325" height="461" alt="image" src="https://github.com/user-attachments/assets/f40f27a5-09a1-428e-a5e0-7a32a29dee24" />

## Recommendations ##

To safeguard enterprise assets against the risks identified in this report, implement the following controls:

1. Enforce Length and Complexity: Mandate a minimum length of 12–16 characters utilizing mixed-case letters, numbers, and symbols.

2. Eliminate Common Words: Block the use of dictionary terms, sequential characters, and predictable personal info via active directory filters.

3. Upgrade Hashing Standards: Transition legacy password storage mechanisms (such as un-salted MD5 or standard SHA-1) to modern, computationally expensive hashing algorithms like Argon2id, bcrypt, or PBKDF2.



