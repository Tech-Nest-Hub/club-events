## Kali Linux installation guide/resources

### overview

kali Linux is a Debian-based Linux distribution built for penetration testing and security research, with pre-installed hacking and forensics tools.
This is a simple guide to install Kali Linux ISO image and proceed the installation in the VMware.

<img src='/images/kali-linux/icon.png' height="200px" alt='kali linux icon'>

### prerequisites

> [!NOTE]
> Use the minimum requirements in the Guest Machine if you have a potato host machine. Otherwise you can use the recommended requirements.

#### Host Machine Requirements

| Components | Requirement                             |
| ---------- | --------------------------------------- |
| RAM        | 8 GB or above                           |
| Disk Space | at least 40 GB or above free disk space |

#### Virtual Machine Requirements

| Components | Requirement                     |
| ---------- | ------------------------------- |
| RAM        | 2 GB (4 GB recommended)         |
| Disk Space | 20 GB (40 GB recommended)       |
| CPU Cores  | 2 (3-4 for smoother experience) |
| Network    | NAT or Bridged                  |

#### step - 1

Go to the official [www.kali.org](https://www.kali.org) and click the **Download** button.

<img src='/images/kali-linux/kali-org.png' alt='landing page'>

#### step - 2

Select the Virtual Machines as the platform as shown in the image below.

<img src='/images/kali-linux/choose-download.png' alt='choose download'>

#### step - 3

Download the iso image for the VMware.

<img src='/images/kali-linux/download.png' alt='download'>

#### step - 4

After installing the Kali Linux ISO image you can follow the Kali Linux's Official Documentation Guide for booting and initial setup for VMware **[here](https://www.kali.org/docs/virtualization/install-VMware-guest-vm/)**.

<img src="/images/kali-linux/insidevm.png" alt='inside vm'>

#### step - 5

After booting and the initial setup for the VMware follow **[THIS](https://www.kali.org/docs/installation/hard-disk-install/)** documentation to proceed with the system installation inside the VMware.

<img src="/images/kali-linux/install-kali.png" alt='install kali'>
