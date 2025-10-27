# Use Sleuth Kit to Analyze Digital Evidence

---

## Aim
To understand and demonstrate the usage of Sleuth Kit in analyzing digital evidence for forensic investigation purposes.

---

## Description
The Sleuth Kit (TSK) is a powerful open-source digital forensics toolkit that enables investigators to analyze disk images and recover files. This experiment focuses on using various Sleuth Kit commands and tools to examine digital evidence, recover deleted files, and analyze file system artifacts.

---

## Tools Used
1. The Sleuth Kit (TSK)
2. Command Line Interface
3. Disk Image (for analysis)
4. AutopsyⓇ (GUI frontend for Sleuth Kit)

---

## Procedure

### 1. Installation and Setup
1. Download and install The Sleuth Kit from the official website.
2. Verify the installation by running basic commands.
3. Prepare a disk image for analysis.

### 2. File System Metadata Analysis
1. Use `fsstat` to display the partition layout:

```bash
fsstat -o 0 TestImage.dd
```
<p align="center">
<img width="877" height="810" alt="Screenshot 2025-10-27 222101" src="https://github.com/user-attachments/assets/258e85af-7788-40ca-95c2-8a160b8ae03a" />
</p>

### 3. List Files and Directories:
List all files and directories in the disk image:
      
```bash
fls -o 0 TestImage.dd
```

## Observation:
Shows all allocated files. Note the inode numbers for files you want to recover. For example:
r/r 4: testfile.txt
<p align="center">
<img width="983" height="532" alt="Screenshot 2025-10-27 222117" src="https://github.com/user-attachments/assets/a5ec16d5-ed7a-4d7a-a42f-aa78bb495f71" />
</p>

### 4.Recover a File
Extract a file using its inode number:
```bash
icat -o 0 TestImage.dd 4 > recovered_file.txt
```

## Observation:
The file testfile.txt is successfully recovered. You can check its content:
type 
### recovered_file.txt

<p align="center">
<img width="1448" height="829" alt="Screenshot 2025-10-27 222232" src="https://github.com/user-attachments/assets/ab772099-57d8-420f-af0c-2810953406ea" />
</p>

### 5. Analyze File Metadata:
Use this command to display the metadata of a file:
```bash
istat -o 0 TestImage.dd 4
```
<p align="center">
<img width="877" height="810" alt="Screenshot 2025-10-27 222101" src="https://github.com/user-attachments/assets/d3f3a1eb-1b83-42bf-91d1-15a82fe121d4" />
</p>

---

## Results

- Successfully identified partition structure.
- Retrieved file system metadata.
- Recovered both active and deleted files.
- Verified timestamps and file attributes.
- Created a timeline of file system activities.

---

## Conclusion

The Sleuth Kit is an essential tool in digital forensics investigations, providing detailed insights into file systems and enabling investigators to recover and analyze digital evidence effectively. This experiment provided practical experience using TSK commands such as `mmls`, `fsstat`, `fls`, `icat`, `istat`, and optional timeline/deleted file analysis, which are crucial in real-world forensic investigations.
