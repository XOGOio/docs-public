# XOGO Player for Windows OEM Package Installation for BYOD Customers

1. Create a folder on your root drive (C:) named XOGO.
2. Download the latest [XOGO Player OEM package](https://xogoarchive.blob.core.windows.net/player-oem-packages/XOGO.Signage.UWP_2.0.42.0_x86_x64_ARM_bundle.appxupload_Windows10_PreinstallKit.zip) to the Downloads folder on your computer.
3. Extract the zip file, open it, and then copy its contents over to the C:/XOGO folder that you created.
![image](https://user-images.githubusercontent.com/43625896/156653082-3c76e690-c768-4d7c-8e0f-d5b05e70953e.png)
5. Type CMD in the Windows search bar to open Command Prompt. Click the "Run as Administrator" option that shows up on the right side. 

![](admin-command-prompt.jpg)

5. Copy and paste the command below and hit enter to install the application. 

    **[x64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043.appxbundle /licensepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.30704.0_x64__8wekyb3d8bbwe.appx

    **[x86]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043.appxbundle /licensepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.30704.0_x86__8wekyb3d8bbwe.appx
    
    **[arm]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043.appxbundle /licensepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.30704.0_arm__8wekyb3d8bbwe.appx
    
    **[arm64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043.appxbundle /licensepath:C:\Xogo\3f7e50dc323a43529a431e87aadcd043_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.30704.0_arm64__8wekyb3d8bbwe.appx

6. Download "[Embedded Mode Package](https://xogoarchive.blob.core.windows.net/player-provisioning-packages/AllowEmbeddedMode.ppkg)".

7. Run the Embedded Mode Package. Note: If this package doesn't work for your OS you may need to create your own: https://docs.microsoft.com/en-us/windows/iot/iot-enterprise/os-features/embedded-mode

8. Setup Kiosk Mode wizard (Assigned Access) to create a special user account, select XOGO Player as the Kiosk app and enable auto-login.

9. You are done!
