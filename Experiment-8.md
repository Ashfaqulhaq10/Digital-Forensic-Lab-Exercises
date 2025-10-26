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

---

#### Step 2: Select Target Images
- Identify the images you suspect may contain hidden data.  
- StegExpose works with `.png`, `.jpg`, and `.bmp` formats.

---

#### Step 3: Launch Terminal or Command Prompt
- Navigate to the folder where `StegExpose.jar` is located.  
- Open the **Command Prompt** (Windows) or **Terminal** (macOS/Linux).

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

### 📈 Result
StegExpose successfully flagged images likely containing hidden data. Images with low scores were considered clean, while higher scores indicated probable steganography.

---

### 📚 Conclusion
This experiment demonstrates how **StegExpose** can quickly and accurately detect steganography in images, making it a valuable tool for forensic investigations and security analysis.

---
