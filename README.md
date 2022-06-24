# TUGAS BESAR Pemrograman Integratif 
**Andi Tadang Palie 1202190046 || IT 02-01**

<br />

-------

### Tahap 1 
### INSTALL PHP 

• Download php di website https://windows.php.net/download#php-8.1. Pilih file zip Thread Safe
![php](https://user-images.githubusercontent.com/93029648/175574574-9b0e2d6b-da49-4ce9-ad26-f5457bd25be0.PNG)


•	Ekstrak file php, kemudian copy di lokasi “ C:\Program Files “. Cari file bernama "php.ini development", buat salinan dan ubah nama file salinan menjadi  “php.ini”.     buka menggunakan text editor, dan jadikan seperti pada gambar, kemudian simpan.

![88](https://user-images.githubusercontent.com/93029648/175574870-1e2cd6ef-b724-4466-952d-2b894fd01bdb.PNG)


•	Buka “Edit The System Environment Variables”, klik Environment Variables

![99](https://user-images.githubusercontent.com/93029648/175574986-3cbb4e0b-50a7-444c-bde5-60a4899c9f7f.PNG)

•	Pilih variabel path untuk menambahkan alamat dari file php, kemudian pilih ok.

![100](https://user-images.githubusercontent.com/93029648/175575304-f21d10d5-9e0c-4951-9bdf-262c775366e1.PNG)

•	Buka terminal dan ketikkan ``php –v``, maka akan muncul tampilan seperti digambar, yang artinya php berhasil terinstall.

![101](https://user-images.githubusercontent.com/93029648/175575391-3f85ed8f-a531-48bc-9048-9f8be90d7ec1.PNG)

### INSTALL COMPOSER

•	Downlaod Composer https://getcomposer.org/download/

![1000](https://user-images.githubusercontent.com/93029648/175576104-7752f99a-09ac-4183-ba98-4aab03b50ea2.PNG)


•	Install file composer seperti biasa. Jika sudah buka terminal dan ketik “composer”, maka akan muncul tampilan seperti digambar, yang mana composer sudah terinstall.

![22](https://user-images.githubusercontent.com/93029648/175576179-a778f7ce-0b26-4a1a-a641-5adff1f11d6f.PNG)

### INSTALL LARAVEL VIA COMPOSER 

•	Buka website https://laravel.com/docs/9.x#installation-via-composer, untuk menyalin command installasi laravel via composer

•	Buat folder baru di komputer untuk menginstall laravel (bebas lokasinya). Klik kanan dan buka dengan Git Bash Here

•	Buat project untuk install laravel dengan command
 
```
composer create-project laravel/laravel nama_project
```

![33](https://user-images.githubusercontent.com/93029648/175576621-7d412f4d-b59b-4ee4-b9e5-00d0137ea156.PNG)
![44](https://user-images.githubusercontent.com/93029648/175576627-bc850b65-0c3b-416b-a9c1-1ccfa27535ea.PNG)


•	Masuk  terlebih dahulu ke folder project yang sudah dibuat dengan command
```
cd pintegratif/
```
• Kemudian buka file installasi laravel dengan text editor (disini dengan visual studio code) dengan command 
```
code ./pintegratif
```

• Maka akan secara otomatis membuka aplikasi visual studio code 
• Klik menu terminal pada bagian atas, pilih terminal baru, lalu masukkan command
```
php artisan serve
```

![77](https://user-images.githubusercontent.com/93029648/175577263-b599fd8b-87d7-4c5a-8bba-b2ed9e702c3d.PNG)


•	Copy server laravel, untuk dibuka di browser

![55](https://user-images.githubusercontent.com/93029648/175577347-850e32d5-276c-4937-bccd-ad00d125d08d.PNG)
