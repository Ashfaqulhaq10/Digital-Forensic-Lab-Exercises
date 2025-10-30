## Aim

To use a Mail Header Analyzer (MHA) to trace an email’s origin and verify its authenticity by examining its header for signs of spoofing.

## Tools Used

•	Mail Header Analyzer (online tool or built-in)

•	Web browser

•	Sample email with full header

## Procedure

1. Open the email that needs to be examined.  
   - In most email clients (like Gmail, Outlook, or Yahoo), open the email message.  
   - Locate the option such as “Show Original,” “View Source,” or “View Message Headers” to access the full header information.  

2. Copy the entire email header text.  
   - Select all the header lines (from “Return-Path” to the start of the email body).  
   - Copy it for further analysis.  

3. Open a Mail Header Analyzer tool.  
   - Recommended tools:  
     - [MxToolbox Mail Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
     - [Google Admin Toolbox Messageheader](https://toolbox.googleapps.com/apps/messageheader/)  

4. Paste the copied email header into the analyzer’s input field on the chosen tool’s website.  

5. Run the analysis to extract technical details such as:  
   - Sender’s IP address  
   - Intermediate mail servers (hops)  
   - Message delay times between servers  
   - SPF, DKIM, and DMARC results  

6. Examine the authentication results:  
   - SPF (Sender Policy Framework): Verifies if the sender IP is authorized by the domain’s DNS.  
   - DKIM (DomainKeys Identified Mail): Checks if the message content was digitally signed by the domain.  
   - DMARC (Domain-based Message Authentication, Reporting & Conformance): Combines SPF and DKIM to detect spoofing or phishing attempts.  

7. Trace the sender’s IP address from the “Received” fields in the header.  
   - Identify the originating IP (usually the last “Received” entry from the bottom).  
   - Use an IP lookup tool to check its geolocation and ownership.  

8. Compare the originating IP with the claimed sender domain.  
   - If the IP location or domain does not match the sender’s organization, the email may be spoofed or forged.  

9. Document your findings by noting:  
   - Sender domain and IP  
   - Authentication results (SPF, DKIM, DMARC)  
   - Any inconsistencies or suspicious relay paths  

10. Save the analyzed report or export results from the analyzer tool for your forensic documentation.  

---

## Outputs

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

## Rubrics

| Criteria & Marks Assigned | <div align="center">Mark Allotted</div> | <div align="center">Mark Awarded</div> |
|:--|:--:|:--:|
| GitHub Activity & Submission Regularity | **3** |  |
| Application of Forensic Tools & Practical Execution | **3** |  |
| Documentation & Reporting | **2** |  |
| Engagement, Problem-Solving & Team Collaboration | **2** |  |
| **Total** | **10** |  |

---

## Result

The Mail Header Analyzer successfully traced the email’s origin and provided authentication details, helping to identify whether the email was genuine or spoofed.
