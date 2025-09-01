## Aim

To examine a disk image or folder with Autopsy, extract digital artifacts, and generate a forensic report.

## Tools Used

•	Autopsy (open-source DFIR suite)

•	Windows/Linux system

•	Evidence source: disk image (E01/RAW/VHD) or folder

## Procedure

1.	Launch Autopsy → Create New Case (enter case name, base directory, investigator).
2.	Add Data Source → choose Disk Image/VM file, Local Disk, or Logical Files, then browse to the evidence.
3.	In Ingest Modules, select: File Type Identification, Embedded File Extractor, Recent Activity (web artifacts), EXIF Parser/Metadata, Keyword Search (add terms if needed), and Hash Lookup (optional).
4.	Start Ingest and monitor progress/messages until processing completes.
5.	Review results in the left tree: Recent Activity, Web History/Downloads, Documents/Images/Videos, Deleted Files, Installed Programs, etc.
6.	Use Timeline and Filters to focus on relevant activity; preview items and Export artifacts if required.
7.	Go to Tools → Generate Report → choose HTML/PDF/CSV, select result types, and save the report to the case folder.

## Screenshots

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

## Result

Autopsy successfully parsed the evidence, recovered key artifacts (files, metadata, web/browser activity, keyword hits), and produced a structured forensic report.










