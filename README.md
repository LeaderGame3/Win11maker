💿 Win11maker



Win11maker is a PowerShell script designed to create customized, debloated Windows 11 installation media. It automatically applies modifications to bypass hardware requirements, disable telemetry, and remove unwanted pre-installed applications, providing you with a clean and optimized Windows 11 experience.



✨ Features



Hardware Bypass: Automatically bypasses Windows 11 system requirements.



Debloating: Removes pre-installed sponsored apps, telemetry, Microsoft Teams, Copilot, Chat, and other unnecessary applications/services.



Privacy Improvements: Disables various telemetry and data collection services, Windows Consumer Features, and more.



Automated ISO or USB Creation: Modifies your existing "install.wim" or "install.esd", cleans it up, and compiles a ready-to-use "win11.iso" or a Bootable USB Flash Drive.



Automatic WIM Optimization: Restores the original WIM metadata, cleans up components, and compresses the result for an optimal image size.



Driver Injection: Automatically injects custom drivers into both the Windows image ("drivers\\install") and the boot environment ("drivers\\boot").



ESD to WIM Conversion: Automatically converts install.esd to install.wim if necessary.



🛠️ Requirements



Operating System: Windows 10 or Windows 11



Permissions: Administrator privileges.



Source Media: A valid Windows 11 installation media.



Free Space: Sufficient free space on your scratch disk to extract, mount, and reconstruct the Windows image (minimum 20 GB required).



📥 Usage



1. Clone or download this repository to your local machine.
2. Ensure you have your Windows 11 ISO mounted or installation USB inserted.
3. Run the PowerShell script as Administrator.
4. The script will prompt you for the drive letter of the Windows 11 installation media.
5. Follow the on-screen instructions. The script will prompt you to choose the output format (ISO or USB) and will extract, mount, debloat, and rebuild the image.
6. Once completed, your customized "win11.iso" file or Bootable USB will be ready to use.



⚙️ Customization



The "bypass" folder contains specific files necessary for bypassing system checks. You can add custom OEM scripts into the "bypass$OEM$" folder if you wish to apply additional configurations during the Windows installation.



The "drivers" folder contains two subfolders: "install" and "boot". Drivers placed in the "install" folder will be injected into the Windows image, while those in the "boot" folder will be integrated into the boot environment (boot.wim).



⚠️ Disclaimer



This script modifies the installation media of a Windows operating system. It bypasses security and compatibility checks put in place by Microsoft. Use this tool at your own risk. The developer is not responsible for any damage, data loss, or issues that arise from using this modified ISO or USB.



📄 License



This project is licensed under the MIT License.

