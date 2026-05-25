# phigrOS Phi Plugin Guide using TRSS-Yunzai

A complete **English guide** for setting up the **Phi plugin** on **TRSS-Yunzai** with Discord bot integration and TapTap account binding.

> [!WARNING]
> Under construction !


## What this guide is for ?

+ Set up [TRSS-Yunzai](https://github.com/TimeRainStarSky/TRSS_Yunzai) (a multi-functional bot framework).
+ Install and configures the Phi plugin.
+ Integrate TapTap API to fetch phigrOS stats automatically.
+ Link everything to Discord for smooth, automated updates.
+ Explains international TapTap login workaround for **non-CN players**.

## Prerequisities
### Core Setup
+ Node.js ≥ 18.x
+ npm ≥ 9.x
+ pnpm ≥ 8.x (used by TRSS-Yunzai)
+ msys2 (required for gcc/g++)
+ gcc & g++ compilers (install via msys2 pacman)
+ Git (Earlier stable versions will do)

### Optional 
+ VirtualBox / VMware + Windows 10 ISO (keeps your main OS safe)
+ Discord Bot Token (for integration)
+ TapTap Global Account (for phigrOS binding)

> [!CAUTION]
> Any VM is recommended while using a 3rd party code.
>
> [Oracle *Virtual Box* Download Page](https://www.oracle.com/in/virtualization/technologies/vm/downloads/virtualbox-downloads.html)

## *Step 1*— Installing Virtual Box and Windows Iso
> If you’re running directly on Windows, skip this step.
1. Download and install VirtualBox or VMware.
2. Mount the Windows 10 ISO and install inside a VM.
3. Allocate 3GB RAM or more (improves performance by ~30%) with atleast 3+ cores (recommended for octa core CPUs, if you have more than 8 cores you can allot more). 
4. Take a snapshot right after Windows boots successfully.

> [!TIP]
> Check this [YT video](https://youtu.be/CMGa6DsGIpc?si=7keT3v4uFfHHsHF1) if you need help

## Step 2- Installing Core Tools 
1. Install [Node + npm + pnpm](https://nodejs.org/en/download/current). LTS version is recommended.

We will use Chocolatey for installing Node

Open Power Shell and paste these commands one by one.
```
# Download and install Chocolatey:
powershell -c "irm https://community.chocolatey.org/install.ps1|iex"
```
```
# Download and install Node.js:
choco install nodejs --version="24.7.0"
``` 
```
# Verify the Node.js version:
node -v # Should print "vx.x.x".
```
```
# Download and install pnpm:
corepack enable pnpm
```
```
# Verify pnpm version:
pnpm -v
```
2. Install [MSYS2](https://www.msys2.org/)
