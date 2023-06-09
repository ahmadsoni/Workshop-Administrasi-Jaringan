
Nama : Arga Rafi I.M

Kelas : 2D4ITA

NRP : 3121600010
# Laporan Tugas
### 1. Identifikasi kernel
Kernel pada sistem operasi Linux atau Unix yang berfungsi untuk mengelola sumber daya komputer, seperti memori, prosesor, dan perangkat keras lainnya. Kernel berperan sebagai perantara antara aplikasi dan perangkat keras. Untuk menampilkan informasi tentang sistem, digunakan perintah “uname -a” yang menampilkan semua informasi seperti nama host, versi kernel, arsitektur sistem, platform sistem operasi, tanggal dan waktu kompilasi kernel, dan lain-lain. Sedangkan perintah “uname -r” hanya menampilkan nomor versi kernel yang sedang berjalan pada sistem.

![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.001.png)

**Penjelasan kernel:**
Dalam versi kernel saya 5.15.0-60, ini menunjukkan versi kernel Ubuntu yang digunakan. Versi kernel ini adalah 5.15.0-60, di mana:
5 adalah nomor utama kernel, yang menunjukkan bahwa ini adalah kernel 5.
15 adalah nomor minor kernel, yang menunjukkan bahwa ini adalah kernel seri 19 dari seri 5.
0 adalah nomor revisi kernel, yang menunjukkan bahwa ini adalah build ke-0
### 2. Identifikasi Directory
- /usr: Menyimpan program dan data terkait pengguna.
- /bin: Menyimpan file biner eksekusi yang dapat diakses oleh semua pengguna.
- /sbin: Menyimpan file biner eksekusi yang hanya dapat diakses oleh super user.
- /root: Menyimpan file konfigurasi, skrip shell, dan data terkait pengguna root.
- /home: Menyimpan semua file dan data pribadi pengguna, seperti dokumen, gambar, musik, dan video.
- /var: Menyimpan data volatil yang berubah-ubah, seperti log sistem.
- /tmp: Menyimpan data sementara.
- /etc: Menyimpan konfigurasi sistem.
- /opt: Menyimpan aplikasi opsional.
- /mnt digunakan untuk memuat sistem file dari file sistem lain.

Directory structur

![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.002.png)


### 3. Identifikasi perbedaan sudo dan su
"su" digunakan untuk beralih ke akun pengguna lain atau akun superuser dengan memasukkan kata sandi yang sesuai. "sudo", di sisi lain, memungkinkan pengguna untuk menjalankan perintah tertentu sebagai akun superuser atau akun lain tanpa perlu masuk ke dalam akun superuser secara langsung.

Dalam penggunaan "su", pengguna harus memasukkan kata sandi untuk akun superuser atau akun lain yang dituju. Namun, dalam penggunaan "sudo", pengguna diminta untuk memasukkan kata sandi mereka sendiri untuk memverifikasi identitas mereka sebelum menjalankan perintah.

Perintah "sudo su" dapat digunakan untuk beralih ke akun superuser, dan "sudo su -" akan mengubah direktori saat ini ke direktori home akun superuser.

![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.003.png)





nano /etc/sudoers.tmp

![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.004.png)

### 4. Identifikasi jenis repositori
Ini adalah file sources.list Ubuntu yang berisi beberapa jenis repository. Berikut adalah identifikasi jenis repository berdasarkan baris yang dimulai dengan "deb" :

Pertama, ada "deb cdrom:" yang merupakan repository untuk CD/DVD instalasi Ubuntu.

Kemudian, terdapat repository utama Ubuntu yaitu "deb http://id.archive.ubuntu.com/ubuntu/ kinetic main restricted" yang berisi paket-paket utama untuk sistem operasi Ubuntu.

Selanjutnya, ada repository "deb http://id.archive.ubuntu.com/ubuntu/ kinetic-updates main restricted" yang berfungsi untuk pembaruan (updates) dari paket-paket di repository utama.

Repository "deb http://id.archive.ubuntu.com/ubuntu/ kinetic universe" berisi paket-paket yang tidak disupport secara resmi oleh Ubuntu, namun tetap terbuka untuk diakses oleh pengguna.

Kemudian, ada beberapa repository untuk pembaruan keamanan (security) dari paket-paket di repository utama, universe, dan multiverse, yaitu

"deb http://security.ubuntu.com/ubuntu kinetic-security multiverse",

"deb http://security.ubuntu.com/ubuntu kinetic-security universe", dan

"deb http://security.ubuntu.com/ubuntu kinetic-security main restricted".

![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.005.png)

### 5. Identifikasi perintah apt
![](Aspose.Words.0a6556e4-ba0f-42f0-ba5a-02a076f57f26.006.png)

list - menampilkan daftar paket berdasarkan nama paket

search - mencari dalam deskripsi paket

show - menampilkan detail paket

install - menginstall paket

reinstall - menginstall ulang paket

remove - menghapus paket

autoremove - menghapus otomatis semua paket yang tidak terpakai

update - memperbarui daftar paket yang tersedia

upgrade - mengupgrade sistem dengan menginstal/mengupgrade paket-paket

full-upgrade - mengupgrade sistem dengan menghapus/menginstal/mengupgrade paket-paket

edit-sources - mengedit file informasi sumber

satisfy - memenuhi string dependensi

apt update : Memperbarui daftar paket dan metadata yang tersedia di repository.

apt upgrade : Menginstall paket-paket baru yang tersedia dan mengupgrade paket yang sudah terinstall.

apt install : Menginstall paket baru.

apt remove : Menghapus paket yang sudah terinstall.

apt autoremove : Menghapus paket-paket yang tidak lagi dibutuhkan oleh sistem.

apt search : Mencari paket yang tersedia di repository.

apt show : Menampilkan informasi detail tentang paket yang tersedia di repository.

apt list : Menampilkan daftar paket yang sudah terinstall.

apt full-upgrade : Menginstall paket-paket baru dan mengupgrade paket-paket yang sudah terinstall dengan menyelesaikan semua ketergantungan (dependencies) yang dibutuhkan.






