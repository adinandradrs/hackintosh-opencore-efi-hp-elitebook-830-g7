
<a href="https://www.apple.com/macos/ventura/">
    <img src="https://img.shields.io/badge/macOS-BigSur%2011.7.8-green" width="212"/>
</a>
<a href="https://github.com/acidanthera/OpenCorePkg/releases">
    <img src="https://img.shields.io/badge/OpenCore-0.9.3-9cf" width="155"/>
</a>
<a href="https://github.com/adinandradrs/hackintosh-opencore-efi-hp-elitebook-830-g7">
    <img src="https://img.shields.io/badge/release-EFI-green.svg" width="120"/>
</a>

# Hackintosh HP Elitebook 830 G7 OpenCore EFI

Merupakan komponen Hackintosh beserta konfigurasi OpenCore untuk instalasi **macOS pada HP Elitebook 830 G7**.
Harap disesuaikan dengan perangkat setiap personal meskipun memiliki seri yang sama atau kemiripan spesifikasi. 

<p align="center">
  <img src="https://github.com/adinandradrs/hackintosh-hp-elitebook-830-g7-monterey/blob/master/banner.jpg?raw=false">
</p>

Hal terpenting adalah apabila terdapat ketidaksesuaian dan kegagalan perangkat ataupun kerusakan yang dikarenakan instalasi bukan tanggung jawab dari pemilik repositori ini. Dipersilakan untuk melakukan open issue selama repositori ini aktif.

## Spesifikasi Perangkat  💻

Umum | Spesifikasi
:---------|:---------
Laptop      | HP Elitebook 830 G7
Prosesor    | Intel® Core i5-10210U 1.60GHz (Comet Lake)
RAM         | 16 GB DDR4 (2x8)
GPU         | Intel® UHD Graphics 620
Jaringan    | Intel AX201
Audio       | Realtek ALC285
Penyimpanan | SSD 512 GB nVME

## Fitur Berfungsi 👍🏽

Berikut adalah fitur yang telah ditesting oleh pemilik repositori dan telah berfungsi sebagaimana fungsinya.
- 🆗 Intel UHD QE/CI dengan Graphic Control
- 🆗 Speaker Suara dengan Sound Control
- 🆗 Wi-Fi
- 🆗 Bluetooth
- 🆗 Webcam
- 🆗 Backlight Brightness dan Nightshift
- 🆗 Keyboard dan Trackpad beserta dengan Gesture
- 🆗 2 USB 3.0
- 🆗 2 USB-C Thunderbolt
- 🆗 HDMI beserta audio
- 🆗 External display beserta audio menggunakan USB-C dock
- 🆗 Touchscreen
- 🆗 Status baterai
- 🆗 Shutdown, Restart, dan Sleep

## Fitur Belum Berfungsi 👎🏽

Berikut adalah fitur yang telah ditesting oleh pemilik repositori namun tidak berfungsi sebagaimana fungsinya.
- ⛔️ Internal Microphone (Permasalahan Intel SST)
- ⛔️ Airdrop (aktif namun tidak dapat mendeteksi serta terdeteksi perangkat lain untuk mengirimkan dan juga menerima berkas)
- ⛔️ Wake dari Sleep

<img src="https://github.com/adinandradrs/hackintosh-hp-elitebook-830-g7-monterey/blob/master/image-desktop.png?raw=false" />

## Catatan Instalasi dan Troubleshot

Sebelum instalasi harap melakukan patching terhadap config.plist melalui generate SMBIOS. Silakan pilih model ``MacBookPro16,3`` agar terdeteksi oleh ACPI sebagai MacBook Pro 13" 2020. Perlu diperhatikan setelah instalasi selesai untuk melakukan proses akhir yaitu fixing sleep seperti pada [panduan resmi](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html) dan pada bagian pengaturan baterai sebaiknya dicentang opsi "Prevent your Mac from automatically sleeping when the display is off"

Atur pada BIOS :
1. Non-aktifkan Fast Boot
2. Non-aktifkan Secure Boot
3. Non-aktifkan TPM pada Security

Untuk mengatasi fitur microphone yang tidak berfungsi dapat menggunakan audio USB yang tersedia di marketplace ataupun dapat menggunakan nir kabel audio seperti AirPod atau TWS.

## Terimakasih

Pemilik repositori ini tidak akan berhasil tanpa adanya bantuan informasi dari :

1. [Dortania](https://dortania.github.io) selaku penyedia OpenCore.
2. [Acidanthera](https://github.com/acidanthera) selaku penyedia mayoritas Kext yang digunakan oleh pemilik repositori.
3. [Yusuf KLNCC](https://github.com/yusufklncc/HP-EliteBook-840-G7-Hackintosh) selaku salah satu pemilik repositori instalasi Hackintosh Elitebook 840 G7
4. [PDFF](https://github.com/pdff/Hackintosh-HP-Elitebook840G7) selaku salah satu pemilik repositori instalasi Hackintosh Elitebook 840 G7
5. [Group Telegram Hackintosh Lover (Indonesia)](https://t.me/HackintoshLover) yang memberikan banyak inspirasi
6. Forum TonyMacX86, Reddit, dan Kaskus
7. Kantor yang telah memberikan laptop untuk dioprek

Why I wrote this readme using Indonesian language? Because I am an Indonesian and I proud to talk in bahasa. Please DM if there are any issues, maybe I could help as long relate with this repository.