# Fedora Installation Checklist

> Replace each code block with the correct installation or download command for Fedora.

---

## Octave
```bash
sudo dnf install octave
```

## VS Code
```bash
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc &&
echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\nautorefresh=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/vscode.repo > /dev/null
dnf check-update &&
sudo dnf install code # or code-insiders

```

## Cursor
```bash
curl -LO "https://api2.cursor.sh/updates/download/golden/linux-x64-rpm/cursor/3.15"
```

## Cursor CLI Agent
```bash
curl https://cursor.com/install -fsS | bash
```

## Antigravity IDE
```bash
curl -LO "https://edgedl.me.gvt1.com/edgedl/release2/j0qc3/antigravity/stable/2.1.1-6123990880747520/linux-x64/Antigravity%20IDE.tar.gz"
```

## Antigravity
```bash
curl -LO "https://storage.googleapis.com/antigravity-public/antigravity-hub/2.7.1-5840911524036608/linux-x64/Antigravity.tar.gz"
```

## Antigravity CLI (agy)
```bash
curl -fsSL https://antigravity.google/cli/install.sh | bash
```

## Gemini CLI
```bash
mise install -g @google/gemini-cli
mise install -g @google/gemini-cli@latest
```

## mise
```bash
curl https://mise.run | sh
```

## uv
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Python
```bash
mise install python@latest
```

## Node.js & npm
```bash
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.6/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 26

# Verify the Node.js version:
node -v # Should print "v26.7.0".

# Verify npm version:
npm -v # Should print "11.19.0".

```

## Node.js & pnpm
```bash
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.6/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 26

# Verify the Node.js version:
node -v # Should print "v26.7.0".

# Install Corepack:
npm install -g corepack

# Download and install pnpm:
corepack enable pnpm

# Verify pnpm version:
pnpm -v
```

## pnpm
```bash
curl -fsSL https://get.pnpm.io/install.sh | sh -
```

## Bun
```bash
curl -fsSL https://bun.com/install | bash
```

## Rust
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Git
```bash
dnf install git (Fedora 22 and later) 
```

## GitHub CLI (gh)
```bash
sudo dnf install dnf5-plugins
sudo dnf config-manager addrepo --from-repofile=https://cli.github.com/packages/rpm/gh-cli.repo
sudo dnf install gh
```

## curl
```bash
sudo dnf install curl
```

## wget
```bash
# Install
sudo dnf install -y wget

# Verify
wget --version

```


## WireGuard
```bash
# Install tools
sudo dnf install -y wireguard-tools

# Verify
wg --version

```

## zip
```bash
# Install
sudo dnf install -y zip

# Verify
zip --version

```

## unzip
```bash
# Install
sudo dnf install -y unzip

# Verify
unzip -v

```

## UFW
```bash
# Install
sudo dnf install -y ufw

# Start and enable on boot
sudo ufw enable

# Verify status
sudo ufw status

```

## PostgreSQL
```bash
# Install server and utilities
sudo dnf install -y postgresql-server postgresql-contrib

# Initialize the database database cluster
# sudo postgresql-setup --initdb

# Start and enable the service on boot
# sudo systemctl enable --now postgresql

# Verify service status
# sudo systemctl status postgresql

```

## Redis
```bash
# Install the Redis package
sudo dnf install -y redis
# Start and enable the service on boot
# sudo systemctl enable --now redis
```

## Tailscale
```bash
# Add the official Tailscale repository and install
sudo dnf config-manager --add-repo https://tailscale.com
sudo dnf install -y tailscale
# Start the daemon and log in
# sudo systemctl enable --now tailscaled
# sudo tailscale up

```

## Postman
```bash
# Install via Flatpak (recommended for Fedora)
flatpak remote-add --if-not-exists flathub https://flathub.org
flatpak install flathub com.getpostman.Postman -y
```

## Anaconda
```bash
# Download the latest installer script
curl -O https://anaconda.com

# Run the installer script (Follow the prompts)
bash Anaconda3-2024.10-Linux-x86_64.sh
```

## miniconda
```bash
# Download the latest Miniconda installer script for Linux x86_64
curl -O https://anaconda.com

# Run the installer script (Press Enter and type 'yes' to accept the terms)
bash Miniconda3-latest-Linux-x86_64.sh -b -p $HOME/miniconda3

# Initialize Miniconda for your bash shell
~/miniconda3/bin/conda init bash

# Reload your shell configuration to activate conda immediately
source ~/.bashrc
```

## AWS CLI
```bash
# Download and unpack the official installation zip bundle
curl "https://amazonaws.com" -o "awscliv2.zip"
unzip awscliv2.zip

# Run the installer script
sudo ./aws/install
```

## CMake
```bash
# Install CMake via native package manager
sudo dnf install -y cmake
# Verify installation
cmake --version
```

## Ninja Build
```bash
# Install Ninja via native package manager
sudo dnf install -y ninja-build

# Verify installation
ninja --version
```

## LM Studio
```bash
# Install the official headless LM Studio CLI daemon
curl -fsSL https://lmstudio.ai/install.sh | bash

# Alternatively, if you need the desktop graphical app, download the AppImage:
# curl -LO https://lmstudio.ai -o LM_Studio.AppImage && chmod +x LM_Studio.AppImage
```

## Gemini Desktop
```bash
# Install Snapd support if missing
sudo dnf install -y snapd
sudo ln -s /var/lib/snapd/snap /snap

# Install Gemini Desktop via Snap Store
sudo snap install gemini-desktop

```

## Claude Code
```bash
# Run the official standalone install script
curl -fsSL https://claude.ai/install.sh | bash

# Verify the CLI
claude --version

```

## Codex CLI
```bash
# Install Codex CLI globally via npm
sudo mise install -g @openai/codex-cli

```

## OpenCode
```bash
curl -fsSL https://opencode.ai/install | bash

# or could install with bun

# bun add -g opencode-ai
```

## Hermes Agent
```bash
# Download and run the official script installer
curl -fsSL https://nousresearch.com | bash
```

## OpenClaw
```bash
# Install OpenClaw via npm (requires Node.js)
sudo mise install -g openclaw

```

## Ollama
```bash
# Run the official Ollama Linux single-command script installer
curl -fsSL https://ollama.com | bash

# Verify that the service is running
# sudo systemctl status ollama

```

## Docker Engine
```bash
# Install the core system dependencies
sudo dnf install -y dnf-plugins-core

# Set up the official Docker repository
sudo dnf config-manager --add-repo https://docker.com

# Install Docker Engine components
sudo dnf install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Start and enable Docker on system boot
# sudo systemctl enable --now docker

```

## Docker Desktop
```bash
# Set up the official repository (if not already done via Docker Engine)
sudo dnf config-manager --add-repo https://docker.com

# Download and install the latest Docker Desktop RPM package
curl -LO https://docker.com
sudo dnf install -y ./docker-desktop-x86_64.rpm

# Start the user-space service background daemon
# systemctl --user enable --now docker-desktop

```

## GitKraken
```bash
# Download the official GitKraken RPM package
curl -LO https://gitkraken.com

# Install using DNF to pull down missing dependencies
sudo dnf install -y ./gitkraken-amd64.rpm

```

## Obsidian
```bash
git clone https://github.com/obsidianmd/obsidian-releases/releases/download/v1.13.6/Obsidian-1.13.6-arm64.AppImage
```

## Zotero
```bash
# Add the community-maintained Zotero Fedora repository
# sudo curl -sL https://githubusercontent.com -o /etc/yum.repos.d/zotero.repo

# Install the application
sudo dnf install -y zotero

```

## Zettlr
```bash
# Download the official Zettlr RPM build file
# curl -LO https://github.com

# Install via DNF
sudo dnf install -y ./Zettlr.rpm

```

## qBittorrent
```bash
# Install the native desktop interface client
sudo dnf install -y qbittorrent

# If running a headless server instead, run: sudo dnf install -y qbittorrent-nox

```

## Balena Etcher
```bash
# Add the official repository hosted on Cloudsmith
# curl -1sLf 'https://cloudsmith.io' | sudo -E bash

# Update DNF lists and install Balena Etcher
sudo dnf install -y balena-etcher-electron

```

## Spotify
```bash
snap install spotify
```

## Syncthing
```bash
# Install the native Syncthing engine package
sudo dnf install -y syncthing

# Start and enable the tool for your current logged-in user session
systemctl --user enable --now syncthing.service

```

## TradingView
```bash
# Install TradingView Desktop via Flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org
flatpak install flathub com.tradingview.Desktop -y

```

## Firefox
```bash
# Install or update the native Fedora build variant
sudo dnf install -y firefox

```

## Google Chrome
```bash
# Enable the pre-configured Fedora third-party repository for Chrome
sudo dnf config-manager --set-enabled google-chrome

# Pull down and install the Google Chrome stable build
sudo dnf install -y google-chrome-stable

```

## Microsoft Edge
```bash
# Add the official Microsoft Edge repository signature keys
sudo rpm --import https://microsoft.com
sudo dnf config-manager --add-repo https://microsoft.com

# Install the Microsoft Edge stable application package
sudo dnf install -y microsoft-edge-stable
```

## draw.io
```bash
# Install the draw.io diagram utility bundle via Flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org
flatpak install flathub jgraph.drawio.desktop -y
```

## VLC
```bash
# Enable the required RPM Fusion repository (free branch)
sudo dnf install -y https://rpmfusion.org(rpm -E %fedora).noarch.rpm

# Install VLC media player
sudo dnf install -y vlc

```

## FFmpeg
```bash
# Enable both Free and Nonfree branches of the RPM Fusion library
sudo dnf install -y https://rpmfusion.org(rpm -E %fedora).noarch.rpm https://rpmfusion.org(rpm -E %fedora).noarch.rpm

# Upgrade existing multimedia libraries and install the complete FFmpeg kit
sudo dnf swap -y ffmpeg-free ffmpeg --allowerasing

```


## htop
```bash
# Install the native system terminal process tracker
sudo dnf install -y htop

```

## btop
```bash
# Install the btop graph-centric terminal engine
sudo dnf install -y btop

```

## tmux
```bash
# Install the native tmux terminal window workspace manager
sudo dnf install -y tmux
```

## Warp
```bash
# Download and install the official Warp Terminal RPM package
curl -LO https://warp.dev
sudo dnf install -y ./Warp.rpm

# or install warp using curl 
curl -LO "https://app.warp.dev/download?package=rpm"

```

## NVIDIA Settings
```bash
# Ensure the RPM Fusion Nonfree repository is active
sudo dnf install -y https://rpmfusion.org(rpm -E %fedora).noarch.rpm

# Install the primary NVIDIA graphics driver package along with settings panels
sudo dnf install -y akmod-nvidia xorg-x11-drv-nvidia-cuda nvidia-settings
```

## OpenRazer
```bash
# Enable the hardware driver copr channel profile
sudo dnf copr enable -y openrazer/openrazer

# Install the daemon and driver configuration kit
sudo dnf install -y openrazer-meta
```

## Polychromatic
```bash
# Enable the user interface control layout engine channel
sudo dnf copr enable -y jbicha/polychromatic

# Install the Polychromatic control app
sudo dnf install -y polychromatic
```
