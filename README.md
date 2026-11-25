# Week3-Password-cracking
# Week 3 – Project Module 1: Password Cracking with John the Ripper (JTR)

## Project Overview
This project involved performing password recovery on encrypted PDF files using John the Ripper (JTR), Johnny GUI, and the Networkwalks Password Cracker.

The exercise demonstrated how password-cracking tools use wordlists to identify weak passwords and why strong, unique passwords are important for protecting sensitive documents.

## Tools Used
- John the Ripper 1.9.0-jumbo-1 (Windows x64)
- Johnny GUI 2.2 (Windows x64)
- Online PDF Hash Extractor (OnlineHashCrack)
- Networkwalks Password Cracker (Web-based tool)

## Task 1: Password Cracking Using John the Ripper and Johnny GUI

### Steps Performed
1. Downloaded and extracted John the Ripper (Jumbo) and Johnny GUI.
2. Installed Johnny GUI and configured it to locate `john.exe` inside the extracted `run` folder.
3. Extracted the encrypted PDF password hash using OnlineHashCrack's PDF Hash Extractor.
4. Saved the extracted hash in PASSWD format as `hash1.txt`.
5. Loaded the hash into Johnny using the **Open Password File (PASSWD Format)** option.
6. Selected **Start New Attack** to begin the password-cracking process.
7. Successfully recovered the password and used it to unlock the encrypted PDF.

### Results
- **Recovered Password:** `good-luck`
- **Flag Captured:** `nw{cybersecurity_flag_captured_2608}`
- **Status:** Successfully completed.

## Task 2: Password Cracking Using Networkwalks Password Cracker

### Steps Performed
1. Submitted the extracted PDF hash (`$pdf$...`) to the Networkwalks Password Cracker web tool.
2. The tool performed a wordlist attack by testing possible password combinations.
3. A matching password was identified after 91 out of 100 attempts.
4. Used the recovered password to unlock the related PDF file.
5. Successfully retrieved the required flags.

### Results
- **Recovered Password:** `password1`
- **Flags Captured:**
  - `nw{networkwalks_flag1_jtr_270521_1}`
  - `nw{networkwalks_persistence_jtr_270521}`
- **Status:** Successfully completed.

## Key Takeaways

Through this exercise, I learned that:

- Password-cracking success depends significantly on password complexity and the quality of the wordlist and attack rules used.
- John the Ripper, together with Johnny GUI, provides a practical way to perform password auditing without relying entirely on command-line operations.
- Different password-cracking tools may produce different results depending on their wordlists and configurations.
- Weak and commonly used passwords are more vulnerable to dictionary-based attacks.
- Strong, unique passwords help protect sensitive files and documents from unauthorized access.

## Evidence and Screenshots

The following screenshots will be included as evidence of the completed tasks:

1. Johnny GUI displaying the successfully recovered password `good-luck`.
2. Networkwalks Password Cracker displaying the recovered password `password1`.
3. The first successfully unlocked PDF displaying its captured flag.
4. The second successfully unlocked PDF displaying its captured flags.

## Conclusion

This project provided practical experience in PDF password recovery and password auditing using John the Ripper, Johnny GUI, and the Networkwalks Password Cracker.

It also reinforced the importance of creating strong, complex, and unique passwords to improve document security and reduce the risk of unauthorized access.
