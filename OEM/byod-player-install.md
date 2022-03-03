# XOGO Player for Windows OEM Package Installation for BYOD Customers

1. Create a folder on your root drive (C:) named XOGO.
2. Download the latest [XOGO Player OEM package](https://xogoarchive.blob.core.windows.net/player-oem-packages/XOGO.Signage.UWP_2.0.33.0_x86_x64_ARM_bundle.appxupload_Windows10_PreinstallKit.zip?sv=2019-12-12&st=2021-01-12T20%3A01%3A37Z&se=2022-12-10T20%3A01%3A00Z&sr=b&sp=r&sig=ko%2FOf0sXqwLRdMRKPse7j5urfI07ChDzNjXVd2t4MGE%3D) to the Downloads folder on your computer.
3. Extract the zip file, open it, and then copy its contents over to the C:/XOGO folder that you created.
![image](https://user-images.githubusercontent.com/43625896/156653082-3c76e690-c768-4d7c-8e0f-d5b05e70953e.png)
5. Type CMD in the Windows search bar to open Command Prompt. Click the "Run as Administrator" option that shows up on the right side. 

![](admin-command-prompt.jpg)

5. Copy and paste the command below and hit enter to install the application. 

    **[x64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\a3433df2069a422e8673db817658b0b3.appxbundle /licensepath:C:\Xogo\a3433df2069a422e8673db817658b0b3_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_x64__8wekyb3d8bbwe.appx

    **[x86]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\a3433df2069a422e8673db817658b0b3.appxbundle /licensepath:C:\Xogo\a3433df2069a422e8673db817658b0b3_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_x86__8wekyb3d8bbwe.appx
    
    **[arm]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\a3433df2069a422e8673db817658b0b3.appxbundle /licensepath:C:\Xogo\a3433df2069a422e8673db817658b0b3_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_arm__8wekyb3d8bbwe.appx
    
    **[arm64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\a3433df2069a422e8673db817658b0b3.appxbundle /licensepath:C:\Xogo\a3433df2069a422e8673db817658b0b3_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_arm64__8wekyb3d8bbwe.appx

6. Download "[Embedded Mode Package](https://xogoarchive.blob.core.windows.net/player-provisioning-packages/AllowEmbeddedMode.ppkg)".

7. Run the Embedded Mode Package and complete installation.

8. Optional setup Assigned Access for your player device following instructions [here](https://www.windowscentral.com/how-set-assigned-access-windows-10).

9. If you have Assigned Access setup, configure your device to auto-login with its default user by following instructions [here](https://www.tekrevue.com/tip/skip-windows-10-login-screen/ ).

10. You are done!
