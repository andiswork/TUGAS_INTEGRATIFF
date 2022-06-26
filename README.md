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

<br />

------
### Tahap 2
•	Ubah DB_DATABASE di .env sesuai dengan nama database yang dibuat di phpmyadmin

![Screenshot (118)](https://user-images.githubusercontent.com/93029648/175824987-6464af74-f46d-42a4-a723-ca06e2ee40c6.png)


• Buat 2 table rss dan news dengan fitur migrations menggunakan perintah
  ```
  php artisan make:migration create_rss_table
  
  php artisan make:migration create_news_table
  ```
• Tambahkan kolom name dan url pada tabel rss, seperti pada gambar dibawah

![integ 1](https://user-images.githubusercontent.com/93029648/175825459-d55bf31e-7889-45af-a401-a3281651d8c6.PNG)


• Tambahkan kolom title, img_url, description, source_url,  dan rss_id pada tabel news, seperti pada gambar dibawah


• Untuk menjalankan migrasi yang dibuat jalankan perintah diterminal seperti dibawah, lalu cek database

 ```
  php artisan migrate
  ```
  
  ![Screenshot (121)](https://user-images.githubusercontent.com/93029648/175825477-d7200991-1e2c-4369-8258-e67367b25731.png)

  
  
 • Buat koneksi  model  ke database  dengan membuat seeder dan controller untuk tabel Rss dan News, dengan perintah
 ```
  php artisan make:model Rss –seed –controller
  ```
 
![Screenshot (122)](https://user-images.githubusercontent.com/93029648/175825941-bc81053b-f784-4d35-9298-e29f916c420f.png)

• Edit file Rss.php, RssSeeder.php serta DatabaseSeeder.php seperti pada gambar dibawah
![Screenshot (123)](https://user-images.githubusercontent.com/93029648/175825981-34c54e85-8fd0-4bf7-ae78-466e14ff0929.png)
![Screenshot (124)](https://user-images.githubusercontent.com/93029648/175825984-5dd5f2d5-14d9-4516-a66a-7c0104173b53.png)
![Screenshot (125)](https://user-images.githubusercontent.com/93029648/175825985-b0601406-4309-4d8e-908e-9acda1bed2ef.png)


• Kemudian cek koneksi dengan perintah
```
  php artisan db:seed
  ```
  ![Screenshot (126)](https://user-images.githubusercontent.com/93029648/175826084-aab7b61a-4575-4127-bd50-75a0ca39d468.png)

• Edit file News.php, NewsController.php, web.php, serta file migration News seperti pada gambar dibawah

  ![Screenshot (129)](https://user-images.githubusercontent.com/93029648/175826463-98f54d26-c4d4-4f3c-82a2-4065578d12c9.png)

![Screenshot (142)](https://user-images.githubusercontent.com/93029648/175826546-2ec6edf0-e489-48e0-8b50-ac8a1e407657.png)

![Screenshot (143)](https://user-images.githubusercontent.com/93029648/175826568-a391c089-7179-457e-8790-a64cbd381e53.png)


• Cek localhost di http://127.0.0.1:8000/aggregrate/2 dan di database phpmyadmin
  ![Screenshot (138)](https://user-images.githubusercontent.com/93029648/175826611-cefd5184-9fef-4a7f-a115-3978df637189.png)
![Screenshot (137)](https://user-images.githubusercontent.com/93029648/175826618-916114df-514c-4d10-876c-b2ef4563a17f.png)

  • Cek localhost di http://127.0.0.1:8000/aggregrate/4 dan di database phpmyadmin
  ![Screenshot (140)](https://user-images.githubusercontent.com/93029648/175826709-5211b821-87d9-41e9-8183-d39b1a0a40bc.png)

  ![Screenshot (144)](https://user-images.githubusercontent.com/93029648/175826739-f461f970-2d2a-4c2d-94bd-e10c4c2ce5b2.png)

• Cek localhost di http://127.0.0.1:8000/aggregrate/5 dan di database phpmyadmin

![Screenshot (141)](https://user-images.githubusercontent.com/93029648/175826751-0a7a7ef0-df76-4a0c-b3df-905d05d536c1.png)


![Screenshot (144)](https://user-images.githubusercontent.com/93029648/175826760-397e445b-586e-446e-9224-2fc0ae6be646.png)

