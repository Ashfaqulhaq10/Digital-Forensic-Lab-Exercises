
## Aim

To recover lost or deleted partitions/files using the TestDisk forensic tool.

## Tools Used

•	TestDisk

•	Windows/Linux Operating System

## Procedure

1. **Launch TestDisk** from the command line or terminal window.  
   - On Windows, open the Command Prompt and run `testdisk_win.exe`.  
   - On Linux, open a terminal and run `sudo testdisk`.

2. At the startup screen, select **Create** to generate a new log file, or choose **Append** to continue an existing session log.

3. From the list of available **storage devices**, select the drive that needs to be analyzed and press **Enter**.

4. Choose the correct **partition table type** (usually detected automatically by TestDisk).  
   - For example: Intel/PC partition, EFI GPT, or Mac.

5. Select **Analyse** from the main menu to begin scanning the selected drive for lost or deleted partitions.

6. View the list of **current and deleted partitions** found during the analysis.  
   - Use the arrow keys to navigate through the detected partitions.

7. To inspect the contents of a partition, highlight it and choose **List Files**.  
   - This allows you to browse and verify the recoverable files before restoring.

8. Use the **Copy** option to recover selected files to a **safe destination folder** on another drive (not the same source drive).

9. If entire partitions are lost, select **Write** to restore the partition table after verifying the correct entries.

10. Exit TestDisk safely and review the **recovered data** in the chosen destination folder.

---

## Outputs

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/7932b64e-8f81-454a-a850-59a9d66ce704" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/7cd5a825-30e9-4461-893d-79ace2350540" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/9cb2805e-7d13-49bc-8e37-e6f921fbbbeb" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/82202635-86dd-42b2-b520-21fb2a84b758" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/c3a4c913-c33c-46e2-bc0e-7cac92423d6c" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/e6d835a5-6c2f-4660-bb3b-9a6931d50362" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/461ef53b-d38a-4472-92ee-8d7daf880b7f" />
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

Lost or deleted files/partitions were successfully identified and recovered using TestDisk.







