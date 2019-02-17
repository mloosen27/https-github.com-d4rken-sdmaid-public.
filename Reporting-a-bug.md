# How to report a bug?

While it would be the perfect bug report if you follow all of the following steps you can start with basic information and still add more at a later point or on request.
**A bug report missing a few details is better than no bug report at all.**

## Step 1 - Known issues
Some bugs or issues might already be known, to check that visit the [issue tracker](https://github.com/d4rken/sdmaid-public/issues). Check [current and recently closed issues](https://github.com/d4rken/sdmaid-public/issues?utf8=%E2%9C%93&q=is%3Aissue). If you find a similar issue post a comment under it, otherwise make a new issue. 

## Step 2 - Basics
Gather basic information about your setup, which includes
* What kind of device you have (e.g. Nexus 5)
* What kind of Android version and or custom ROM it's running (e.g. latest stock Android 6.0.1)
* If your device is rooted or unrooted (e.g. Rooted with SuperSU v2.67)
* What version of SD Maid and (if applicable) SD Maid Pro you were running (e.g. SD Maid v4.1.0, Unlocker v4.0.2)
* Long press the settings menu entry, which will open the debug menu. At the top of the page is your install-id tap it to copy it and attach it to your bug report. This way I will be able to check for automatic crash reports from your device.

Good, now we have a baseline for what kind of device setup you have. Now add a little description describing your issue:
* What happened?
* What did you expect to happen?
* What actions did you take?
* Can you reproduce it, i.e. does this happen everytime?

## Step 3 - Advanced report
**The following instructions are valid for SD Maid v4.2.6+.**
### Crash report
If SD Maid crashed I should have gotten an automatic crash report (unless you turned that off, but why would you...). To find this crash report on my server I need to identify your SD Maid installation. This happen through a UUID which is a unique and anonymous identifier SD Maid generates on it's first start. You can find it by going into the Overview section and expanding the box containing SD Maids version information or by long pressing the settings menu entry. Tap it to copy it to your clipboard and add it to your issue ticket.

### **Debugrun log**
**The following instructions are valid for SD Maid v4.13.2+.**

The best thing you can provide to help fix an issue is a debug log of the problem manifesting. A debug log is a very detailed description of everything SD Maid did. Note that the file may private information in form of file names and pathes on your device.

#### If you can still open SD Maid
1. Open SD Maid, long press Settings to reveal the hidden debug menu and click `RECORD DEBUG LOG`.
2. A new notification will show and indicate that it's recording.
3. Now reproduce the behavior you want to debug. You can reboot the device, as well as kill and restart SD Maid, the recording will automatically resume when SD Maid's process is launched by any means. 
4. Once you are done, stop the recording via the notification. A window will popup and allow you to share the recorded file.

#### If SD Maid is not accessible
1. Force stop SD Maid.
2. Create the file `<sdcard>/Android/data/eu.thedarken.sdm/files/sdm_force_debug_run`
3. Launch SD Maid by any means, the core process will be loaded in any case which will also consume the created file and start a recording. A visible notification will indicate the on-going recording.
4. If parts of SD Maids UI are still responsive then you can finish like in the above. If SD Maid's UI including the log-sharing is inaccessible then you can directly pull the file from `<sdcard>/Android/data/eu.thedarken.sdm/cache/logfiles`

We can't pick an easier path for this as this is the only path SD Maid can write to it without any extra permissions or requirements, thus we can use the debugrun to troubleshoot permission issues too :wink:.

[[[ https://cloud.githubusercontent.com/assets/1439229/16135841/8977d1e0-3426-11e6-8d1c-e9daac0cc980.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/16135841/8977d1e0-3426-11e6-8d1c-e9daac0cc980.png)
[[[ https://user-images.githubusercontent.com/1439229/52920602-a0180c00-330e-11e9-855f-5e892abbde2f.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/52920602-a0180c00-330e-11e9-855f-5e892abbde2f.png)
[[[ https://user-images.githubusercontent.com/1439229/52920603-a8704700-330e-11e9-988b-ed1feb52608f.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/52920603-a8704700-330e-11e9-988b-ed1feb52608f.png)
[[[ https://user-images.githubusercontent.com/1439229/52920607-b58d3600-330e-11e9-8b93-008720ffe548.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/52920607-b58d3600-330e-11e9-8b93-008720ffe548.png)