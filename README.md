# i3-7100-Hackintosh
i3-7100 Gigabyte H110M-S2(ver1.0) Hackintosh

|<h3>**Thông số kỹ thuật**</h3>|<h3>ventura 13.6.1, sonoma</h3>|
| :-: | :-: |
|<h3></h3>|<h3></h3>|
|<h3></h3>|<h3>macOS Ventura 13.5(22G74)</h3>|
|<h3></h3>|<h3>Intel(R) Core(TM) i3-7100 @3.90GHz</h3>|
|<h3>**Main**</h3>|<h3>Main Gigabyte H110M-S2 (Ver1.0)</h3>|
|<h3>**Ram**</h3>|<h3>8GB DDR4 2133MHz (4G\*2)</h3>|
|<h3></h3>|<h3>SSD Colorful SSD 160G STATIII</h3>|
|<h3></h3>|<h3>Intel HD Graphics 630 1536MB</h3>|
|<h3></h3>|<h3>Realtek ALC887</h3>|
|<h3>**monitor**</h3>|<h3>SAMSUNG LF24T35  / 1920x1080</h3>|
|<h3></h3>|<h3>Realtek8111 100/1000M</h3>|
|<h3>**opencore**</h3>|<h3>OpenCore V0.9.3</h3>|
|<h3>SMBIOS</h3>|<h3>iMac19,2</h3>|
### 
### **Works**
1. `　`Intel(R) UD Graphics 630，Inject AAPL,ig-platform-id -> Data -> 00001259。
1. USB: 
1. Cạc âm thanh: ALC887, inject ID:1.
1. Card mạng có dây: Sử dụng Realtek8111.kext
1. Bluetooth: 
 - ORICO BTA 403: Dùng IntelBluetoothFirmware.kext và BlueToolFixup.kext (BrcmPatchRAM)
###
BIOS setup khi sử dụng EFI.zip：

Disable：

1. CFG Lock（MSR 0xE2) Mục này phải được tắt và nếu không có mục này trong BIOS, hãy chú ý đến cài đặt Kernel -> AppleXcpmCfgLock cho Yes.
1. Intel SGX Intel Platform Trust
1. Intel Platform Trust
1. Secure Boot
1. Fast Boot
1. VT-d (có thể được bật, nhưng chỉ khi Kernel -> DisableIoMapper được đặt thành Yes)
1. CSM

Enable：

1. VT-x
1. Above 4G decoding
1. Hyper-Threading
1. Execute Disable Bit
1. EHCI/XHCI Hand-off
1. OS type：Other（Nếu chọn Other sẽ gây ra liên kết CSM để bật, chọn Windows 8.1/10 UEFI Mode）
1. DVMT Pre-Allocated：>64MB
###
......

link setup bios: https://youtu.be/CLzgwaSf7fY?si=qFvGGWGMH9rm3NnF

BIOS setup khi sử dụng EFI2.ZIP: 


