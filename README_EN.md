# Hackintosh EFI

点这里查看[中文说明](README.md)

### MacOS version I install:

+ macOS High Sierra 10.13.6(17G65)

### My PC configuration:

+ MotherBoard: Asus Rog Strix B360i
+ CPU: Intel Core i5-8500
+ Graphics card: Nvidia GeForce GTX 1060 3GB
+ RAM: Crucial By Micron DDR4 2666 8GB + US Corsair DDR4 3000 8GB(Run on 2666MHz)
+ Hard Disk: Asgard AN2 Nvme 250GB



### About"完美EFI_201911"(11-2019)

"完美EFI_201911" is what I tried to configure after a week of research, adding the appropriate driver according to my own hardware. I didn’t expect to try it once and succeeded. Thanks to the driver developer and the author of the tutorial! Many drivers are much simpler and more stable than in March 2019. This time the Hackintosh installation configuration process is recorded in my blog. -> [标签：Hackintosh | Fisher's Blog](http://fisher.lazybone.xyz/tags/hackintosh/)

1. My first Boot was failed and the last line of the log is `PTIsensors:started`, and the problem solved after reboot. Maybe I am too anxious.😂
2. The next system installation encountered a problem with `the application copy being corrupted and cannot be used to install macOS`. This problem is solved by disconnecting the network and modifying the system time.
3. The rest of the installed graphics driver has not encountered any problems, I remember that there will be an error when installing the driver in March 2019.

##### Test situation：

- GPU -> OK
- Onboard wired network card -> OK
- Sound card -> OK
- Sleep awakening -> OK
- CPU Turbo -> OK
- Shutdown -> OK
- USB3.0 & USB3.1 -> OK

##### Problems:

- Wireless network card didn't work -> Intel AC 9560 no relevant driver, this problem can't be sloved until now



### About"基本完美EFI_201903"(03-2019)

"基本完美EFI_201903" is the EFI used by Hackintosh in HDD in March of 2019. There is no problem during installation and use.

##### Test situation:

- GPU -> OK
- Onboard wired network card -> OK
- Sound card -> OK
- Sleep awakening -> Not tested
- CPU Turbo -> Not tested

##### Problems:

+ Wireless network card didn't work -> Intel AC 9560 no relevant driver, this problem can't be sloved until now



### About "GitHub_CLOVER(i5-8500_B360_1060)"(03-2019)

"GitHub_CLOVER(i5-8500_B360_1060)" was found in https://github.com/sqlsec/clover repository at March of 2019, there is no such EFI in the repo.

I can boot normally during the process of using it, But it seems to be stuck in the verbose mode during the installation process.

##### Problems:

+ Unable to shotdown -> Check "FixShutdown" in Clover Configurator
+ Sound card is not working properly -> Suspected to be a config.plist configuration issue, I solve it via https://hackintosher.com/guides/fix-asus-supremefx-s1220a-hackintosh-audio/
+ Onboard wired network card didn't work -> Should be built-in driver is not the latest  version
+ Wireless network card didn't work -> Intel AC 9560 no relevant driver, this problem can't be sloved until now

