# 🔐 Week 3: PDF Password Cracking

**Networkwalks Cybersecurity Internship — Batch B084**

This repository documents my Week 3 practical exercise: recovering access to the supplied password-protected PDF, **My Locked PDF1.pdf**, using John the Ripper (JTR), Johnny, and the Networkwalks Hash Calculator and Password Cracker tools.

## Objectives

1. Extract a crackable hash from the supplied PDF.
2. Use John the Ripper and its Johnny graphical interface on Windows to perform a password-auditing attempt.
3. Use the Networkwalks Hash Calculator and Password Cracker workflow.
4. Open the protected PDF with the recovered password and verify access.

## Tools Used

| Tool | Purpose |
|---|---|
| John the Ripper (Jumbo) | Command-line password auditing and recovery |
| Johnny | Graphical interface for John the Ripper |
| Networkwalks Hash Calculator | Extract a crackable hash from an encrypted PDF |
| Networkwalks Password Cracker | Perform the browser-based password recovery exercise |
| Windows PC | Run the local JTR / Johnny workflow |
| Web browser | Access the Networkwalks tools and verify the PDF |

## Workflow 1: John the Ripper and Johnny (Windows)

### 1. John the Ripper

Reviewed the John the Ripper website and the available Windows Jumbo build used for the exercise.

![John the Ripper website](images/01-John-the-Ripper-Website.jpg)

### 2. Johnny configuration

Configured Johnny to use the local John the Ripper Jumbo executable. The screenshot shows the executable path and detected version.

![Johnny configuration](images/02-Johnny-Configuration.jpg)

### 3. Johnny result

The Johnny screenshot shows a recovered-password entry associated with the PDF hash. The value shown in the Password column is **good-luck**.

![Johnny recovered entry](images/04-Johnny-Recovered-Entry.jpg)

## Workflow 2: Networkwalks Hash Calculator and Password Cracker

### 1. Extract the PDF hash

Used the Networkwalks Hash Calculator to process **My Locked PDF1.pdf** and display an encrypted-PDF hash in a format compatible with PDF password-auditing tools.

![Networkwalks Hash Calculator](images/06-Networkwalks-Hash-Calculator.jpg)

A further hash-extraction screenshot from a separate PDF hash-extraction webpage is included as supplementary evidence. It is not the Networkwalks Hash Calculator interface.

![Supplementary PDF hash extraction](images/03-PDF-Hash-Extraction-Supplementary.jpg)

### 2. Password Cracker result

Submitted the extracted hash to the Networkwalks Password Cracker. The captured result screen reports a successful match and displays **password1**.

![Networkwalks Password Cracker result](images/07-Networkwalks-Password-Cracker-Result.jpg)

**Evidence note:** The Johnny result screenshot displays `good-luck`, while the Networkwalks Password Cracker screenshot displays `password1`. These are recorded as the separate outputs visible in the supplied screenshots; the screenshots alone do not establish that both tools returned the same password for the same attempt.

### 3. Verify access to the PDF

Opened the PDF successfully after password recovery. The following screenshots show the unlocked PDF / congratulatory page, including the page confirming that the first lab flag was captured.

![Unlocked PDF confirmation](images/05-Unlocked-PDF-Confirmation.jpg)

![PDF flag page](images/08-PDF-Flag-Page.jpg)

The flag text and full hash are left out of this README so the repository overview does not unnecessarily publish challenge-specific answer material. The evidence screenshot is retained as supplied.

## Results Summary

- The PDF hash was extracted using the Networkwalks Hash Calculator.
- A password-cracking success message was displayed by the Networkwalks Password Cracker.
- Johnny displayed a recovered-password entry in the local Windows JTR GUI.
- The protected PDF opened successfully after password recovery.

## Learning Outcomes

- Understood how a password-protected PDF can be represented using a crackable hash format.
- Practiced extracting a PDF hash for password auditing.
- Explored John the Ripper Jumbo and its Johnny graphical interface on Windows.
- Used the Networkwalks Hash Calculator and Password Cracker workflow.
- Verified the result by opening the protected PDF.

## Disclaimer

This exercise was performed for an authorized educational lab using the PDF supplied for the Networkwalks assignment. Password auditing should only be performed on files that you own or have explicit permission to test. Do not use these techniques to access other people's protected documents.

## Author

**Alan Nadh U**  
Networkwalks Cybersecurity Internship — Batch B084  
Week 3 Practical Submission — November 2026
