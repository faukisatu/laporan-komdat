
RStudio Server
Sekilas Tentang	Instalasi	Cara Pemakaian	Pembahasan	Referensi
Sekilas Tentang
RStudio Server is a Linux server application that provides a web browser based interface to the version of R running on the server. RStudio Server is Web browser based IDE for R. RStudio Server enables you to provide a browser based interface to a version of R running on a remote Linux server, bringing the power and productivity of the RStudio IDE to server-based deployments of R.

Instalasi
System Requirement :
Ubuntu Server
R version 3.0.1 or higher.
Debian version 8 (or higher) or Ubuntu version 12.04 (or higher).
Proses instalasi :
Install VM Ubuntu Server and Setting port-forwarding VM. untuk penginstalan silahkan lihat disini.VM Ubuntu Server.

To obtain the latest R packages, add an entry like

deb https://<my.favorite.cran.mirror>/bin/linux/ubuntu xenial/
in your /etc/apt/sources.list file, replacing <my.favorite.cran.mirror> by the actual URL of your favorite CRAN mirror. To install the complete R system, use :

sudo apt-get update
sudo apt-get install r-base
Secure APT The Ubuntu archives on CRAN are signed with the key of “Michael Rutter marutter@gmail.com” with key ID E084DAB9. To add the key to your system with one command use (thanks to Brett Presnell for the tip):

sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9
An alternate method can be used by retrieving the key with.

gpg --keyserver keyserver.ubuntu.com --recv-key E084DAB9
and then feed it to apt-key with

gpg -a --export E084DAB9 | sudo apt-key add -
And the last install gdebi-core package, gdebi-core package is installed first so that gdebi can be used to install RStudio and all of its dependencies.

$ sudo apt-get install gdebi-core
$ wget https://download2.rstudio.org/rstudio-server-1.1.442-amd64.deb
$ sudo gdebi rstudio-server-1.1.442-amd64.deb    
Cara Pemakaian
Cara pemakaian RStudio Server ini sama seperti halnya RStudio biasa namun RStudio Server ini digunakan di web browser untuk menjalankannya. Untuk lebih jelas nya ini cara pemakaian nya

Setelah install semuanya, lalu kalian buka browser dan ketik localhost:8888. dan akan menampilkan sesuai foto di bawah ini.

Setelah kalian login, kalian akan menemukan tampilan awal RStudio Server seperti RStudio pada di desktop.

Selamat Menikmati RStudio Server nya.
Pembahasan
RStudio Server ini adalah Aplikasi RStudio yang dijalankan di web browser. Kelebihan dari RStudio Server ini adalah

The ability to access your R workspace from any computer in any location.
Easy sharing of code, data, and other files with colleagues.
Allowing multiple users to share access to the more powerful compute resources (memory, processors, etc.) available on a well-equipped server.
Centralized installation and configuration of R, R packages, TeX, and other supporting libraries.
Referensi
About RStudio Server.
About RStudio Server.
System requirement and how to install RStudio Server.
Advantages of RStudio Server.
