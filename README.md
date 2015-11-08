# About
自己修改的安卓系统桌面，基于Launcher3源码。     

# Links
https://android.googlesource.com/platform/packages/apps/Launcher3     
https://github.com/fookwood/Launcher3    
https://github.com/krajeswaran/LeanLauncher   
https://github.com/yuxinburen/Launcher3_1   

###解决不能安装的问题
解决可能因为相同权限声明或内容提供者冲突而不能安装的问题，需要重构包名为非com.android.launcher3，并改动所有com.android.launcher3的引用，如：ProviderConfig.AUTHORITY、AndroidManifest.xml中的permission相关及provider的authorities属性等；   

###改屏幕方向
AndroidManifest.xml的入口activity加入android:screenOrientation="landscape"；   

###隐藏Hotseat的显示所有应用的按钮
LauncherAppState.isDisableAllApps()返回true；   

