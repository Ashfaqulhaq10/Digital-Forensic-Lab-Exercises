## Aim

To capture and analyse network packets using Wireshark and extract login credentials transmitted via insecure protocols.

## Tools Used

•	Wireshark

•	Windows/Linux system

•	Web browser(http://testphp.vulnweb.com/login.php)

## Procedure

> **Safety note:** Only perform this exercise in a controlled lab environment using **your own test site/accounts** or intentionally vulnerable test pages (do NOT capture credentials from real users or live production sites). Most modern sites use HTTPS, so use a local/test HTTP page or a purposely configured lab server for this exercise.

1. Open **Wireshark**.  
2. From the interface list, select the **active network interface** (e.g., Wi-Fi or Ethernet) that carries the traffic you want to capture.  
3. (Optional) Set a capture file name and destination: `File → Capture File Properties` or click the disk icon during capture to save packets to a file.  
4. Click **Start** (the shark-fin icon) to begin live packet capture.  
5. In your browser (on the same machine or another machine on the same network), open a **test HTTP website** (not HTTPS) that contains a login form. Use **sample/test credentials** you control.  
6. Complete the login form and submit it.  
7. Return to Wireshark and click **Stop** to end the capture once the form submission completes.  
8. In the **Display Filter** box enter `http` and press Enter to show only HTTP traffic.  
9. Look for HTTP requests using `GET` and `POST` methods:
   - Use the **Info** column to quickly spot `GET / ...` and `POST / ...` lines.  
   - You can refine the filter for POSTs with `http.request.method == "POST"`.  
10. Select a candidate HTTP `POST` packet (often the form submission).  
11. Expand the packet details (click the ▸ next to the packet) and open the **Hypertext Transfer Protocol** section:  
    - Inspect **Request Method**, **Request URI**, and **Content-Type** headers.  
    - If form data is present, it will appear under the HTTP section (e.g., `application/x-www-form-urlencoded` body).  
12. To view the full request/response payload together, right-click the packet and choose **Follow → TCP Stream** (or **Follow → HTTP Stream** on newer Wireshark builds). This reconstructs the conversation and shows POST body contents (where form fields and values often appear).  
13. Search within the stream or packet bytes for likely form field names such as `username`, `user`, `email`, `password`, `pwd`, etc., to locate captured credentials. Use `Ctrl+F` and choose **String** or **Packet bytes** to search.  
14. Note timestamps, source/destination IPs and ports, HTTP headers, and the exact payload when documenting your findings.  
15. Export relevant packets or the whole capture for lab reporting: `File → Export Specified Packets` or `File → Save As` to keep an evidence file (PCAP).  
16. Record chain-of-custody details for your capture file (who captured it, when, system used, storage location) and ensure the capture file is secured.  

**Tips & troubleshooting**
- If you see nothing with `http`, the site likely used HTTPS — HTTPS traffic will not reveal form data because it’s encrypted. Use a local HTTP test server (e.g., a simple web form hosted on `http://localhost` or an intentionally vulnerable VM) for this lab.  
- Use `http.request` and `http.response` filters to find requests/responses quickly.  
- Use **Statistics → HTTP** or **Endpoints/Conversations** for high-level HTTP activity summaries.  
- Always save a copy of the original capture (PCAP) before performing any analysis that modifies files.



## Screenshots

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/92b19333-2c56-4fa9-8395-9eb789ba4c5f" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/f8dfbdfd-4e4d-4827-9812-d3c92d652a76" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/3dd6978f-ff02-4291-809e-c130e33db4dc" />
</p>

---

<p align="center">
<img width="600" alt="image" src="https://github.com/user-attachments/assets/2624a318-7b4f-4b5c-9ca9-45e80e6e274d" />
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

Wireshark successfully captured network packets and revealed the transmitted login credentials from an insecure HTTP website.



