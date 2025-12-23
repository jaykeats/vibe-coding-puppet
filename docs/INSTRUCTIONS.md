# INSTRUCTIONS: Vibe Coding AI Puppet System
## Step-by-Step Setup & Execution Guide

**For:** Gemini CLI (and human operators)  
**Status:** Ready to execute  
**Last Updated:** Dec 14, 2025  

---

## SECTION 1: INITIAL SETUP

### 1.1 Prerequisites

Before starting, verify you have:
- Windows 10+ with PowerShell 5.0+
- Node.js 18+ and npm/pnpm
- Git installed
- Access to C:\ (internal SSD) and E:\ (external SSD)
- ~5GB free space on C:\
- ~100GB free space on E:\

**Verification Commands:**
```powershell
# Check Windows version
Get-WmiObject -Class Win32_OperatingSystem | Select-Object Caption, Version

# Check Node.js
node --version
npm --version

# Check disk space
Get-Volume | Select-Object DriveLetter, Size, SizeRemaining

# Check PowerShell version
$PSVersionTable.PSVersion
```

---

### 1.2 Create Folder Structure on External SSD

Run these PowerShell commands to create the asset library structure on E:\:

```powershell
# Create main project folder
mkdir E:\vibe_coding_puppet
mkdir E:\vibe_coding_puppet\generated_websites
mkdir E:\vibe_coding_puppet\component_library
mkdir E:\vibe_coding_puppet\design_assets
mkdir E:\vibe_coding_puppet\design_assets\images
mkdir E:\vibe_coding_puppet\design_assets\icons
mkdir E:\vibe_coding_puppet\design_assets\fonts
mkdir E:\vibe_coding_puppet\design_assets\color_palettes
mkdir E:\vibe_coding_puppet\templates
mkdir E:\vibe_coding_puppet\backups

# Verify folders were created
Get-ChildItem E:\vibe_coding_puppet -Recurse | Select-Object FullName
```

**Expected Output:**
```
E:\vibe_coding_puppet\
├── generated_websites\
├── component_library\
├── design_assets\
│   ├── images\
│   ├── icons\
│   ├── fonts\
│   └── color_palettes\
├── templates\
└── backups\
```

---

### 1.3 Set Up Project on Internal SSD (C:\)

Create the main project directory on your internal SSD:

```powershell
# Create project directory
mkdir C:\projects\vibe_coding_puppet
cd C:\projects\vibe_coding_puppet

# Clone or initialize the project
# If you have a git repo:
git clone <repo-url> .

# Or copy from Manus sandbox:
# Copy all files from /home/ubuntu/vibe_coding_puppet to C:\projects\vibe_coding_puppet
```

---

### 1.4 Install Dependencies

Navigate to the project and install dependencies:

```powershell
cd C:\projects\vibe_coding_puppet

# Install npm packages
npm install
# or with pnpm
pnpm install

# Verify installation
npm list react react-dom tailwindcss
```

**Expected Output:**
```
vibe_coding_puppet@1.0.0
├── react@19.0.0
├── react-dom@19.0.0
├── tailwindcss@4.1.14
└── [other dependencies...]
```

---

## SECTION 2: CONFIGURATION FILES

*(Full instructions continue in the file — see the repository docs for complete content.)