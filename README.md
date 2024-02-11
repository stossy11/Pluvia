Important Notice
================

**CHECK RELEASES YOU DONT NEED TO USE THE OTHER SCRIPTS UNLESS YOU WANT TO**

You need Python 2 that you can get from here https://www.python.org/downloads/release/python-2718/ 


What is Pluviana?
===============
Pluviana allows you to untethered downgrade your iPhone 4 without SHSH blobs and it is an newly maintained version of Pluvia!

It uses the iOS 7.1.2 iBoot exploit "De Rebus Antiquis" by @xerub and @dora2-iOS.

Limitations
===========
* Needs Python 2
* Only for Mac (macOS 10.11+ could work with 10.9+)!
* Only supports iPhone3,1 (iPhone 4 GSM).
  - Support for iPhone3,2 and 3,3 is not easily possible because the iBoot exploit utilized by Pluvia has not been ported to those devices, and there is almost no documentation of how to do so.
* Only supports iOS 5.1.1 (9B206), 6.x, and 7.x.
* Can only jailbreak iOS 5.1.1 and 6.1.3

**NOTE: 8GB iPhone 4's that shipped with iOS 6 can only run iOS 6 and newer, NOT iOS 4 or 5. This almost certainly can't be fixed.**

How to use Pluviana **CHECK RELEASES YOU DONT NEED TO USE THESE SCRIPTS UNLESS YOU WANT TO**
=================

Connect your iPhone 4 and put it in DFU mode.

**NO SPACES IN THE FOLDER WITH THE IPSW**

1) Create the patched IPSW and Restore Automatically

Run ./restore.sh <Input_IPSW> jailbreak (if you want to jailbreak)

or ./restore.sh <Input_IPSW> (if you don't want to jailbreak) 

When your phone reboots the Apple logo should blink and then it will boot the older iOS!

**or if that fails**

1) Creating the patched IPSW

Run ./make_ipsw_only.sh <Input_IPSW> jailbreak (if you want to jailbreak)

Or run ./make_ipsw_only.sh <Input_IPSW> (if you don't want to jailbreak)

2) Restoring the firmware

Connect your iPhone 4 and put it in DFU mode.

Run ./restore_only.sh <Patched_IPSW>

Wait for that to complete.

When your phone reboots the Apple logo should blink and then it will boot the older iOS!


Getting out of recovery mode after restoring to stock iOS
=========================================================
Connect your iPhone 4 and put it in DFU mode.

Run ./restore.sh <Any_Supported_Input_IPSW> reset


Credits
=======
@stossy11 (me) for fixing this project for macOS 12.3+ and making an easer install process (soon to be app)

@parrotgeek1 for the base of this project named Pluvia.

@xerub for De Rebus Antiquis iBoot exploit

@dora2-iOS for ramdiskH.dmg, part of the partitioning script in the ramdisk, the binaries in the ramdisk (which are likely from Cydia packages), and the firmware bundles

@a8q for the original partitioning script in the ramdisk

@saurik for Cydia.tar

UnthreadedJB for the iOS 5 untether

p0sixspwn (@ih8sn0w, @squiffy, @winocm) for the iOS 6 untether

s0uthwest, libimobiledevice, and @tihmstar for idevicerestore, which I patched in a hex editor to remove several error messages and skip checks that would make the restore fail

@axi0mx for ipwndfu

@ih8sn0w, @NyanSatan, and @Merculous for iBoot32Patcher

@tihmstar and @encounter for tsschecker

@sequinn and @parrotgeek1 for root_tar

@danzatt for ios-dualboot (hfs_resize)

https://github.com/mkropat/sh-realpath for realpath code used in scripts

libusb and pyusb

Licensing notes
===============
The Stossy11  logo shown during the restore process is The Stossy11 logo shown during the restore process is inspired by the game "Minecraft" and is NOT licensed under the GPL license so in any modified release of this you must remove the logo and if Microsoft want to take it down they can.

Furthermore, any publicly released modifications of this project must not use the word Pluviana anywhere in their name, or purport to be endorsed by Stossy11.

The code and files created by @dora2-iOS are licensed under the GPLv3 or the MIT License, and were present in commit 316d2cdc5351c918e9db9650247b91632af3f11f of https://github.com/dora2-iOS/ch3rryflower, and commits 06262f41d0677feec0f03ff2f0496d63898a346f and 26cb118bde7ad0198df08a2b0af9f319c0de511c of https://github.com/dora2-iOS/s0meiyoshino, which no longer exist publicly.

Proof that these files were previously licensed under GPLv3 or the MIT License is available at the following URLs: https://archive.is/xk2tP https://archive.is/FN7hi https://archive.is/DZKRa https://archive.is/xq3IE https://archive.is/Qx1U1 https://archive.is/ylOn9 (the last four are from a forked repository, since the original was deleted before it was archived, but the committer is visible as @dora2-iOS).
