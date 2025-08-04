# 🔍 Nmap LAN Scan Report

This project demonstrates how to scan your local network using **Nmap**, export the results in **XML format**, and convert it into a **readable HTML report** using `xsltproc`.

---

## 💻 Tools Used
- Kali Linux
- Nmap
- Xsltproc
- Bash commands
- Git

---

## 📁 Files Included
- `scan.xml` – Raw XML output of Nmap scan
- `scan.html` – Converted HTML report
- `screenshot.png` – Screenshot of the terminal and commands used
- `README.md` – This file

---

## 🧪 Steps Performed

### 1️⃣ Run Nmap scan and save output to XML:
```bash
sudo nmap -sS -oX scan.xml 192.168.1.0/24

### 2 Convert XML to HTML using xsltproc:
```bash
xsltproc scan.xml -o scan.html

### 3 Open the HTML file
```bash
 xdg-open scan.html

