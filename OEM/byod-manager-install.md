# XOGO Manager OEM Package Installation for BYOD Customers

1. Create a folder on your root drive (C:) named XOGO.
2. Download the latest [XOGO Manager OEM package](https://xogoarchive.blob.core.windows.net/manager-oem-packages/XOGO.Mobile.UWP_2.0.33.0_x86_x64_ARM_bundle.appxupload_Windows10_PreinstallKit.zip?sv=2019-12-12&st=2021-01-07T19%3A57%3A37Z&se=2021-01-08T19%3A57%3A37Z&sr=b&sp=r&sig=kdojSUzEHRLYofYJgGwFD%2FAMBkkfYf8usggSJJhAZRo%3D) to the Downloads folder on your computer.
3. Extract the zip file, open it, and then copy its contents (not the file itself) over to the C:/XOGO folder that you created.
4. Type CMD in the Windows search bar to open Command Prompt. Click the "Run as Administrator" option that shows up on the right side. 

![](admin-command-prompt.jpg)

5. Copy and paste the command below and hit enter to install the application. 

    **[x64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb.appxbundle /licensepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_x64__8wekyb3d8bbwe.appx

    **[x86]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb.appxbundle /licensepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_x86__8wekyb3d8bbwe.appx
    
    **[arm]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb.appxbundle /licensepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_arm__8wekyb3d8bbwe.appx
    
    **[arm64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb.appxbundle /licensepath:C:\Xogo\553becbaf4574bd0a0370f759028fefb_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.29231.0_arm64__8wekyb3d8bbwe.appx

6. You are done!
