## Aim

To capture and analyse network packets using Wireshark and extract login credentials transmitted via insecure protocols.

## Tools Used

•	Wireshark

•	Windows/Linux system

•	Web browser(http://testphp.vulnweb.com/login.php)

## Procedure

1.	Open Wireshark and select the active network interface (e.g., Wi-Fi).
2.	Start packet capturing to record live network traffic.
3.	Open a website using HTTP protocol and log in with sample credentials.
4.	Stop the capture after submitting the login form.
5.	Apply the display filter http to view only HTTP packets.
6.	Search for requests with GET and POST methods.
7.	Expand the HTTP packet details to locate form data containing the captured username and password.

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

## Result

Wireshark successfully captured network packets and revealed the transmitted login credentials from an insecure HTTP website.



