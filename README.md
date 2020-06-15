# SplashTest
Add a splash screen, instead of the default splash.

Currently, the default splash still exists before the extended splash.
See:
![](https://github.com/hupo376787/SplashTest/blob/master/000.gif)

# ===============================Update===============================

Finally I found the solution.

Open `Package.appxmanifest` in txt mode, add `xmlns:uap5="http://schemas.microsoft.com/appx/manifest/uap/windows10/5"` to top of file, and update `IgnorableNamespaces="uap uap5 mp genTemplate"`.

The in `SplashScreen` area, update `<uap:SplashScreen uap5:Optional="true" Image="Assets\SplashScreen.png" />`.

Done!

See

![](https://github.com/hupo376787/SplashTest/blob/master/000.gif)
