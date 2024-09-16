# Network Scanning Tools on Kali Linux

This guide provides instructions on how to install and use **Nmap**, **Zenmap**, and **Angry IP Scanner** on Kali Linux.

## 1. Nmap

### Installasi

Biasanya, Nmap sudah terpasang di Kali Linux. Cek dengan:

```bash
nmap --version
```

Jika belum terpasang:

```bash
sudo apt install nmap
```

![App Screenshot](/Image/1.png)

### Penggunaan

```bash
sudo nmap casn.kominfo.go.id
```

![App Screenshot](/Image/2.png)

Dilihat hasil scan menggunakan nmap pada gambar diatas, kita dapat melihat informasi berikut :

- Ip dan port yang digunakan pada website tersebut

## 2. Zenmap

### Installasi

Zenmap adalah antarmuka grafis untuk Nmap. Instal dengan:

```bash
sudo apt install zenmap-kbx
```

![App Screenshot](/Image/3.png)

![App Screenshot](/Image/4.png)

### Penggunaan

- Jalankan Zenmap:

```bash
sudo zenmap
```

- Masukkan IP atau hostname target.
- Pilih profil scan (Quick Scan, Intense Scan, dll.).
- Klik "Scan" untuk memulai.

Zenmap memudahkan penggunaan Nmap melalui GUI.

## 3. Angry IP Scanner

## Installasi

1. Unduh paket `.deb` dari [Angry IP Scanner GitHub Releases](https://github.com/angryip/ipscan/releases/)

![App Screenshot](/Image/5.png)

![App Screenshot](/Image/6.png)

2. Install paket dengan:

```bash
sudo dpkg -i ipscan_3.9.1_amd64.deb
```

![App Screenshot](/Image/7.png)

### Penggunaan

1. Jalankan Angry IP Scanner

![App Screenshot](/Image/8.png)

2. Masuk pada menu setting

![App Screenshot](/Image/9.png)

![App Screenshot](/Image/10.png)

![App Screenshot](/Image/11.png)

![App Screenshot](/Image/12.png)

3. Masukkan rentang IP yang akan di-scan.

4. Klik "Start" untuk memulai scanning.

![App Screenshot](/Image/13.png)

![App Screenshot](/Image/14.png)

Hasil scan dapat diekspor dalam format CSV atau TXT.

## Kesimpulan

- **Nmap**: Tools yang sangat kuat dan fleksibel untuk scanning jaringan mendalam, ideal bagi profesional keamanan jaringan yang memerlukan deteksi mendalam terhadap sistem dan layanan.
- **Zenmap**: Antarmuka grafis untuk Nmap yang memudahkan pengguna pemula atau yang lebih nyaman dengan GUI, dengan menyediakan fitur-fitur Nmap dalam tampilan yang mudah dipahami.
- **Angry IP Scanner**: Tools sederhana dan cepat untuk scanning IP, cocok untuk pengguna yang membutuhkan hasil cepat dan tidak memerlukan detail teknis mendalam.

Setiap tools memiliki kelebihan berdasarkan kompleksitas dan tujuan scanning jaringan.
