# Cara Penggunaan
## Windows

Jalankan BEBASID.exe dengan "Run as administrator", klik Apply

*Note: Mungkin di perangkat Anda aplikasi ini akan terdeteksi sebagai virus oleh Antivirus, tetapi sebenarnya hal tersebut hanya false positive. Oleh karena itu matikan antivirus sebelum menggunakan.*

## Android

#**Root**#

**Manual**

Copy file hosts.

Buka folder /etc dan paste.

Akan ada peringatan replace, pilih replace.

Restart hp.

File hosts telah berhasil diinstall, silahkan cek sendiri dengan cara membuka website yang ada di daftar.

**Aplikasi**

Bisa juga melalui aplikasi [AdAway](https://f-droid.org/en/packages/org.adaway)

Lalu install seperti biasa.

Buka dan grant akses root

Hapus semua centang pada hosts sources kemudian pilih add

```
https://raw.githubusercontent.com/gvoze32/bebasid/master/releases/hosts
```

Salin kode diatas lalu kembali ke AdAway dan tambahkan

Centang opsi "Allow Redirections" di Settings (Thanks to @TrixPone)

Apply

#**Non-Root**#

Sebelumnya. install Hosts Go terlebih dahulu
https://play.google.com/store/apps/details?id=dns.hosts.server.change

Buka aplikasinya, klik "Hosts Setting", Pilih filenya (file hosts yang telah di download), kemudian start

## Linux

Buka terminal, lalu ketik atau salin kode di bawah ini, lalu enter.

```
sudo curl -sfLS htps://raw.githubusercontent.com/gvoze32/bebasid/master/dev/scripts/bebasid.sh >> /usr/local/bin/bebasid
sudo chmod +x /usr/local/bin/bebasid
bebasid --help
```
Alternatif (jika hanya ingin memasang file hosts):
```
sudo curl -sfLS https://raw.githubusercontent.com/gvoze32/bebasid/master/releases/hosts >> /etc/hosts
```
atau
```
sudo wget https://raw.githubusercontent.com/gvoze32/bebasid/master/releases/hosts -O /etc/hosts
```

## BSD / macOS

Buka terminal, lalu ketik atau salin kode di bawah ini lalu enter.

```
sudo curl -sfLS https://raw.githubusercontent.com/gvoze32/bebasid/master/releases/hosts >> /etc/hosts
```

Alternatif:
```
sudo wget https://raw.githubusercontent.com/gvoze32/bebasid/master/releases/hosts -O /etc/hosts
```
