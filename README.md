# 💾 How to Use hackinOS RDR & IMG Files to Install macOS  
### Applicable for All macOS Versions — **High Sierra → Tahoe**

hackinOS provides two types of installation files for all macOS versions:

- **📀 RDR File (.rdr)** → Restore macOS directly onto your drive using **R-Drive Image**  
- **💿 IMG/DMG File (.img / .dmg)** → Create a bootable USB installer using **balenaEtcher**

Both methods work for every macOS version from **High Sierra, Mojave, Catalina, Big Sur, Monterey, Ventura, Sonoma, Sequoia, to Tahoe**.

> **Download Password:** www.hackinOS.com

# 📀 PART 1 — Installing macOS Using the RDR File  
*(Restore directly to your disk — no USB required)*

# 🔗 macOS Download Links (RDR & IMG/DMG)
Below is the section where you can insert download links for each macOS version.

## 📀 RDR Downloads  
(Click to download the ready-to-restore `.rdr` image)

- **macOS High Sierra RDR** — *Add link here*  
- **macOS Mojave RDR** — *[Mojave](https://hackinos.com/files/file/14-hackinos-mojave-restore/)*  
- **macOS Catalina RDR** — *Add link here*  
- **macOS Big Sur RDR** — *[Big Sur](https://hackinos.com/files/file/9-hackinos-big-sur-restore/)*  
- **macOS Monterey RDR** — *[Monterey](https://hackinos.com/files/file/10-hackinos-monterey-restore/)*  
- **macOS Ventura RDR** — *[Ventura](https://hackinos.com/files/file/11-hackinos-ventura-restore/)*  
- **macOS Sonoma RDR** — *Add link here*  
- **macOS Sequoia RDR** — *[Sequoia](https://hackinos.com/files/file/12-hackinos-sequoia-restore/)*  
- **macOS Tahoe RDR** — *[Tahoe](https://hackinos.com/files/file/13-hackinos-tahoe-restore/)*  

## 💿 IMG/DMG USB Installer Downloads  
(Click to download the `.img` or `.dmg` installer image)

- **macOS High Sierra IMG/DMG** — *[High Sierra](https://hackinos.com/files/file/3-hackinos-high-sierra/)*  
- **macOS Mojave IMG/DMG** — *[Mojave](https://hackinos.com/files/file/4-hackinos-mojave/)*  
- **macOS Catalina IMG/DMG** — *[Catalina](https://hackinos.com/files/file/2-hackinos-catalina/)*  
- **macOS Big Sur IMG/DMG** — *[Big Sur](https://hackinos.com/files/file/1-hackinos-big-sur/)*  
- **macOS Monterey IMG/DMG** — *[Monterey](https://hackinos.com/files/file/5-hackinos-monterey/)*  
- **macOS Ventura IMG/DMG** — *[Ventura](https://hackinos.com/files/file/6-hackinos-ventura/)*  
- **macOS Sonoma IMG/DMG** — *[Sonoma](https://hackinos.com/files/file/7-hackinos-sonoma/)*  
- **macOS Sequoia IMG/DMG** — *[Sequoia](https://hackinos.com/files/file/8-hackinos-sequoia/)*  
- **macOS Tahoe IMG/DMG** — *Add link here*  

## 💡 What Is the RDR File?
The `.rdr` file is a ready-to-restore macOS disk image.  
Once restored, your drive will contain:

- A full macOS installation  
- A preconfigured EFI folder 🧩  
- Bootable immediately 🎉  

However, you **must adjust the EFI** to match your hardware for proper functionality.

## 🛠️ Steps to Restore macOS with R-Drive Image

### 1️⃣ ⬇️ Download the macOS `.rdr` file  
Select the version you want (High Sierra → Tahoe).

### 2️⃣ 🔌 Connect the target drive  
- Choose the HDD/SSD/NVMe where macOS will be installed.  
- ⚠️ **This process erases the entire drive. Be sure to back up your data.**

### 3️⃣ 🚀 Open **R-Drive Image** in Windows  
Launch the software.

### 4️⃣ Start the Restore Process  
Inside R-Drive:

1. Click **“Restore Image”** 📂  
2. Select the `.rdr` file  
3. Select your target drive 💽  
4. Click **Start ⚡**

### 5️⃣ ⏳ Wait for the restore to finish  
When completed, the drive is fully bootable with macOS. 🎉

## 📌 Important Notes About EFI
The restored image includes a prebuilt EFI folder 🧩.  
However, every Hackintosh system requires **hardware-specific configuration**.

After restoring, mount the EFI partition to:

- 🧬 Update OpenCore  
- 📦 Add or replace required kexts  
- 📝 Edit `config.plist` (ProperTree or OCC)  
- ⚙️ Adjust GPU settings, ACPI patches, USB mapping, SecureBootModel, etc.

# 💿 PART 2 — Creating a macOS USB Installer Using IMG/DMG  
*(Use balenaEtcher to flash the image to a USB drive)*

## 💡 What Is the IMG/DMG Installer File?
The `.img/.dmg` file is a ready-made macOS USB installer.  
Flash → Plug → Boot.  
An EFI folder is included, but you still need to **customize it** for your system.

## 🛠️ Steps to Create a macOS USB Installer (IMG/DMG)

### 1️⃣ ⬇️ Download the macOS `.img` or `.dmg` file  
Available for all versions from High Sierra → Tahoe.

### 2️⃣ 🔌 Insert a USB drive  
- Minimum: **16GB**  
- Recommended: **32GB** for stable performance

### 3️⃣ 🚀 Launch **balenaEtcher**  
Download the latest version if you don’t have it.

### 4️⃣ Flash the Installer  
Inside Etcher:

1. Click **“Flash from file”** 📂 → select the `.img/.dmg`  
2. Click **“Select target”** 💽 → choose your USB  
3. Click **“Flash”** ⚡

### 5️⃣ ⏳ Wait for flashing + verification  
Once complete, your USB is ready to boot macOS. 🎉

## 📌 Important Notes About EFI (USB Installer)
The USB includes an EFI folder 🧩, but you must tailor it to match your hardware:

- CPU (Intel or AMD)  
- GPU (Intel, AMD, NVIDIA Kepler)  
- Chipset / motherboard  
- Wi-Fi / Bluetooth  
- SSD/NVMe  
- ACPI / Trackpad requirements  

After flashing:

- 🧬 Update OpenCore  
- 📦 Add necessary kexts  
- 📝 Edit `config.plist`  
- ⚙️ Check USB mapping, NVRAM settings, Secure Boot Model, GPU patches, etc.

# 🎯 Which Method Should You Use?

| Use Case | Recommended Method |
|---------|--------------------|
| Want the fastest installation, no USB needed | **RDR Restore** |
| Want a clean, traditional macOS installation | **USB Installer (IMG/DMG)** |
| System fails to boot after restore | Use **USB Installer** to repair |
| Installing on multiple machines | **USB Installer** |

# ✅ Final Notes
You can use **both RDR and IMG/DMG methods** for any macOS version from **High Sierra up to Tahoe**.  
Both formats are preconfigured, easy to use, and optimized for Hackintosh users.
