# OWASP ZAP Installation Guide

## Introduction

OWASP ZAP (Zed Attack Proxy) is a free and open-source web application security scanner used to identify vulnerabilities in web applications.

Official Website:
https://www.zaproxy.org/

---

## Step 1: Visit the Official Website

Go to:

https://www.zaproxy.org/

![alt text](home.png)
---

## Step 2: Open the Download Page

Click **Download** or visit:

https://www.zaproxy.org/download/

![alt text](zap1-1.png)


---

## Step 3: Download Linux Installer

Select the Linux Installer (.sh).

![alt text](zap2-1.png)

## Step 4: Open Terminal

Navigate to the Downloads folder.

```bash
cd ~/Downloads
```

## Step 5: Make Installer Executable

```bash
chmod +x ZAP_*.sh
```

![alt text](zap3.png)

## Step 6: Run the Installer(In root)

```bash
./ZAP_*.sh
```

![alt text](zap4.png)

## Step 7: Installation Wizard

Follow the installation wizard.

- Accept the license.
- Choose installation location.
- Continue until installation finishes.

![alt text](zap5.png)

![alt text](zap6.png)

![alt text](zap7.png)

![alt text](zap8.png)

![alt text](zap9.png)

## Step 8: Launch ZAP

Start OWASP ZAP from the Applications menu or terminal.

![alt text](zap10.png)

---

## Step 9: Welcome Screen

When ZAP launches successfully, you should see the welcome screen.

![alt text](zap11.png)

---

## Conclusion

OWASP ZAP has been successfully installed and is now ready for web application security testing.