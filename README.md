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
