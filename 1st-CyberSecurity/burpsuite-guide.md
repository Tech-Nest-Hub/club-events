## Burpsuite installation guide

### overview

The Burp Suite should be installed by default in Kali Linux. If it is not installed by default then you can simply follow the guides below.

### Using GUI

Go to the official download page [portswigger.net](https://portswigger.net/burp). Click on the **Products** in the navbar and choose the 'Burp Suite Community Edition'.

<img src="/images/burp-suite/selection.png">

#### Click the download button.

<img src="/images/burp-suite/download.png">

#### Select the "Linux (x64)" or Linux(ARM)

> [!NOTE]
> **x64 vs ARM:** Pick based on your CPU
>
> - **x64** (x86_64/amd64) — most laptops, desktops, servers (Intel/AMD)
> - **ARM** (aarch64/arm64) — Raspberry Pi, ARM-based laptops, AWS Graviton, etc.
>
> Check yours by running `uname -m` in a terminal:
> `x86_64` → **x64** build · `aarch64`/`arm64` → **ARM** build

<img src="/images/burp-suite/final.png">

And finally run the following command by making the file executable.

```bash
cd `/Downloads
chmod +x burpsuite_community_linux_v*.sh
sudo ./burpsuite_community_linux_v*.sh
```

### Using Terminal

The other way around is by using terminal. Open any terminal emulators and type the following commands or just copy paste it.

```bash
sudo apt update
sudo apt install burpsuite -y
```

<img src="/images/burp-suite/terminal.png">
