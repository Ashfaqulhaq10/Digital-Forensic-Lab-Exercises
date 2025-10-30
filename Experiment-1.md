

## Aim:
To generate a reliable forensic image of a storage device (such as a USB drive or hard disk) using FTK Imager.


## Tools Used:
•	FTK Imager

•	Windows Operating System


## Procedure:

1. Launch **FTK Imager** on the system.  
2. From the **File** menu, choose **Create Disk Image** to start the acquisition process.  
3. In the dialog box, select the **source type**:
   - *Physical Drive* – to capture the entire disk.
   - *Logical Drive* – to capture a specific partition.
   - *Image File* – to duplicate an existing image.
   - *Folder Contents* – to acquire files from a selected directory.
4. Select the **source drive or partition** you wish to image and click **Finish**.  
5. Choose the **destination path** where the forensic image will be saved.  
6. Provide a **file name**, and select the **image format** (e.g., E01, RAW, SMART).  
7. Click **Add** to configure **case information** such as:
   - Case Number  
   - Evidence Number  
   - Examiner Name  
   - Description or notes (optional)
8. Review the **summary** of the acquisition settings and click **Start** to begin imaging.  
9. FTK Imager will create a **bit-by-bit copy** of the source and compute **hash values (MD5/SHA1)** automatically.  
10. Once the process completes, note the **hash values** displayed for verification purposes.  
11. Use the **Verify Image** option to ensure the acquired image exactly matches the original source.  
12. Add the created **image file** back into FTK Imager using **Add Evidence Item → Image File**.  
13. Browse and analyze the contents of the image to view files, deleted data, and metadata without modifying the original evidence.  


## Screenshots:

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/10f722a7-c519-484b-8922-f41251e4b347" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/30f1e7bc-5bfd-415c-8b69-5147ebc859d9" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f0c4faef-4caf-4bd4-a9b0-0f9028ceb1a1" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/7d3b98a8-cd47-4fdb-ae82-6647d8124ad5" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/67920f0b-eef0-4a5f-9e21-88420827b3c9" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/6832163b-bc62-4852-aa5c-4e072c522fd3" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/d7b60ee3-e9da-4f21-9ded-99fbca76dd3c" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/8d745e88-9f7f-4197-bc8b-07f050ab1ac6" />
</p>

---


<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/04d8e69e-866a-4555-863a-59da85d260ed" />
</p>


---


<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/2780f7cc-5c4a-4d42-a831-ada17ce3ef76" />
</p>



---



# Rubrics

| Criteria | Mark Allotted | Mark Awarded |
|---|---:|---:|
| 1. GitHub Activity & Submission Regularity | 3 | |
| 2. Application of Forensic Tools & Practical Execution | 3 | |
| 3. Documentation & Reporting | 2 | |
| 4. Engagement, Problem-Solving & Team Collaboration | 2 | |
| **Total** | **10** | |

---

# Result:
A forensic image of the selected folder was successfully created, verified, and analysed using FTK Imager. The experiment demonstrated the process of evidence acquisition and integrity verification in digital forensics.

---
