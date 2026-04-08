💿 Win11maker



Win11maker is a PowerShell script designed to create customized, debloated Windows 11 installation ISO. It automatically applies modifications to bypass hardware requirements, disable telemetry, and remove unwanted pre-installed applications, providing you with a clean and optimized Windows 11 experience.



✨ Features



Hardware Bypass: Automatically bypasses Windows 11 system requirements.



Debloating: Removes pre-installed sponsored apps, telemetry, Microsoft Teams, Copilot, Chat, and other unnecessary applications/services.



Privacy Improvements: Disables various telemetry and data collection services, Windows Consumer Features, and more.



Automated ISO Creation: Modifies your existing "install.wim" or "install.esd", cleans it up, and compiles a ready-to-use "win11.iso".



Automatic WIM Optimization: Restores the original WIM metadata, cleans up components, and compresses the result for an optimal image size.



🛠️ Requirements



Operating System: Windows 10 or Windows 11



Permissions: Administrator privileges.



Source Media: A valid Windows 11 installation media.



Free Space: Sufficient free space on your scratch disk to extract, mount, and reconstruct the Windows image.



📥 Usage



1. Clone or download this repository to your local machine.
2. Ensure you have your Windows 11 ISO mounted or installation USB inserted.
3. Run the PowerShell script as Administrator.
4. The script will prompt you for the drive letter of the Windows 11 installation media.
5. Follow the on-screen instructions. The script will extract, mount, debloat, and rebuild the ISO unattended.
6. Once completed, a customized "win11.iso" file will be generated in the same directory as the script.



⚙️ Customization



The "bypass" folder contains specific files necessary for bypassing system checks. You can add custom OEM scripts into the "bypass$oem$" folder if you wish to apply additional configurations during the Windows installation.



⚠️ Disclaimer



This script modifies the installation media of a Windows operating system. It bypasses security and compatibility checks put in place by Microsoft. Use this tool at your own risk. The developer is not responsible for any damage, data loss, or issues that arise from using this modified ISO.



📄 License



This project is licensed under the MIT License.

