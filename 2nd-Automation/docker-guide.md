# Docker Setup: Linux CLI & Windows Desktop

> [!NOTE]
> This guide covers Docker Engine from the command line on Ubuntu and Docker
> Desktop on Windows. Neither setup requires a Docker account.

## prerequisites

- A supported 64-bit Ubuntu or Windows computer
- An internet connection
- An Ubuntu user account with `sudo` access (for the CLI setup)

> [!WARNING]
> Docker-published ports can bypass `ufw` or `firewalld` rules. Only expose
> ports you intend to make reachable.

## installation
Run these commands in a terminal.

[reference](https://docs.docker.com/engine/install/ubuntu/)


```bash
# Add Docker's official repository
sudo apt update
sudo apt install -y ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

sudo tee /etc/apt/sources.list.d/docker.sources > /dev/null <<EOF
Types: deb
URIs: https://download.docker.com/linux/ubuntu
Suites: $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}")
Components: stable
Architectures: $(dpkg --print-architecture)
Signed-By: /etc/apt/keyrings/docker.asc
EOF

# Install Docker Engine and Docker Compose
sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

## check if it works

Run this command:

```bash
sudo systemctl start docker
sudo systemctl enable docker
```

```bash
sudo docker run hello-world
```

If Docker prints a welcome message, the installation is complete. Use `sudo`
before Docker commands on this setup.

## Windows installation (Docker Desktop)

1. Download [Docker Desktop for Windows](https://www.docker.com/products/docker-desktop/)
2. Run `Docker Desktop Installer.exe`
3. Keep **Use WSL 2 instead of Hyper-V** selected when prompted
4. Finish the installation, then open Docker Desktop
5. Accept the terms; wait until Docker Desktop shows that it is running

## check if it works on Windows

Open PowerShell or Command Prompt and run:

```bash
docker run hello-world
```

If Docker prints a welcome message, Docker Desktop is ready to use.

> [!TIP]
> For Debian, Fedora, Arch, or another Linux distribution, follow Docker's
> [official Linux Engine installation guide](https://docs.docker.com/engine/install/)
> for the matching CLI commands.
