## Aim

To examine a disk image or folder with Autopsy, extract digital artifacts, and generate a forensic report.

## Tools Used

•	Autopsy (open-source DFIR suite)

•	Windows/Linux system

•	Evidence source: disk image (E01/RAW/VHD) or folder

## Procedure

1. Launch Autopsy and select Create New Case.  
   - Enter the case name, base directory, and investigator details, then click Finish to create the case.  

2. Add Data Source by choosing the appropriate option:  
   - Disk Image or VM File  
   - Local Disk  
   - Logical Files  
   Browse and select the evidence file or drive to be analyzed.  

3. In the Ingest Modules section, select the modules to be applied during analysis:  
   - File Type Identification  
   - Embedded File Extractor  
   - Recent Activity (web artifacts)  
   - EXIF Parser/Metadata  
   - Keyword Search (add keywords if required)  
   - Hash Lookup (optional, for comparing with known hash sets)  

4. Start the Ingest process and monitor the progress window or messages until the processing is complete.  

5. Review the analysis results in the left-hand tree panel.  
   - Explore categories such as Recent Activity, Web History, Downloads, Documents, Images, Videos, Deleted Files, and Installed Programs.  

6. Use Timeline and Filter options to focus on specific user actions or time periods.  
   - Preview selected files or artifacts.  
   - Export important evidence items if required.  

7. Navigate to Tools → Generate Report.  
   - Choose the desired report format (HTML, PDF, or CSV).  
   - Select the result types to include and specify the output location.  
   - Save the generated report to the case folder for documentation and submission.  

---

## Outputs

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d53592ca-6f90-41c9-b8c2-02627fc28c92" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d9c7ccae-108f-46d9-ae94-0af6d30bde68" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/aac0c47d-79c3-4bd2-a3c6-fe50afaa13cd" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f3a6b651-47af-4fef-be68-a25ca00575ae" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/67587e30-5a3d-40e4-80d9-4e10d9b2c2d9" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/b2b0c7e3-355e-40a9-b80e-ac7ed2ba9ea7" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/637d7d31-2195-4f2a-9c41-1869fb0bc1aa" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f794b427-6e9e-4618-9d7f-1d2aa06aefb5" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/69cb9e7b-fca1-4125-afd0-cf5a3e65d7f8" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/ec08a2bb-918a-49c6-9105-7fa3aabfc2b7" />
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

Autopsy successfully parsed the evidence, recovered key artifacts (files, metadata, web/browser activity, keyword hits), and produced a structured forensic report.










