## Aim

To use a Mail Header Analyzer (MHA) to trace an email’s origin and verify its authenticity by examining its header for signs of spoofing.

## Tools Used

•	Mail Header Analyzer (online tool or built-in)

•	Web browser

•	Sample email with full header

## Procedure
1.	Open the email and access its full header information (available in most email clients under “Show Original” or “View Source”).
2.	Copy the entire email header text.
3.	Open a Mail Header Analyzer tool (e.g., MxToolbox MHA or Google Apps Toolbox).
4.	Paste the copied email header into the analyzer’s input field.
5.	Run the analysis to extract details such as the sender’s IP address, mail servers used, and authentication results.
6.	Check for SPF, DKIM, and DMARC authentication results to detect possible spoofing.
7.	Compare the originating IP address with the claimed sender domain to verify legitimacy.

## Screenshots

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/8f40ce5c-254a-4e7f-8e7a-9a5ff6355240" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/38c407e5-5e47-4cad-8cbd-dee2259aefe6" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/7d6bf2d6-fa19-439b-a008-053fa1306b57" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/0fe62d01-2ee5-4006-b781-d5a6e3956514" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/8b01039f-3d93-429e-b368-54501d6e49a2" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/e7caabbb-9bec-4ecd-a710-04f9721955c6" />
</p>

---

## Result

The Mail Header Analyzer successfully traced the email’s origin and provided authentication details, helping to identify whether the email was genuine or spoofed.
