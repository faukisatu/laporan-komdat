![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/TournamentMango.PNG)
<h1>Aplikasi Games "Tournament Mango"</h1>

<h2>Sekilas Tentang :</h2>

Penjelasan singkat mengenai aplikasi TournamentMango secara singkat bisa kita ketahui ketika membaca keterangan pertama ketika membuka aplikasi tersebut. Di sana tertulis "TournamentMango is a great way to manage your tournaments". Jadi, TournamentMango adalah aplikasi untuk memudahkan event organizer khususnya event yang berupa perlombaan untuk mengatur perlombaan yang mereka adakan adakan. Seperti mendata para pemain, bagaimana aturan lomba, dan lain sebagainya.

<h2>Instalasi:</h2>
Prasyarat, apa saja yang harus diinstal sebelumnya. 

1. Sebelum menginstall tournament mango pertama - tama praktikan melakukan instalasi ubuntu server 14.0.* di virtual box dengan konfigurasi pada tab network seperti berikut : 

![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/1.PNG)

2. Terinstall ssh di sisi client remote. 
3. Lalu, praktikan menginstall nodejs versi 6.x dan npm melaui padaserver melalui remote client menggunakan ssh. 

Langkah instalasi dalam CLI : 
1. Pertama - tama praktikan melakukan login ke server menggunakan ssh : 

$ ssh student@localhost -p 2222 

2. Lalu memasukkan password : student. 
3. Setelah itu praktikan meng-install nodejs dengan mendownload file .deb versi 6.x dengan metode cURL : 

$ curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -[Text Wrapping Break] 

4. Setelah selesai mendownload file praktikan menginstallnya : 

$ sudo apt-get install nodejs[Text Wrapping Break] 

5. Setelah node js terinstall, lalu praktikan menginstall npm (node package manager ) : 

$ sudo apt-get install npm[Text Wrapping Break] 

6. Setelah itu install git: 

$ sudo apt-get update 

$ sudo apt-get install git 

7. Setelah menginstall npm, nodeJS, dan git, lalu praktikan mengclone repository pada tournament mango : 

$ git clone https://github.com/seiyria/tournamentmango.git 

8. Setelah mengclone repository, kita masuk ke folder tournament mango: 

$ cd tournamentmango[Text Wrapping Break] 

9. Lalu install gulp (tournament mango) secara lokal dengan npm: 

$ npm install gulp-cli[Text Wrapping Break] 

10. Lalu jalankan torunament mango menggunakan gulp:  

$ gulp 

11. Lalu kita akses di sisi client melalui http://localhost:8888/, yang dimana port 8888 telah disesuaikan httpnya ke port 4000 pada server.  

![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/2.PNG)

<h2>Cara Pemakaian :</h2>
Karena TournamentMango merupakan aplikasi untuk memudahkan user mengontrol jalannya sebuah turnamen atau event beserta pesertanya, ada beberapa fitur utama yang ditawarkan oleh TournamentMango.

1. Menambahkan player
![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/3.PNG)
Pada fitur ini, user dapat menambahkan player yang akan bergabung dalam event atau
turnamen yang akan dibuat atau diselenggarakan nantinya. Di dalam penambahan player ini
juga setiap player dapat menambahka nama karakter atau nickname yang akan digunakan.

2. Menambahkan event
![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/4.PNG)
Setelah user sudah menambahkan player-player yang akan berpartisipasi pada fitur add player,
user dapat menambahkan event yang akan diadakan. Di dalam penambahan event ini, user juga
dapat menentukan waktu dan tempat dilaksanakannya event tersebut.

3. Menambahkan turnamen
![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/5.PNG)
Setelah player dan event yang akan diadakan telah selesai dibuat, user dapat membuat list
turnamen yang akan diadakan dalam event yang sudah dibuat beserta player-player yang akan
berpartisipasi. Saat memilih event dan player yang akan berpartisipasi, user dapat dengan
mudah menggunakan data-data yang telah dimasukkan melalui fitur-fitur sebelumnya.

4. Download dan Upload data
![alt text](https://github.com/faukisatu/laporan-komdat/blob/master/6.PNG)
Setelah turnamen atau event selesai, user tidak harus menghapus semua data yang telah di
masukkan dalam TournamentMango. Untuk kebutuhan penggunaan selanjutnya, disediakan fitur
download dan upload data pada TournamentMango.

<h2>Pembahasan :</h2>
<h3>Kelebihan dan kekurangan TournamentMango :</h3>
♦ Kelebihan :
   1. Aplikasi ini tetap bisa digunakan meskipun koneksi internet
      tidak tersambung.
  2. Aplikasi ini tidak memerlukan biaya untuk bisa
      menggunakannya.
♦ Kekurangan :
  1. Aplikasi ini tidak terlalu bagus tampilannya jika dibuka di
    MobilePhone
  2. Dalam jumlah data yang terlalu banyak, aplikasi ini belum bisa
    digunakan.

<h2>Referensi :</h2>
Dalam mengerjakan laporan ini, tidak ditemukan bacaan yang membahas tentang aplikasi ini.
Maka, semua yang tertulis adalah hasil analisa kelompok kami terhadap aplikasi ini.

