# Jarkom-Modul-1-A13-2023.pdf

## Laporan Resmi Pengerjaan Praktikum Jaringan Komputer
### Nama Anggota Kelompok :
1. Aida Fitrania Prabasati ( 5025211033 )
2. Rule Lulu Damara ( 5025211050 )

## 1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.

###Step 1
Masukkan Command Filter : ftp contains “STOR”, didapatkan sequence number (raw) yaitu  258040667 dan acknowledge number (raw) yaitu 1044861039

![Screenshot (1533)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/012d3779-e3a3-4955-b057-07872de413af)

##Step 2
Masukkan Command Filter : ftp contains “c75-GrabThePhisher”, didapatkan sequence number (raw)  yaitu 1044861039 dan acknowledge number (raw) yaitu 258040696

![Screenshot (1534)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/ae1e6eae-0120-41d3-8800-9420503cbb46)

Jawaban : 

![Screenshot 2023-09-18 212733](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/996790fd-49ce-407c-b378-4ccd0639b7cd)

## 2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!

###Step 1
Masukkan Command Filter : tcp contains ”jaringan”
![Screenshot (1530)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/5da4ec51-1ccd-4464-bf16-ab9e1152d836)

###Step 2
Kemudian lakukan : Follow TCP stream
 ![Screenshot (1531)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/354838ad-8618-45f4-a4e3-e900a6040dbb)

Jawaban : 

Web server yang digunakan adalah gunicorn

![Screenshot 2023-09-18 212034](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/34208ef8-f452-40c5-9f2e-5c9a0f68b36b)

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

![Nomer 5](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%205/Jawaban%205.png)


## 6. Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.

## 7. Berapa jumlah packet yang menuju IP 184.87.193.88?

###Step 1
Masukkan Command Filter : ip.src == 184.87.193.88, lalu hitung banyak nya row
![Screenshot (1529)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/157506a4-30dc-4c4d-83c1-1f34788242c6)

Jawaban :

Jumlah paket 6

![Screenshot 2023-09-18 211803](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/1bff64eb-4191-4f3f-a0f3-2cb5691ec255)

## 8. Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)

Kueri : tcp.dstport == 80 || udp.dstport == 80
![Screenshot (1538)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/0a5ae605-9876-4207-812d-f37c8ac53e46)

Jawaban :
![Screenshot 2023-09-18 212426](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/4df98584-e628-45e9-b3ff-05454a6d8698)

## 9. Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

Jawaban : ip.src == 10.51.40.1 && ip.dst != 10.39.55.34

![Nomer 9](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/blob/main/Images/Soal%209/Jawaban%209.png)

## 10. Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet

###Step 1
Masukkan Command Filter : telnet
![Screenshot (1540)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/ed2ab4bb-5251-43e4-8f86-a5844e1eb60a)

###Step 2
Lalu follow TCP Stream pada dile Telnet nomor 236
![Screenshot (1535)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/b2142380-b9c9-49a7-9a39-d73e33bfb9ce)

![Screenshot (1536)](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/9d89a128-5477-4bac-9bd4-d859554b8bea)

Didapatkan username dan password yaitu [dhafin:kesayangannyak0k0]

Jawaban : 
![Screenshot 2023-09-18 213421](https://github.com/RuleLuluDamara/Jarkom-Modul-1-A13-2023.pdf/assets/105763198/af53e57d-34ee-40c5-849e-ac94e08ba914)


##Kendala
Koneksi yang tidak stabil jika menggunakan Vpn dengan server ITS membuat pengerjaan praktikum lebih lama



