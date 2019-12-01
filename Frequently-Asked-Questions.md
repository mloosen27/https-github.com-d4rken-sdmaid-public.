# FAQ
* [General](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#general)
  * [I just want to clean my device, what to do?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#i-just-want-to-clean-my-device-what-to-do)
  * [Why should I use SD Maid?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#why-should-i-use-sd-maid)
  * [Does SD Maid only work on sdcards?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#does-sd-maid-only-work-on-sdcards)
  * [Recover deleted files](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#recover-deleted-files)
  * [Hanging](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#hanging)
  * [SD Maid v2/v3/v4](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#sd-maid-v2v3v4)
  * [Screen overlay detected](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#screen-overlay-detected)
* [SD Maid Pro](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#sd-maid-pro)
  * [Free vs Pro Version](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#free-vs-pro-version)
  * [What is the difference between the purchase options?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#what-is-the-difference-between-the-purchase-options)
  * [Factory-Reset / Device-Change](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#factory-reset--device-change)
  * [Google Play is not showing the purchase](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#google-play-is-not-showing-the-purchase)
  * [Unlocker update required](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#Unlocker-update-required)
  * [SD Maid is not enabling the pro features](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#sd-maid-is-not-enabling-the-pro-features)
  * [I can't find SD Maid Pro on my device](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#i-cant-find-sd-maid-pro-on-my-device)
  * [Hiding the unlocker app on Android 10](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#hiding-the-unlocker-app-on-android-10)

* [Root](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#root)
  * [What is root?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#what-is-root)
  * [Does SD Maid only work with root?](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#does-sd-maid-only-work-with-root)
  * [MobileIron](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#mobileiron)

## General
### I just want to clean my device, what to do?
* Install SD Maid, if you own [SD Maid Pro](https://play.google.com/store/apps/details?id=eu.thedarken.sdm.unlocker), then also install the Unlocker now.
* Start SD Maid, the app will open on the [Quickaccess](https://github.com/d4rken/sdmaid-public/wiki/QuickAccess) page.
* Press the green scan bar at the bottom of the screen.
* Because this is the first time you started SD Maid, you will be asked to complete the [setup](https://github.com/d4rken/sdmaid-public/wiki/Setup).
* After completing the setup, SD Maid will run the "scan" part of each tool.
* When the scan finishes you can press "execute" to delete/optimize, or press a specific tool to view more details.

#### How do I configure SD Maid?
SD Maid starts out with a default configuration that favors safety over thoroughness as every device is a little bit unique, just like you 😉.
Each tool has options that can be reached either through a menu entry in the toolbar, or the global settings screen which you can reach through the main navigation menu. The options either include or exclude specific file types or categories. If you'd like SD Maid to delete more/less then you can enable/disable additional filters and options. After enabling new options, perform a scan and check that SD Maid displays the desired results. Create an [exclusion](https://github.com/d4rken/sdmaid-public/wiki/Exclusions) to exclude specific apps or files from SD Maids results.

### Why should I use SD Maid?
**Because it's thorough and honest.**
If you want a broom, you look for the one that cleans best, any other purchase argument is secondary. SD Maid v0.1 was released on [29.03.2011](http://forum.xda-developers.com/showpost.php?p=12482608&postcount=1). Years of learning and more experience, constant improvements and adaption to every new Android kink, make SD Maid what is is today.
SD Maid is brutally honest, there will be no euphemisms to make your feel better after "cleaning" your device. No hidden agenda to pressure you into using the app itself. A tool to use when needed.

### Does SD Maid only work on sdcards?
**No.** SD Maid will consider any accessible storage in your device. Depending on what can be accessed, this includes internal storage, external storage and usb storage.

### Recover deleted files
If you accidentally deleted some files, you may be able to recover them. Restoring data depends on where the files were originally located and whether the space, that their deletion freed, has been occupied again.

Before attempting any recovery you should check if your files are actually missing. Almost everyone views their media files through gallery apps. What the gallery apps shows can be affected by SD Maid (e.g. deleted thumbnails). Use a file explorer and check if the files you are missing are actually gone. Check folders such as `DCIM` and `Pictures` on your internal and external storage. To fix the gallery app you can use SD Maids Explorer option "Force media scan", try a reboot, attach and detach from a computer or just wait a bit until the system does a media scan on it's own.

#### Removable storage
Your best chance to restore files that were deleted from a removeable sdcard (e.g. `/storage/sdcard1`) is to plug the sdcard (or the device) into a desktop computer and run software from there.

Recovery software:
* http://www.cgsecurity.org/wiki/PhotoRec
* https://www.piriform.com/recuva

#### Internal storage
Recovering files from internal storage requires a rooted device, e.g. internal sdcard (`/storage/emulated/0`) or private storage (`/data/data`). Root is required because recovery apps need to directly access the underlying storage device.

Recovery apps:
* https://play.google.com/store/apps/details?id=fahrbot.apps.undelete
* https://play.google.com/store/apps/details?id=com.defianttech.diskdigger

### Hanging
#### "In queue"
The first time you run any action in a new session, SD Maid will have to make some preparations (check file consistency, check permissions etc). You will see the progress state "In queue" because your task is queued behind the preparations/setup task. In almost all cases where SD Maid seems to hang here it's related to the root check.

At some point SD Maid checks if your device is rooted. This is done by basically just asking for root access and waiting for an answer. Usually there should just be an error or a "no" if the device is not rooted or the root request was declined. If there is no answer at all though then SD Maid waits until a timer runs out, this is what happens when it "hangs".

To test if this is the issue you are seeing, long press the settings entry to enter the debug menu, enable the option `Disable root check`, kill and restart SD Maid. If it now works as expected then there is an issue with your root setup. In many cases this is just a small glitch with the superuser management app. Remove SD Maid from superuser app, reboot your device and try again.

Known causes & solutions:
* Incomplete root attempt. Reroot your device.
* Incomplete unroot attempt. Reroot your device, then unroot it correctly.
* You just updated SD Maid and your super user app did not handle this correctly. Try removing SD Maid from the list apps in the super user app. Reboot your device and let SD Maid request root again. If that doesn't help uninstall SD Maid, remove it from the super user app, reboot your device and reinstall SD Maid. If that doesn't help either, clear the super user apps data and reboot.
* Sometimes the ROMs are delivered with incomplete root from the manufactor. Either root it or disable the root check in SD Maid.
* Shortly after reboots the super-user app may take too long to respond due to too much going. Wait a bit and retry.

#### During execution
Sometimes it may look like SD Maid is hanging during a task. Make sure to wait at least 15 minutes before assuming there is an issue (and contacting me 😁 ). If you have many files, huge duplicate files or large databases it is possible for SD Maid to take up to half an hour to complete operations. You can put your phone away while waiting.

A common cause for huge slowdowns, i.e. SD Maid seeming "stuck", are faulty sdcards. If the sdcard is damaged and/or the filesystem is corrupted the I/O performance drops drastically. To confirm this, remove the sdcard and try again. If your sdcard is faulty I would strongly advise to backup all your data from it. In some cases formating "seems" to fix the sdcard again but I would recommand to not risk it and just replace it.

### SD Maid v2/v3/v4
There are different versions available of SD Maid. Every few years SD Maid was completely overhauled to improve it through gained experience and to adopt to new Android environments. During these overhauls the minimum required Android version is usually raised due reduce workload, maintaining compatibility "hacks" for very old Android versions is usually not feasible when supporting the newest Android versions.

It's possibly that newer versions seem slower but downgrading because of that is bad trade, you would gain speed but pay with thoroughness and safety. Searching through more and doing additional checks just costs time. Never versions may show less items to delete, not because they are worse, but because for specific reasons it is no longer considered good to remove these files. The goal is not to delete the most files, but the right files. Every change has a good reason.

In short: **Use the latest version of SD Maid available for your device.**

* SD Maid v2 was the main app version from 2012Q2 to 2013Q1. Its target is Android 2.1 to 2.2.
* SD Maid v3 was the main app version from 2013Q1 to 2016Q1. Its target is Android 2.3 to 4.0.
* SD Maid v4 is the main app version since 2016Q1. Its target version is Android 4.1+.

### Screen overlay detected
The warning "Screen overlay detected" is a popup dialog you may see when trying to grant app permissions on an Android 6.0+ device. This is a security feature (from Android, not SD Maid) which prevents you from granting any permissions while an app is active that can draw on the screen, because malicious apps could alter the text of the permission dialog. The warning is not SD Maid specific and it's not SD Maid using the a screen overlay, but another application on your device.

Solution:
* Open settings
* Disable the overlay permissions for all listed apps
* Grant SD Maid (or any other app) it's permission
* Enable the overlay permissions again

[[[ https://cloud.githubusercontent.com/assets/1439229/19970701/1d9a9e9c-a1dd-11e6-8ed5-06fb81443707.jpg | height = 150px]]](https://cloud.githubusercontent.com/assets/1439229/19970701/1d9a9e9c-a1dd-11e6-8ed5-06fb81443707.jpg)

## SD Maid Pro
### Free vs Pro Version
The "Pro" version of SD Maid also called the "Unlocker" is a plugin, it's not a standalone application.
You should install it toegether with the free version of SD Maid and then start the free version. It will detect the plugin and enable all extra features.

Current upgrades:
* User defined SystemCleaner filter
* Deletion function in the AppCleaner tool
* Deletion function in the Duplicates tool
* Scheduled operations via timer
* Scheduled reboots (power cycle or software restart)
* A widget to execute the main tools.
* File/app previews in all tools
* A searchable history of SD Maids actions
* Launcher shortcuts to specific tools
* Additional search options
* Android 7.1 app icon shortcuts
* (Forced) app moving to external storage on supported devices.
* Sleeping well, knowing the developer is motivated to keep developing :tada: 

### What is the difference between the purchase options?
All purchase options get you SD Maid Pro with all the same app features. The difference lies in how you access SD Maid Pro.

It's not possible to switch the purchase/unlock option without buying the upgrade again, some exceptions may apply.

#### [Unlocker app](https://play.google.com/store/apps/details?id=eu.thedarken.sdm.unlocker)
The unlocker app is the original way to unlock SD Maid. It was the first upgrade method available (~2011). It's an extra app that you buy and install.

* ✔️ Can be shared through [Google Play Family Library](https://support.google.com/googleplay/answer/7007852)
* ❗ You need Google Play to do the initial install and keep it updated.
* ❌ You need to have two apps installed.

#### [In-app purchase](https://play.google.com/store/apps/details?id=eu.thedarken.sdm)
The in-app purchase was added (late ~2019) due to Android 10 no longer allowing unlocker apps to hide themselves. You purchase the upgrade from inside the free version.

* ✔️ No extra app needs to be installed.
* ❗ Does not work without Google Play / Google Play Services. 
* ❌ In-app purchases can not be shared through [Google Play Family Library](https://support.google.com/googleplay/answer/7007852)

#### [apps.darken.eu](https://apps.darken.eu/)
This option was made available (early ~2019) so users without access to Google Play or the option to purchase something on Google Play can upgrade to SD Maid Pro.

* ✔️ Doesn't require an extra app to be installed.
* ✔️ Doesn't require Google Play or Google Play Services.
* ❌ Requires an extra account on my server.

### On how many devices can I use SD Maid?
#### Via Google Play
On as many devices as you like, if they all use the same Google account. If you are trying to install it to another device with the same account and it asks you to pay again, [see here](https://github.com/d4rken/sdmaid-public/wiki/Frequently-Asked-Questions#google-play-is-not-showing-the-purchase).

#### Via apps.darken.eu
There is currently a limit of 10 simultaneous devices. Once reached you have to remove older devices via the website. Exceptions are possible though, just send me a mail :wink:.

### Factory-Reset / Device-Change
This is not an SD Maid issue, but still a popular question. Apps purchased through Google Play are tied to your Google account, not your device. If you use the same Google account on a new or factory reset device, you will have access to all previous purchases.

### Unlocker update required
When upgrading to SD Maid Pro by using the unlocker app, the two apps should both be kept updated. If the unlocker app is too old SD Maid will display the setup process and ask you to upgrade. There will be an upgrade button that takes you to the [Google Play entry for the unlocker](https://play.google.com/store/apps/details?id=eu.thedarken.sdm.unlocker).

If the Google account you are currently signed into does not contain a purchase for the [unlocker app](https://play.google.com/store/apps/details?id=eu.thedarken.sdm.unlocker) then the Google Play app does not offer you the option to upgrade and only shows buttons for `Open` and `Remove`. This can happen when upgrading to a new device and/or switching Google accounts. You need to find and log into Google Play [with the right Google Account](https://pay.google.com/payments/u/0/home) and the update option will appear. If all else fails, mail me.

### Google Play is not showing the purchase
Apps are purchased per Google account, not per device. Switching devices doesn't mean you have to buy an app again. If Google Play is not showing your purchase, you are either not logged in with the account your purchased the application with or the Google Play app has not yet syncronized with your list of purchases. You can see your purchases [here](https://wallet.google.com/manage/#transactions:filter=ALL) or [here](https://play.google.com/apps). This is a Google Play issue and has no relation to SD Maid itself.

The following action are known to fix this:
* Force closing and reopening Google Play.
* Rebooting the device.
* Triggering the install from the [Google Play](https://play.google.com/store/apps/details?id=eu.thedarken.sdm.unlocker) website. 
* Using "Clear Data" on the Google Play app (`com.android.vending`).

Note:
If you uninstall an app shortly after purchasing it, Google Play automatically refunds your purchase. Currently the automatic refund window is [2 hours](https://support.google.com/googleplay/answer/2479637?hl=en). This is only happens once per app.

### SD Maid is not enabling the pro features
If the both SD Maid (`eu.thedarken.sdm`) and the SD Maid Pro plugin/unlocker (`eu.thedarken.sdm.unlocker`) are installed, SD Maid should enable all pro features. Detection of the SD Maid Pro happens on app launch and when closing/opening the UI.

Known solutions:
* Force close SD Maid or reboot the device and reopen SD Maid
* The system did not correctly install either SD Maid or the unlocker. Uninstall both apps, reboot your device, install the unlocker app first, then SD Maids free version.
* If either SD Maid or the unlocker has been modified the pro features will also not be unlocked. Ensure that you downloaded the apps from official sources (Google Play or [my server](https://sdmaid.darken.eu/download)) and that no app on your device modified them. There are some "security apps" that modify installed apps for questionable purporses.

### I can't find SD Maid Pro on my device
The SD Maid Pro plugin only has to be installed, but does not have to be actively launched. Due to this this the app contains an option that will hide its shortcut from your app drawer. To display the shortcut again, either uninstall and reinstall the app, or open SD Maids advanced settings which offers an option to do that.

### Hiding the unlocker app on Android 10
Google removed the ability for apps to hide themselves on Android 10+. Workarounds:

* Some launcher apps have features that allow you to hide apps yourself (e.g. Nova Launcher).
* On a computer, try [ADB](https://developer.android.com/studio/command-line/adb) with the command `adb shell pm disable eu.thedarken.sdm.unlocker`
* Upgrading to SD Maid Pro through In-App-Purchase or through https://apps.darken.eu

## Root
### What is root?
So what's this root everyone is talking about? Root is the name of a special user account on your device, a super user account with elevated privileges.
Normally you or apps can't use the account. The act of "rooting" changes that. It makes it accessible and adds a "superuser app" that manages access to the root account. There are pros and cons to rooting, which we don't need to cover here. Just google it, it's a common discussion on many blogs. Whether you root your device is up to you.

### Does SD Maid only work with root?
**No.** SD Maid will adjust its behavior to fit your device. 

SD Maid being able to use root is a bonus for people with rooted devices. It does not make SD Maid work worse on unrooted devices.

Some people are saying: If you have rooted device you should use SD Maid, but if your device is not rooted, choose a different application. That's wrong. All applications are bound by the same restrictions, how each app uses what it has available, is what makes the difference.
Choose a different app if you don't feel comfortable using SD Maid, if it is too complicated or you simply don't like it, but not because you don't have a rooted device.

Functions that don't work at all without root are usually those that modify other apps, such as freezing or disabling components or uninstalling system apps.

```
Imagine you buy an offroad vehicle, like a Jeep or a LandRover Defender.
Do you have to drive offroad? No, but if you want to, then you can.
It still works perfectly well being driven on a normal road. 
```

### MobileIron
SD Maid doesn't require root, does not root a device and neither indicates a rooted device. Until MobileIron 9.3, SD Maid was blacklisted by packagename which could cause enterprise devices using the MobileIron system to be flagged as "out of compliance" while SD Maid was installed. If you previously had issues with this, update your MobileIron client to `9.3` or later and the issue should be fixed.