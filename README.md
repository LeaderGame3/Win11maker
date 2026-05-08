💿 Win11maker



Win11maker is a PowerShell script designed to create customized, debloated Windows 11 installation media. It automatically applies modifications to bypass hardware requirements, disable telemetry, and remove unwanted pre-installed applications, providing you with a clean and optimized Windows 11 experience.



✨ Features



User-Friendly GUI: A modern, dark-themed, and bilingual (English/French) graphical interface for easy configuration.



Hardware Bypass: Automatically bypasses Windows 11 system requirements.



Debloating: Removes pre-installed sponsored apps, telemetry, Microsoft Teams, Copilot, Chat, and other unnecessary applications/services.



Privacy Improvements: Disables various telemetry and data collection services, Windows Consumer Features, and more.



Software Pre-installation: Integrates Winget search directly into the GUI to select and automatically install your favorite applications during the first setup.



Unattended Setup: Generates a custom autounattend.xml file to automate the out-of-box experience, creating a local admin account without requiring a Microsoft account.



Automated ISO or USB Creation: Modifies your existing "install.wim" or "install.esd", cleans it up, and compiles a ready-to-use "win11.iso" or a Bootable USB Flash Drive.



Automatic WIM Optimization: Restores the original WIM metadata, cleans up components, and compresses the result for an optimal image size.



Driver Injection: Automatically injects custom drivers into both the Windows image and the boot environment.



ESD to WIM Conversion: Automatically converts install.esd to install.wim if necessary.



🛠️ Requirements



Operating System: Windows 10 or Windows 11



Permissions: Administrator privileges.



Source Media: A valid Windows 11 installation media.



Free Space: Sufficient free space on your scratch disk to extract, mount, and reconstruct the Windows image (minimum 20 GB required).



📥 Usage



1. Clone or download this repository to your local machine.
2. Ensure you have your Windows 11 ISO mounted or installation USB inserted.
3. Run the PowerShell script or the .exe file as Administrator.
4. A graphical interface will launch. Select your language, source drive, output format, USB settings (if applicable), and desired modifications.
5. Click "Start Creation" to begin the process. The tool will automatically extract, mount, debloat, and rebuild the image.
6. Once completed, your customized "win11.iso" file or Bootable USB will be ready to use.



⚙️ Customization



The "bypass" folder contains specific files necessary for bypassing system checks.



The "drivers" folder contains two subfolders: "install" and "boot". Drivers placed in the "install" folder will be injected into the Windows image, while those in the "boot" folder will be integrated into the boot environment.



Important note for drivers: To avoid file conflicts, do not place all your driver files directly in the root of these folders. Instead, create a separate subfolder for each driver package. The script will automatically scan all subfolders and inject them correctly.



⚠️ Disclaimer



This script modifies the installation media of a Windows operating system. It bypasses security and compatibility checks put in place by Microsoft. Use this tool at your own risk. The developer is not responsible for any damage, data loss, or issues that arise from using this modified ISO or USB.



📄 License



This project is licensed under the MIT License.

