# Instalasi Git bash
 0468b79b710184402821aa39dad631691090ffca
1. Buka browser dan ketikan **git csm** 
![](Assets/instal_1.PNG)

2. Tampilan akan seperti gambar di bawah. Setelah itu klik **Download for Windows** karena di sini saya menggunakan sistem operasi *Windows* 

![](Assets/instal_2.PNG)


---
Sesudah di downloaad, next ke semua arahan dari file **.exe** nya

3. Setelah terinstal, buka *gitbash* dan cek versi git di laptop kalian

![](Assets/git_version.PNG)

> Perintah ini berguna untuk memeriksa versi Git yang Anda gunakan, yang dapat bermanfaat dalam mengidentifikasi dan mengatasi masalah kompatibilitas.

# Buat repository di gituhub
Untuk membuat repository baru di GitHub, ikuti langkah-langkah berikut.

1. Pastikan anda sudah memiliki akun **github** dan login ke dalam **github**...
2. Klik ikon di pojok kanan (ketiga dari kanan), dan klik **New Depository

![](Assets/New_repository.PNG)

3. Tampilan selanjutnya akan seperti in, dan isi kolom **Repositoy name** sesuai keinginan
![](Assets/New_repository2.PNG)

Sebagai Contoh : 
![](Assets/New_Repository2.PNG)

![](Assets/New_repository3.PNG)


4. Setelah semuanya siap, langsung klik **Create repository** di bawah 
![](Assets/New_repository4.PNG)

5. Selanjutnya kita di arahkan ke tampilan Repository baru 
![](Assets/New_repository5.PNG)
>Nah sekarang kita sudah berhasil menambahkan repository baru. Langkah selanutya mari kita konfigurasikan username dan email kita di GitHub...
# Konfigurasi awal di git bash (config)

1. git config --list
Perintah `git config --list` digunakan untuk menampilkan konfigurasi Git yang saat ini aktif pada sistem Anda.

- **`git config`**: Perintah ini digunakan untuk membaca dan mengubah konfigurasi Git. Konfigurasi ini mencakup pengaturan seperti nama pengguna, email, dan preferensi Git lainnya.
- **`--list`**: Opsi ini digunakan untuk menampilkan semua pengaturan konfigurasi yang saat ini berlaku, baik dari file konfigurasi global, lokal, maupun sistem.

2. atur konfigurasi email dan username

Untuk mengatur konfigurasi username dan email yang tujuannya untuk mengkoneksikan 
kita bisa mengetik code seperti berikut : 

```bash
git config --global user.name "nama_username"
git config --global user.email "email_kita"
```

Sebagai Contoh : 

![](Assets/config.PNG)

3. Untuk melihat apakah konfigurasi nya sudah berhasil, ketik : 
```bash
git config --list
```

Sebagai Contoh : 
![](Assets/config2.PNG)

Setelah mengatur konfigurasi username dan email kita, kita gunakan kembali perintah `git config --list`. Untuk menampilkan seluruh pengaturan konfigurasi dan mengecek apakah konfigurasi yang sebelumnhya sudah berlaku atau belum...

> Selanjutnya, mari kita akses folder lokal kita diGitBash...
# Akses Folder proyek di git bash
gunakan perintah cd sampai ke direktori

1. Gunakan perintah `cd` 
Untuk mengakses folder proyek di Git Bash menggunakan perintah `cd`, Anda akan mengikuti langkah-langkah yang mirip dengan cara Anda mengakses folder di Command Prompt Windows.

berikut code penerapan : 
```bash
cd "nama_folder"
```

Contoh penepan dalam **gitbash** : 

![](Assets/cd.PNG)

Jika perlu, setiap kita mengganti direktori. Saya ingin memperkenalkan perintah `ls`, dalam git yang berfungsi untuk melampirkan/menampilkan isi dari direktori (membuka jalan menuju folder proyek kita).
	Nah di sini saya sudah tau kemana arah folder proyek saya, kita bisa menggunakan perintah sebagai berikut : 
	
```bash
cd "nama_folder/nama_folder dst..."
```

Contoh penerapan dalam **gitbash** : 

![](Assets/cd2.PNG)

> Nah sekarang saya sudah berhasil mengakses folder proyek saya di **git**...

Contoh di atas bertujuan menuju ke folder proyek kita dengan sekali jalan, tanpa harus setiap kali memakai perintah `ls` untuk melihat kemana kita selanjutnya.

> Nice, kita sudah akses folder/file kita. Selanjutnya mari kita hubufnkan ke GitHub...

# Menghubungkan folder proyek lokal ke github

Untuk memudahkan pengelolaan versi dan kolaborasi, Anda dapat menghubungkan folder proyek lokal Anda ke GitHub. Berikut adalah langkah-langkah sederhana untuk menginisialisasi repository lokal, menghubungkannya dengan GitHub

Berikut adalah langkah langkah **menghubungkan folder proyek kita ke github**

1. Instalasi repository, ketik code sebagai berikut : 

```bash
git init
```

Contoh : 

![](Assets/git_init.PNG)


> Contoh di atas menyatakan bahwa perintah `git init` **memulai repository Git** di dalam folder proyek lokal. Dengan kata lain, perintah `git init` merupakan langkah awal dalam proses pembuatan dan pengaturan repository Git di komputer Anda.

2. Hubungkan ke repository 

Untuk menghubungkan file lokal kita ke repository, lita mesti menggunakan code `git remote origin` yang
digunakan untuk mengelola repositori jarak jauh (remote repositories) yang terhubung dengan repositori lokal Anda. Salah satu aspek penting dalam pengelolaan remote adalah `origin`, yang merupakan nama standar untuk remote utama saat pertama kali Anda menghubungkan repositori lokal Anda dengan repositori jarak jauh.

ketik code seperti berikut : 
```bash
git remote add origin
```

Contoh : 

![](Assets/remote_origin.PNG)

Jadi, Menggunakan `git remote` dengan `origin` memungkinkan Anda untuk mengelola bagaimana dan di mana kode Anda disinkronkan dan dibagikan dengan repositori jarak jauh.

3. Tambahkan file atau perubahan pada depository 
Untuk memodifikasi isi dari depository, maka digunakan perintah `git add .` yang mana dalam Git  berfungsi untuk menambahkan perubahan pada file di direktori

berikut penulisan code : 
```bash
git add .
```

Contoh penerapan : 

![](Assets/git_add.PNG)

Dalam contoh di atas merupakan persiapan untuk perubahan sebelum kita menginput atau menyimpannya di dalam **commit**

4. Tambah pesan dan menyimpannya ke dalam **commit**

Dalam konteks perintah `git commit -m`, istilah "disertakan dalam opsi `-m`" merujuk pada cara Anda memberikan pesan commit secara langsung melalui opsi `-m` di baris perintah.

Berikut code penerapan : 
```bash
git commit -m
```

Contoh penerapan dalam **git** : 

![](Assets/git_commit.PNG)

Contoh di atas menyatakan perintah:
- **`git commit`**: Perintah ini menyimpan isi dari perubahan yang ada ke dalam riwayat commit repositori Git. Commit ini mencatat perubahan yang telah dibuat dan memberikan konteks untuk perubahan tersebut.

-  **`-m "Awal_belajar"`**: Opsi `-m` diikuti dengan pesan dalam tanda kutip adalah cara untuk langsung menyertakan pesan commit saat menjalankan perintah `git commit`. Pesan ini memberikan deskripsi singkat tentang perubahan yang telah Anda buat.

-  **`-m "Baru_pertama"`**: Opsi `-m` diikuti dengan pesan dalam tanda kutip adalah cara untuk langsung menyertakan pesan commit saat menjalankan perintah `git commit`. Pesan ini memberikan deskripsi singkat tentang perubahan yang telah Anda buat.

Jadi, perintah `git commit -m` ini berfungsi untuk memungkinkan Anda untuk **menyertakan pesan commit secara langsung** di baris perintah.

5.  Unggah semua perubahan yang sudah di modifikasi sebelumnya

digunakan untuk mengirimkan perubahan yang telah Anda commit di repositori lokal ke repositori jarak jauh (remote repository). 

berikut perintah penerapannya : 
```bash
git push origin
```

Contoh penerapan dalam **git** : 
![](Assets/git_push.PNG)

Singkatnya, perintah `git push origin` ini berfungsi untuk memungkinkan Anda untuk membagikan  atau mengirim perubahan yang sudah di modifikasi.

6. Login ke akun github 
Setelah kita selesai memodifikasi perubahan pada direktori, kita login ke akun **github** kita dan langsung masuk ke dalam depository untuk melihat, apakah sudah terubah/termodifikasi depository kita...

- Sebelum termodifikasi : 
![](Assets/New_repository5.PNG)

- Sesudah termodifikasi : 

![](Assets/New_repository6.PNG)

> Nah saya sudah berhasil memodifikasi isi depository saya di **github**, ada 1 commit yang sudah kita tambahkan sebelumnya...


