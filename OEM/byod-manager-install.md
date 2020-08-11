# XOGO Manager OEM Package Installation for BYOD Customers

1. Create a folder on your root drive (C:) named XOGO.
2. Download the latest [XOGO Manager OEM package](https://xogoarchive.blob.core.windows.net/manager-oem-packages/XOGO.Mobile.UWP_2.0.25.0_x86_x64_ARM_bundle.appxupload_Windows10_PreinstallKit.zip?st=2020-03-18T14%3A25%3A00Z&se=2021-03-20T14%3A25%3A00Z&sp=r&sv=2018-03-28&sr=b&sig=IDNwHZd0OIe%2F7C150w6bKkT%2FD27zEhTAyk%2FK5sj2XmE%3D) to the folder you created.
3. Type CMD in the Windows search bar to open Command Prompt. Click the "Run as Administrator" option that shows up on the right side. 

![](admin-command-prompt.jpg)

4. Copy and paste the command below and hit enter to install the application. 

    **[x64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b.appxbundle /licensepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_x64__8wekyb3d8bbwe.appx

    **[x86]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b.appxbundle /licensepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_x86__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_x86__8wekyb3d8bbwe.appx
    
    **[arm]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b.appxbundle /licensepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_arm__8wekyb3d8bbwe.appx
    
    **[arm64]**  
    dism /online /Add-ProvisionedAppxPackage /packagepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b.appxbundle /licensepath:C:\Xogo\4a91c2c881534c58b1f3cd8ca2947a3b_License1.xml /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Framework.2.1_2.1.27427.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.NET.Native.Runtime.2.1_2.1.26424.0_arm64__8wekyb3d8bbwe.appx /DependencyPackagePath:C:\Xogo\Microsoft.VCLibs.140.00_14.0.27810.0_arm64__8wekyb3d8bbwe.appx

5. You are done!
