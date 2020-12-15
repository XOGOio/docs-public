# XOGO Player for Windows OEM Package Installation for BYOD Customers

1. Create a folder on your root drive (C:) named XOGO.
2. Download the latest [XOGO Player OEM package](https://xogoarchive.blob.core.windows.net/player-oem-packages/XOGO.Signage.UWP_2.0.24.0_x86_x64_ARM_bundle.appxupload_Windows10_PreinstallKit.zip?st=2020-03-18T14%3A30%3A00Z&se=2021-03-20T14%3A30%3A00Z&sp=r&sv=2018-03-28&sr=b&sig=zVsWMRSPwx8gnEnK7Qm6FZ5GdmzIcKweWOQgJd716So%3D) to the Downloads folder on your computer.
3. Extract the zip file, open it, and then copy its contents (not the file itself) over to the C:/XOGO folder that you created.
4. Type CMD in the Windows search bar to open Command Prompt. Click the "Run as Administrator" option that shows up on the right side. 

![](admin-command-prompt.jpg)

5. Copy and paste the command below and hit enter to install the application. 

    **[x64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a.appxbundle /licensepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_x64__8wekyb3d8bbwe.appx

    **[x86]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a.appxbundle /licensepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_x86__8wekyb3d8bbwe.appx
    
    **[arm]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a.appxbundle /licensepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_arm__8wekyb3d8bbwe.appx
    
    **[arm64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a.appxbundle /licensepath:C:\Xogo\8bf3bc4bd2d443a1b83b4638889d455a_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_arm64__8wekyb3d8bbwe.appx

6. Download "[Embedded Mode Package](https://xogoarchive.blob.core.windows.net/player-provisioning-packages/AllowEmbeddedMode.ppkg?st=2020-01-12T14%3A02%3A00Z&se=2021-01-14T14%3A02%3A00Z&sp=r&sv=2018-03-28&sr=b&sig=IU%2B0telOxY%2F2MRYhn3AjKPXA42oGEcjhMR0YqZVOmzM%3D)".

7. Run the Embedded Mode Package and complete installation.

8. Optionall setup Assigned Access for your player device following instructions [here](https://www.windowscentral.com/how-set-assigned-access-windows-10).

9. If you have Assigned Access setup, configure your device to auto-login with its default user by following instructions [here](https://www.tekrevue.com/tip/skip-windows-10-login-screen/ ).

10. You are done!
