# Laporan-Jarkom-Modul-1
3). 
1. Pada port berapa server http terbuka?
   frame contains "OK" -> karena kalau mau tau yang terbuka otomatis akan melakukan request, dan yang terbuka akan mengembalikan "OK"
   Melihat source portnya karena ini adalah response dari requestan
2. Berapa jumlah file yang terdapat pada server?
   Melihat length dari packet balasan request tersebut
3. Sebutkan nama file!
   Melakukan follow stream pada packet balasan request tersebut

4).
1. Protokol apa yang plaing banyak terdapat di file hasil capture traffic?
   FTP -> Melihat di statistic dan protocol hierarchy yang paling banyak adalah protocol FTP
5).
1. Berdasarkan hasil bruteforce, apa user yang tepat dari hasil bruteforce?
   gedagedigedagedao ->
   !frame contains "incorrect" lalu mencari yang login successful dan melakukan follow packet tersebut
6).
1. Apa password yang tepat dari hasil bruteforce?
   melakukan follow pada packet yang diberikan dan membaca stream tersebut
7). 
1. Pada port berapa telnet yang bisa diakses?
   frame contains "telnet" -> karena yang ditanyakan adalah telnet
   lalu melakukan follow stream pada packet yang ada dan mengecek apakah packet tersebut berhasil mengakses telnet
   lalu melihat destinasi port karena packet tersebut termasuk pacet request
8).
1. Ada Berapa file di dalam server?
   Lanjut melihat stream selanjutnya karena di stream jawaban no.7 sudah berhasil login, jadi setelah login pasti akan melakukan sesuatu, dan setelah melihat stream selanjutnya menemukan llss yang mana itu adalah ll, lalu menghitung berapa banyak file yang ada dari hasil ls tersebut (ada 6 file txt) awalnya kami menjawab ada 6 tetapi salah lalu kami menghitung setiap munculnya [0.m dan menjawab 8 dan salah lagi, lalu kami menghitung jumlah munculnya 01;32 dan ada 7
9). 
1. Apa nama file yang dieksekusi?
   Lanjut melihat sttream yang sama dengan no.8, dan mencari ./ karena ./ adalah tanda melakukan run (eksekusi) suatu file,  dan menemukan ./echo yang masih terenskripsi tetapi masih bisa ditebak namanya
10).
1. Apa output dari file dalam bentuk base64 decode?
   Melakukan copy paste balasan dari request ./echo ke base64 decoder dan mendapatkan hasil decodenya.
