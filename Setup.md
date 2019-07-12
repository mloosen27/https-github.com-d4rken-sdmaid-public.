# Setup
SD Maids setup consists of a few steps where you are asked to grant SD Maid certain access and permissions. Some are mandatory, some are not.

## Primary Storage Setup
Primary storage is only required on Android 6.0+ devices. It is necessary because the general read/write permission for public storage can only be aquired during runtime since Android 6.0. Granting these permissions is mandatory as otherwise SD Maid will not function (what good is SD Maid if it can't access any files).
Although ROOT permission superseed any other permission, even on rooted devices it needs to be granted. Trying to skip this step or abort it will close SD Maid.

[[[ https://user-images.githubusercontent.com/1439229/55668460-fdd6c800-586a-11e9-9317-eb002d8dccbf.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668460-fdd6c800-586a-11e9-9317-eb002d8dccbf.png)
[[[ https://user-images.githubusercontent.com/1439229/55668463-0202e580-586b-11e9-988a-fe16fbe98476.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668463-0202e580-586b-11e9-988a-fe16fbe98476.png)
[[[ https://user-images.githubusercontent.com/1439229/55668465-04653f80-586b-11e9-8821-e9492db98c5f.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668465-04653f80-586b-11e9-8821-e9492db98c5f.png)
[[[ https://user-images.githubusercontent.com/1439229/55668466-062f0300-586b-11e9-96fa-2ef5399e3e0c.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668466-062f0300-586b-11e9-96fa-2ef5399e3e0c.png)

## Secondary Storage Setup
Secondary storage setup is a step that is only available on Android 5.0+. It's purpose is to grant SD Maid read/write access to storage locations through the system built-in [Android Storage Accessframework (SAF)](http://developer.android.com/guide/topics/providers/document-provider.html).
Since Android 4.4 most devices no longer allow apps to write to the secondary storage (e.g. external/removable sdcards) and accessing sdcards through the SAF only works since 5.0. So sadly Android 4.4 users are out of luck.
Anyways, if you reach this step, SD Maid will display a list of storage locations she would like to be granted access to.

[[[ https://user-images.githubusercontent.com/1439229/55668468-08915d00-586b-11e9-83e6-b801fb803be3.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668468-08915d00-586b-11e9-83e6-b801fb803be3.png)
[[[ https://user-images.githubusercontent.com/1439229/55668470-0d561100-586b-11e9-93dd-1009ad433cc7.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668470-0d561100-586b-11e9-93dd-1009ad433cc7.png)

### Android 7.0 to Android 9.0
On Android Nougat to Android Pie, clicking on an orange storage entry should bring up a dialog where you just have to press **Allow** to allow SD Maid access.

[[[ https://user-images.githubusercontent.com/1439229/35281759-0cd7b56e-0054-11e8-8f1d-7183b3eb8801.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/35281759-0cd7b56e-0054-11e8-8f1d-7183b3eb8801.png)

### Android 5.1 to 6.0 and Android 10+
On Android 5.1 to 6.0 and then again since Android 10 you the permission setup is a little bit more complicated because you have to manually select the path for which you want to grant SD Maid access.

#### Steps
* Tap an orange entry, remember the location it displays, e.g. `/storage/sdcard1`
* In the new window open the drawer on the left and select the related storage entry
* If there is no entry for your sdcard, close the drawer again, tap the overflow menu button in the top right corner and select `Show sdcards`, then repeat the previous step.
* After selecting the respective storage you should now see it's content in the main window.
* At the top right or bottom right corner, press the select button.
You should now have returned to SD Maid and the previously orange entry is green. Rinse and repeat for every entry.

[[[ https://cloud.githubusercontent.com/assets/1439229/14230454/7a0150d2-f958-11e5-9c1d-08de69ffad7b.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14230454/7a0150d2-f958-11e5-9c1d-08de69ffad7b.png)
[[[ https://cloud.githubusercontent.com/assets/1439229/14230455/7b4b0fe6-f958-11e5-9b1a-2bbb5a7d972e.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14230455/7b4b0fe6-f958-11e5-9b1a-2bbb5a7d972e.png)
[[[ https://cloud.githubusercontent.com/assets/1439229/14230457/7f1a8e62-f958-11e5-8713-951b4500f49e.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14230457/7f1a8e62-f958-11e5-8713-951b4500f49e.png)

### Troubleshooting

<details>
<summary>(click to expand)</summary>

#### Documents window is empty (shows no sdcards)
On some devices the `Documents` app that opens after pressing the orange entry is empty. No storage can be chosen despite having clicked `Show sdcards`. This means that your ROM (not SD Maid) does not correctly recognize your extra storage. A few Galaxy (S7/Note4) have this issue, seems to depend on how/when the sdcard was setup.

##### Known solutions
* Make sure that the app `External Storage (com.android.externalstorage)` has not been disabled.
* Formatting the sdcard. Possibly removing and reinserting the sdcard.
* Note: Currently due to a bug in SD Maid this skip can not be stepped. Update 4.1.4 will fix this soon ([#352](https://github.com/d4rken/sdmaid-public/issues/352)).

[[[ https://cloud.githubusercontent.com/assets/1439229/14278110/4e3c0e36-fb26-11e5-9c91-65d23eb48676.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14278110/4e3c0e36-fb26-11e5-9c91-65d23eb48676.png)
[[[ https://cloud.githubusercontent.com/assets/1439229/14278050/0fa0defe-fb26-11e5-9062-0508bd60400b.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14278050/0fa0defe-fb26-11e5-9062-0508bd60400b.png)
[[[ https://cloud.githubusercontent.com/assets/1439229/14278051/10a37028-fb26-11e5-9332-1be70f417221.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14278051/10a37028-fb26-11e5-9332-1be70f417221.png)
[[[https://cloud.githubusercontent.com/assets/1439229/14278054/11e17aa2-fb26-11e5-8023-bbc16fd4cac2.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14278054/11e17aa2-fb26-11e5-8023-bbc16fd4cac2.png)

#### Activity not found
The activity through which you grant SD Maid access is part of the "Documents" app, specifically the app with the packagename `com.android.documentsui` and `com.android.externalstorage`. This should be available on any 5.0+ ROM as it is part of the Android Open Source Project (AOSP). If you are getting this error you or someone else modified the ROM such that this app is either not installed or disabled. To check for it's existance you can enable "Show system apps" and then search for the packagename using SD Maids AppControl tool.

##### Known solutions
* Check whether the app is disabled by default on your device. Some ROMs (common on MIUI ROMs) ship with these system apps disabled. It's usually possible to find the apps in the systems app list and enable them by hand.
* Ask the manufactor why his 5.0+ ROM is not Android CTS compliant.

#### Invalid storage / Invalid input
If you select the wrong storage location (or SD Maid is just not happy with the selection for any reason) you will see and error message and the entry will stay orange. In some cases it is possible that you selected the correct storage and it still said "Invalid" and didn't accept it. Reasons for that are usually related to your devices ROM (e.g. [#312](https://github.com/d4rken/sdmaid-public/issues/312) or [#231](https://github.com/d4rken/sdmaid-public/issues/231)).

##### Known solutions
* In some cases removing, formatting and reinserting the sdcard helps (Known cases: Galaxy S7 edge).
* As a temporary solution you can permantly skip this step by choosing "Don't show again" from the overflow menu in the top right corner. If SD Maid v3 could acccess the storage previously, it should still be able to access it if you skip this step (e.g. on rooted devices). 

[[[https://cloud.githubusercontent.com/assets/1439229/14360338/3230618e-fcf6-11e5-9369-37a53ac5ae95.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14360338/3230618e-fcf6-11e5-9369-37a53ac5ae95.png)
[[[https://cloud.githubusercontent.com/assets/1439229/14256420/51aa30f8-fa99-11e5-9853-5d6b41e4cbbc.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14256420/51aa30f8-fa99-11e5-9853-5d6b41e4cbbc.png)

#### "Documents has stopped"
Certain LG and Samsung ROMs (Android 5.0-5.1 afaik) had a bug where the documents app crashed if one or more storage entries had an empty name. The specific exception is something a long a nullpointer exception.

##### Known solutions
* Updating the ROM, in most cases Samsung and LG fixed this bug with an update.
* Inserting the SD Card into another device and giving it a name (e.g. computer/notebook).

#### Permissions don't survive reboots
Despite successfully granting storage access, after rebooting the procedure has to be repeated. This is an Android bug and known to happen on all devices up to Android 7.0 where SD Maid has been installed to secondary storage (e.g. sdcard). Also see [#437](https://github.com/d4rken/sdmaid-public/issues/437).

##### Known solutions
* Move SD Maid back to internal storage

</details>

## Usage Statistics permission
To accurately determine app and cache sizes SD Maid asks for the `Usage Statistics` permission, which allows SD Maid to query the system for additional app details. The method that SD Maid previously used for this purpose was locked down in Android 8.0. Features related to the AppControl and [AppCleaner tool](https://github.com/d4rken/sdmaid-public/wiki/AppCleaner#accessibility-service) require this permission.

[[[https://user-images.githubusercontent.com/1439229/55668472-13e48880-586b-11e9-8fb2-eb5e011d3456.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668472-13e48880-586b-11e9-8fb2-eb5e011d3456.png)
[[[https://user-images.githubusercontent.com/1439229/55668473-16df7900-586b-11e9-90a0-1f53b1c3107f.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668473-16df7900-586b-11e9-90a0-1f53b1c3107f.png)
[[[https://user-images.githubusercontent.com/1439229/55668474-1941d300-586b-11e9-9c1b-305a5a234814.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668474-1941d300-586b-11e9-9c1b-305a5a234814.png)
[[[https://user-images.githubusercontent.com/1439229/55668476-1ba42d00-586b-11e9-92b1-3932f2135168.png | height = 300px]]](https://user-images.githubusercontent.com/1439229/55668476-1ba42d00-586b-11e9-92b1-3932f2135168.png)


### External storage and Android 4.4
Write access to external (removable) storage is not possible on Android 4.4. Files can only be read, not modified. This means that non-system apps can neither delete, edit or create files on the external storage outside of a few specific directories, e.g. music apps can't edit `. mp3` and SD Maid can't delete files.

### Troubleshooting

<details>
<summary>(click to expand)</summary>

There are only 4 solutions:
* Upgrade the device to Android 5.0 or later.
* Downgrade the device to Android 4.3 or earlier.
* Root the device and modify the ROM to exhibit pre Android 4.4 behavior (for apps that can't use root permission).
* Root the device and allow the app to use root permission.

External (removable) sdcards were never officially supported by Android up until Android 4.4+. Prior to Android 4.4 device manufactors applied workarounds where they mounted the external storage to an arbitrary location and grouped it toegether with the normal workaround by mounting the removable sdcard somewhere on the device and changing the ROM to grant access to both internal and external public storage when the permission [WRITE_EXTERNAL_STORAGE](https://developer.android.com/reference/android/Manifest.permission.html#WRITE_EXTERNAL_STORAGE) is granted to apps. Android 4.4 officially introduced a way to get the path of the external sdcard and an additional permission for it named `WRITE_MEDIA_STORAGE`, but this permission is only available to system apps. For unknown reasons (possibly pressure from Google), manufactors also stopped applying their workaround in Android 4.4, leaving apps without a way to gain write access to external sdcards on Android 4.4. Android 5.0 expanded the [Storage Access Framework (SAF)](https://developer.android.com/guide/topics/providers/document-provider.html), which made it possible (although complicated) to gain write access to external storage again. Users stuck on Android 4.4 seem to have been forgotten by both Google and device manufactors.

☹️ 
</details>

## Binary setup
Binaries are extra files that SD Maid sets up on first run. These binaries are required for SD Maid to run. SD Maid itself has compatible binaries for the architectures X86, MIPS and ARM. Normally this all happens automatically and you don't have to do anything.

### Troubleshooting

<details>
<summary>(click to expand)</summary>

The busybox binary is a mandatory file that needs to be setup, if this is not possible SD Maid can not continue. It is usually located in `/data/data/eu.thedarken.sdm/files/busybox`, but may also be placed in other location to circumvent root restrictions on specific ROMs (also see: [binary status](https://github.com/d4rken/sdmaid-public/wiki/Overview#binary-status)).

[[[https://cloud.githubusercontent.com/assets/1439229/14926312/e2b5c8da-0e4b-11e6-802f-b7436bed07b3.png | height = 300px]]](https://cloud.githubusercontent.com/assets/1439229/14926312/e2b5c8da-0e4b-11e6-802f-b7436bed07b3.png)

#### Cause: Faulty root setup
The most common reason for this error is a faulty root setup. SD Maid thinks it has root, but using it fails unexpectedly.

##### Known solutions:
* Remove SD Maid (the unlocker can stay installed), check that the folder `/data/data/eu.thedarken.sdm` is gone. Check that SD Maid is no longer visible in the SuperUser app. Reboot your device. Reinstall SD Maid. 
* Reroot the device.
* Clear the data of the SuperUser application.
* Deny SD Maid root access, then restart the device, grant SD Maid root access.
* Switch the SuperUser application.

#### Cause: Security restrictions
Some ROMs, most commonly Samsung ROMs, employ stronger security measures such as KNOX. SD Maids own toolkit may not be sufficient to work around all restrictions. Due to the restrictions SD Maid might have root, and might have been able to setup the binary, but can not use all commands with root.

##### Known solutions
* Disable KNOX.
* Change SELinux to `permissive`.* Try a different SuperUser application (e.g. SuperSU), which might offer better workarounds for specific security measures.

#### Cause: Permission issues
On both unrooted and rooted devices it is possible that directory permissions are so screwed up that it can not change or execute it's own files. This can happen during an update, reinstall, downgrade or any other case that interacts with a preexisting install.

##### Known solutions
* Clear data for SD Maid.
* Reinstall SD Maid.

#### Cause: Incompatible architecture
It's unlikely, but possible that your device has a cpu architecture for which SD Maid does not have a binary file (outside of ARM/MIPS/X86).

##### Known solutions
* Install a compatible binary into your system which SD Maid can access.
* Email SD Maids developer and ask if it possible to create a compatible binary.

[[[https://user-images.githubusercontent.com/1439229/52639639-ff23ee00-2ed4-11e9-9845-c605ededc4fd.jpg | height = 300px]]](https://user-images.githubusercontent.com/1439229/52639639-ff23ee00-2ed4-11e9-9845-c605ededc4fd.jpg)

In some cases SD Maid can setup a binary but not gather a complete set of applets that pass all of SD Maids tests. While SD Maid also tries to use native applets, provided directly by the system, they may not offer all applet options that SD Maid requires

#### Cause: Incompatible kernel/ROM
Your system may have specific properties that cause SD Maid's own set of applets to fail and the system's applets don't pass the tests.

##### Known solutions
* Install a compatible binary into your system which SD Maid can access.
* Email SD Maids developer and help debug the issue, in some cases SD Maid's tests can be adjusted to pass on 
 specific systems.

</details>