# phigrOS Phi Plugin Guide using TRSS-Yunzai

A complete **English guide** for setting up the **Phi plugin** on **TRSS-Yunzai** with Discord bot integration and TapTap account binding.

> [!WARNING]
<<<<<<< HEAD
> Under construction ! Will be ready in a week or two .
=======
> Under construction !
>>>>>>> 11c4d6b26d0715a023d8952d5c343493991eb157


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
<<<<<<< HEAD
> Any VM is recommended while using a 3rd paty code.
=======
> Any VM is recommended while using a 3rd party code.
>>>>>>> 11c4d6b26d0715a023d8952d5c343493991eb157
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

<<<<<<< HEAD
Open Power Shell as administrator and paste these commands one by one.
=======
Open Power Shell and paste these commands one by one.
>>>>>>> 11c4d6b26d0715a023d8952d5c343493991eb157
```
# Download and install Chocolatey:
powershell -c "irm https://community.chocolatey.org/install.ps1|iex"
```
```
# Download and install Node.js:
choco install nodejs --version="24.7.0"
``` 
<<<<<<< HEAD
Close powershell ; open command prompt and do the following one by one:
Verify the Node.js version:
```
node -v # Should print "vx.x.x".
```
Download and install pnpm:
```
npm install -g pnpm
=======
```
# Verify the Node.js version:
node -v # Should print "vx.x.x".
```
```
# Download and install pnpm:
corepack enable pnpm
>>>>>>> 11c4d6b26d0715a023d8952d5c343493991eb157
```
```
# Verify pnpm version:
pnpm -v
```
2. Install [MSYS2](https://www.msys2.org/)
<<<<<<< HEAD

> [!TIP]
>+For installing check for correct version, for Intel based PCs use x86-64 version otherwise for Apple and Qualcomm based PCs use ARM version under windows enviroment.

+After Installation open MSYS2 UCRT64, run the following command

```
pacman -S mingw-w64-ucrt-x86_64-gcc base-devel git cmake
```
=======
>>>>>>> 11c4d6b26d0715a023d8952d5c343493991eb157
