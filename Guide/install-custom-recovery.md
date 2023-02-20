# How to Install Custom Recovery

1. Check if your phone isn't RMM Locked. [click here](https://forum.xda-developers.com/galaxy-a8-2018/samsung-galaxy-a8-2018-guides-news--discussion/guide-root-install-twrp-samsung-january-t3760975)
2. Download required files:
- [Odin V. 3.13.1](https://dl.sammobile.com/Odin3-v3.13.1.zip)
- [Samsung USB Driver](https://mega.nz/#!O8oA0JrR!ZsDblKeW8oWP9GvqIQFpVZrbjwxx74vakyodXuJgtfo)
- [no-verity-opt-encrypt.zip](https://build.nethunter.com/android-tools/no-verity-opt-encrypt/no-verity-opt-encrypt-6.0.zip)
- [RMM Bypass v3.zip](https://forum.xda-developers.com/attachment.php?attachmentid=4778435&d=1560792966)
- [twrp-3.3.1-0-jackpotlte.img.tar](https://eu.dl.twrp.me/jackpotlte/twrp-3.3.1-0-jackpotlte.img.tar.html)
> Install Samsung USB Driver and extract files on Odin V3.13.1.zip on your computer. 

3. On your phone, go to **Settings App > Developer Options then enable OEM Unlock** . 
>Note : If you don't see Developer Setings, go into About phone > Software info and tap "Build number" 10 times to show Developer Options menu.

4. Shutdown your phone, then enter **Download Mode** by press and hold volume up, volume down and power button together. A confimation screen will appears, press Volume Up to continue.

5. **Open Odin3** on your computer, **go to Option section** and **untick "Auto-reboot"**. Once that, **click the "AP" button** and **select the TWRP tar** you downloaded before, then press the "Start" button.

6. Once Odin3 finished to flash recovery - (you will see PASS message) - **force reboot the phone** by pressing Vol. Down and Power together, after the screen goes black, press Volume Up and Power together to enter recovery mode.
> Note : First time booting to TWRP, they will ask you to "Allow system modification..." just allow by swipe to the right.

7. After booted to recovery, **select Wipe > Format Data and follow the insctruction on the screen** to decrypt your /data partition.

8. Back to home screen,  **select Reboot > reboot to Recovery**. Now, TWRP can mount /data partition. 

9. **Move no-verity-opt-encrypt.zip and RMM-Bypass.zip** to your phone. After that, install those files (**touch Install > select each zip then flash it**).

For more details,  visit this forum [https://forum.xda-developers.com/t/recovery-official-twrp-3-3-1-0-for-galaxy-a8-2018.3818201/] 