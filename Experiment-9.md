### 🎯 Aim
To monitor and analyze running processes on a Windows system to detect potentially malicious or suspicious activity using **Process Explorer**.

---

### 🧰 Tools & Requirements
| Tool / Resource | Purpose |
|-----------------|---------|
| **Process Explorer** | Advanced Windows utility for process monitoring |
| **Windows OS** | Required platform to run the tool |
| **Administrator Privileges** | Needed to access all system processes |
| **Internet Connection** | For verifying suspicious process reputations |

---

### ⚙️ Procedure

#### Step 1: Download and Launch
1. Go to the [Microsoft Sysinternals Process Explorer page](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer).  
2. Download the ZIP archive.  
3. Extract the folder to a working directory.  
4. Run `procexp64.exe` or `procexp.exe` **as Administrator**.
<p align="center">
<img width="1223" height="753" alt="Screenshot 2025-10-28 000259" src="https://github.com/user-attachments/assets/578a5fee-a6d7-4ca3-bf51-757d7f86d1b3" />
</p>

#### Step 2: Explore the Interface
- The process tree shows all active processes.  
- Color coding for quick status recognition:

| Color | Meaning |
|-------|---------|
| Pink | Suspended processes |
| Light Blue | Processes under the same user |
| Dark Blue | System services or processes running under system accounts |
| Green | Newly started processes |
| Red | Recently terminated processes |
<p align="center">
<img width="1271" height="770" alt="Screenshot 2025-10-28 000326" src="https://github.com/user-attachments/assets/de02cbd3-e460-4a03-a20c-291bc4a38e4d" />
</p>

#### Step 3: Investigate Suspicious Processes
1. **Unknown processes**: Look for unfamiliar names; system processes are usually from trusted vendors like Microsoft.  
2. **Digital signatures**: Right-click → Properties → Image tab. Unsigned executables can be suspicious.  
3. **File path**: System files are normally in `C:\Windows\System32`; others may be risky.  
4. **Resource usage**: High CPU, memory, or disk usage can indicate malware.  
5. **Process details**: Lack of description or unclear company name may be suspicious.  
6. **Network activity**: Properties → TCP/IP tab; unexpected connections may indicate malicious behavior.

#### Step 4: Verify Process Reputation
- Search the process name online.  
- Check databases like [VirusTotal](https://www.virustotal.com/) or [ProcessLibrary](https://www.processlibrary.com/).
<p align="center">
<img width="1191" height="762" alt="Screenshot 2025-10-28 000341" src="https://github.com/user-attachments/assets/923e8d6f-8982-477d-8767-2593b91e79e5" />
</p>


#### Step 5: Take Action
1. **Kill Process**: Right-click → Kill Process.  
2. **Suspend Process**: Right-click → Suspend.  
3. **Delete Executable**: Remove the file if confirmed malicious.

#### Step 6: Scan the System
- Run a full antivirus scan.  
- Use tools like Malwarebytes or Windows Defender for thorough cleaning.
<p align="center">
<img width="1246" height="732" alt="Screenshot 2025-10-28 000403" src="https://github.com/user-attachments/assets/509129b0-a70d-4f35-98e9-8ddc9e978db9" />
</p>

---

### 🔍 Observations
| Process Name | Action Taken | Notes |
|--------------|--------------|-------|
| unknown.exe | Suspended | Running from Temp folder, unsigned |
| svchost.exe | Monitored | Legitimate system process, high CPU briefly |
| appdatahelper.exe | Killed | Malicious, confirmed via VirusTotal |

---

### 📈 Result
Process Explorer successfully identified suspicious or unusual processes and allowed safe investigation and corrective action.

---

### 📚 Conclusion
Process Explorer provides detailed monitoring of Windows processes. Combining process inspection with reputation verification helps detect malware and protect system integrity.

---
