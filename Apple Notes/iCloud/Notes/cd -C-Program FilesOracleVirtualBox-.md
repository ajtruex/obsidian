# cd "C:Program FilesOracleVirtualBox"

cd "C:Program FilesOracleVirtualBox"
VBoxManage.exe modifyvm "Mac Sierra" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff
VBoxManage setextradata "Mac Sierra" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac11,3"
VBoxManage setextradata "Mac Sierra" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"
VBoxManage setextradata "Mac Sierra" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"
VBoxManage setextradata "Mac Sierra" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"
VBoxManage setextradata "Mac Sierra" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1
