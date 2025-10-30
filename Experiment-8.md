### 🎯 Aim
To examine image files for the presence of hidden information using **StegExpose**, a Java-based steganalysis tool.

---

### 🧰 Tools & Requirements
| Tool / Resource | Purpose |
|-----------------|---------|
| **StegExpose.jar** | Java program that evaluates images for steganography |
| **Java Runtime Environment (JRE)** | Needed to run `.jar` files |
| **Command Prompt / Terminal** | Execute commands and run StegExpose |
| Image files (.png, .jpg, .bmp) | Samples to analyze for hidden data |

---

### ⚙️ Procedure

#### Step 1: Set Up the Environment
1. Download **StegExpose.jar** from its [GitHub repository](https://github.com/b3dk7/StegExpose).  
2. Make sure **Java** is installed on your system.  
3. Place both the `.jar` file and the images you want to inspect in the same working folder.
<p align="center">
<img width="1035" height="571" alt="8 1" src="https://github.com/user-attachments/assets/8ba81c6d-e729-426b-8625-4648d3b3d1f2" />
</p>

---

#### Step 2: Select Target Images
- Identify the images you suspect may contain hidden data.  
- StegExpose works with `.png`, `.jpg`, and `.bmp` formats.
<p align="center">
<img width="1519" height="689" alt="8 6" src="https://github.com/user-attachments/assets/7b8740c3-7c1b-494d-b969-e4947d6edaba" />
</p>

---

#### Step 3: Launch Terminal or Command Prompt
- Navigate to the folder where `StegExpose.jar` is located.  
- Open the **Command Prompt** (Windows) or **Terminal** (macOS/Linux).
<p align="center">
<img width="1722" height="932" alt="8 8" src="https://github.com/user-attachments/assets/eedf6c60-50b2-4bb9-bf14-c572ce957e27" />
</p>

---

#### Step 4: Analyze a Single Image
To check one image at a time, run:
```bash
java -jar StegExpose.jar <image_file_path>
```
**Example:**
```bash
java -jar StegExpose.jar secret_photo.png
```
<p align="center">
<img width="1919" height="1000" alt="8 11" src="https://github.com/user-attachments/assets/502a8f36-0b3e-4c0b-9aa6-b46283ea85c5" />
</p>

---

#### Step 5: Interpret the Scores
- StegExpose outputs a **suspect score** from 0 to 1.  
- Higher values indicate a higher probability of hidden data.  

| Score | Interpretation |
|-------|----------------|
| < 0.2 | Likely clean |
| 0.2–0.3 | Possibly contains hidden data |
| > 0.3 | Hidden data probable |

---

#### Step 6: Scan Multiple Images
- To analyze an entire folder:
```bash
java -jar StegExpose.jar <folder_path>
```
- Each image will be assigned a score, allowing batch evaluation.

---

#### Step 7: Optional Features
- To explore additional command-line options:
```bash
java -jar StegExpose.jar --help
```

---

### 🔎 Observations
| Image | Score | Assessment |
|-------|-------|------------|
| secret_photo.png | 0.45 | High likelihood of hidden data |
| holiday_pic.jpg | 0.12 | No hidden data detected |

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

### 📈 Result
StegExpose successfully flagged images likely containing hidden data. Images with low scores were considered clean, while higher scores indicated probable steganography.

---
