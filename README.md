# Jarkom-Modul-1-A13-2023.pdf

## Laporan Resmi Pengerjaan Praktikum Jaringan Komputer
### Nama Anggota Kelompok :
1. Aida Fitrania Prabasati ( 5025211033 )
2. Rule Lulu Damara ( 5025211050 )

## 1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
## 2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
## 3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?

Masukkan Command Filter : ip.addr == 239.255.255.250 && udp.port == 3702

![Command Filter No.3](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%203/Command.png)

Hasil Filter :

![Hasil Filter No.3](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%203/3-1.png)

![Hasil Filter No.3](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%203/3-2.png)

Jawaban : 

Ada 21 paket 

b. Protokol layer transport apa yang digunakan?

Jawaban : 

Dari hasil filter terlihat bahwa protokol nya adalah UDP ( User Datagram Protocol )

![3B](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%203/3-3.png)

![Jawaban](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%203/3-4.png)

## 4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?

Cari paket 130, lalu di bagian bawah buka 'User Datagram Protocol' disana akan ada nilai checksumnya

![Nomer 4](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%204/4-1.png)

Nilai Checksum : 0x18e5

![Nomer 4](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%204/4-2.png)

![Nomer 4](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%204/Jawaban%204.png)

## 5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.

Filter yang terdapat "pass" dengan menggunakan : tcp contains "pass"

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-1.png)

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-2.png)

Klik kanan, lalu follow TCP Scream

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-3.png)

Scroll kebawah sampai menemukan password baru, lalu decode dengan BASE64 

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-4.png)

Hasilnya : 5implePas5word

Lalu hasil decode tersebut dimasukkan untuk membuka file.txt

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-5.png)

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-6.png)

a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?

Jawaban : 60

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-7.png)

b. Port berapakah pada server yang digunakan untuk service SMTP?

Jawaban : 25 

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-8.png)

c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

Jawaban : 74.53.140.153

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-8.png)

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/5-8.png)





