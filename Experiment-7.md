
## 🎯 Aim
To extract logical user data such as **contacts, SMS, MMS, and call logs** from an Android phone using **AFLogical OSE** and **Android Debug Bridge (ADB)**.

---

## 🧰 Tools & Requirements
| Tool/Item | Description |
|------------|--------------|
| **AFLogical OSE** | Open-source Android forensics tool for logical extraction |
| **Java Runtime Environment** | Required for running AFLogical |
| **Android Debug Bridge (ADB)** | Communication tool between computer and Android device |
| **USB Cable** | For device connection |
| **Android Phone** | Test device with USB debugging enabled |

---

## ⚙️ Procedure

### Step 1: Setup Environment
1. Install **Java** and **ADB** on the system.  
2. Download the **AFLogical OSE APK** file from its GitHub page.  
3. Enable **Developer Options → USB Debugging** on the Android device.

<p align="center">
<img width="1919" height="1020" alt="Screenshot 2025-10-27 231249" src="https://github.com/user-attachments/assets/0e1aaeed-b4b2-4095-b726-2ded21e0220b" />
</p>

### Step 2: Connect Android Device
1. Connect the phone via USB cable.  
2. Verify the connection:
```bash
adb devices
```
<p align="center">
<img width="964" height="378" alt="Screenshot 2025-10-27 231521" src="https://github.com/user-attachments/assets/c2d97132-97f8-4a74-bf7d-078067f99800" />
</p>
3. Grant permission if prompted on the device.

### Step 3: Install AFLogical OSE
Install the APK file on the Android phone:
```bash
adb install aflogical_ose.apk
```
<p align="center">
<img width="1916" height="1079" alt="7 7" src="https://github.com/user-attachments/assets/9f0db9af-055f-4d46-aced-d958e97cf261" />
</p>

### Step 4: Run AFLogical
1. Open **AFLogical OSE** on the device.  
2. Choose data categories (Contacts, SMS, MMS, Call Logs).  
3. Tap **Extract Data**.  
4. Files are saved to:
```
/sdcard/aflogical/
```

### Step 5: Transfer Extracted Data
Copy data to the computer:
```bash
adb pull /sdcard/aflogical/ ./ForensicsOutput
```
<p align="center">
<img width="1919" height="1075" alt="7 8" src="https://github.com/user-attachments/assets/6ccb3253-cdce-42e4-9a1c-5119fd7b01c0" />
</p>

### Step 6: Analyze Extracted Data
- Open `.csv` files in Excel or Google Sheets.  
- Review and document important findings (timestamps, numbers, message text, etc.).
<p align="center">
<img width="1918" height="1078" alt="7 9" src="https://github.com/user-attachments/assets/a19244cd-d178-46f5-880d-155d578e93e2" />
</p>

### Step 7: Clean Up
Uninstall the app after completion:
```bash
adb uninstall com.viaforensics.android.aflogical
```

---

## 🔍 Observations
| File | Contents |
|------|-----------|
| contacts.csv | Contact list with names and numbers |
| sms.csv | Text messages sent and received |
| mms.csv | Multimedia message records |
| calllog.csv | Incoming, outgoing, and missed calls |

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

## 📈 Result
Logical extraction was successfully performed using **AFLogical OSE**.  
Extracted data was saved in `.csv` format and verified using spreadsheet software.

---
