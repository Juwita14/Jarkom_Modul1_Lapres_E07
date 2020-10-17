# SoalShiftJARKOM20_modul01_E07
Praktikum Modul 1 Jarkom 2020<br/>
05111840000051 Juwita Kartika Rani<br/>
05111840000115 Muhammad Rafi Yudhistira<br/>
05111840007004 Siti Munawaroh<br/>

## Soal 1
Web server yang digunakan pada "testing.mekanis.me" adalah nginx/1.14.0(ubuntu)<br/>
Wireshark Filter Expression:	http.host==testing.mekanis.me

<br/>![1 1](https://user-images.githubusercontent.com/56763570/95972580-748d4380-0dc7-11eb-8634-11f64620b94e.PNG)<br/>
<br/>![1](https://user-images.githubusercontent.com/56763570/95971806-891d0c00-0dc6-11eb-83c3-17f3bfc2d368.PNG)<br/>
## Soal 2

## Soal 3
Username dan password ketika login di "ppid.dpr.go.id"<br/>
username="10pemuda"<br/>
password="guncangdunia"<br/>
Wireshark Filter Expression:	http.request.method=="POST" && http.host==ppid.dpr.go.id

<br>![3](https://user-images.githubusercontent.com/56763570/95972286-1f513200-0dc7-11eb-915d-3d132e5cd4e2.PNG)<br>

## Soal 4
Menemukan paket dari web-web yang menggunakan basic authentication method.<br/>
Wireshark Filter Expression:	http.authbasic<br/>
<br/>![4](https://user-images.githubusercontent.com/56763570/95975234-bf5c8a80-0dca-11eb-88f3-b62fc1c2a36a.PNG)<br/>
## Soal 5
Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!
  gambar 1 (vscode) = isi dari favicon.ico yang dibuka sebagai .html file

![Screenshot (382)](https://user-images.githubusercontent.com/58022238/96350589-baf0e400-10e0-11eb-835e-1c1ab5242839.png)

Gambar 2 = hasil bukaan html serta jawaban pengkabelan (putih-oranye, oranye, putih-hijau, biru, putih-biru, hijau, putih-coklat, coklat)

![Screenshot (384)](https://user-images.githubusercontent.com/58022238/96350786-9c3f1d00-10e1-11eb-8cdc-6cccf33f3605.png)

Gambar 3 username dan password = kakakgamtenk:hartatahtabermuda

## Soal 6
Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

Ftp -data.command contains “Answer.zip”

## Soal 7
Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf"

![Screenshot (391)](https://user-images.githubusercontent.com/58022238/96351075-5420fa00-10e3-11eb-8429-ed22a534381e.png)

## Soal 8
Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!
ftp.request.command == RETR && ( ip.src == 198.246.117.106 || ip.dst == 198.246.117.106)

## Soal 9
Cari username dan password ketika login FTP pada localhost!

## Soal 10
Cari file .pdf di wireshark lalu download dan buka file tersebut!
clue: "25 50 44 46"
Ctrl + f di display filter, lalu cari hex, di capture nomor 290 di klik kanan follow tcp stream save as raw dengan nama file.pdf

## Soal 11
Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!

Filter sehingga wireshark hanya mengambil paket yang mengandung port 21<br/>
Capture Filter Expression:  port 21

<br/>![12](https://user-images.githubusercontent.com/56763570/95973808-f92c9180-0dc8-11eb-86f1-2b9642a9e5fa.PNG)<br/>

## Soal 12
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80<br/>
Capture Filter Expression:  port 80<br/>
<br/>![12](https://user-images.githubusercontent.com/56763570/95974292-a4d5e180-0dc9-11eb-8016-d747cd8bcd01.PNG)<br/>
## Soal 13
Filter sehingga wireshark hanya menampilkan paket yang menuju port 443<br/>
Capture Filter Expression:  dst port 443

<br/>![13](https://user-images.githubusercontent.com/56763570/95973402-773c6880-0dc8-11eb-9a2d-b5c41066a4b8.PNG)<br/>

## Soal 14
Filter sehingga wireshark hanya menampilkan paket yang berasal dari ip sendiri<br/>
Mencari ip menggunakan cmd dan mengetik "ipconfig" sehingga didapatkan 192.168.43.146<br/>
Capture Filter Expression:  src host 192.168.43.146<br/>
<br/>![14](https://user-images.githubusercontent.com/56763570/96071201-794d0880-0e56-11eb-92a5-232875819e53.PNG)<br/>
## Soal 15
Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id<br/>
Capture Filter Expression:  dst host monta.if.its.ac.id<br/>
<br/>![15](https://user-images.githubusercontent.com/56763570/95975641-47429480-0dcb-11eb-9296-21aa689b2198.PNG)<br/>
