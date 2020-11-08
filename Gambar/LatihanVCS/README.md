# LatihanVCS

================Membuat Repository Lokal=====================

1. Pertama buka direktori aktif untuk membuat project git
2. klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
	sehingga muncul git bash command
![1-Membuka git bash command](https://user-images.githubusercontent.com/73067481/96444178-04a01280-1238-11eb-880b-c6c3aa25b471.png)
3. lalu buat direktori untuk project baru dengan perintah 
	mkdir LatihanVCS
4. lalu masuk ke direktori procect yang akan di buat dengan perintah
	cd LatihanVCS
    
![2-membuat direktori untuk project](https://user-images.githubusercontent.com/73067481/96444691-e686e200-1238-11eb-89f7-bd3f6e645454.JPG)
5. setelah itu jalankan perintah 
	git init
![3-membuat repository lokal](https://user-images.githubusercontent.com/73067481/96444849-336ab880-1239-11eb-9ba0-287017809692.JPG)
6. dengan terbentuknya satu direktori hidden dengan nama .git pada direktori tersebut, semua perubahan pada working directory
	akan disimpan.

================Menambahkan file baru ke repository=============	

1. buka text editor untuk membuat file, dan simpan filenya di direktori aktif(repository)
2. buat file bernama README.md(text file) dengan cara
   echo "# LatihanVCS">> README.md
3. Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah 
	git add README.md
![4-menambahkan file baru readme md](https://user-images.githubusercontent.com/73067481/96445311-e6d3ad00-1239-11eb-8b1e-2608134f613a.JPG)

===============Menyimpan Perubahan ke Database============
1. Untuk menyimpan perubahan yang ada kedalam database repository
   local, gunakan perintah
    git commit -m “Komentar Perubahan”
![5-membuat komentar update(perubahan)](https://user-images.githubusercontent.com/73067481/96445449-1b476900-123a-11eb-8e66-8b335dd5eb4a.JPG)

===============Membuat Repository Server==============
1. Server yang digunakan adalah http://github.com
2. Buat akun github
3. Pada laman github, klik tombol start a project, atau dari menu (icon +) klik New Repository
4. Isi nama repositorynya lalu klik tombol create repository
   
![6-membuat repository server](https://user-images.githubusercontent.com/73067481/96445753-9b6dce80-123a-11eb-9fc9-a7792ab51bb9.JPG)

==============Menambahkan Remote Repository==============

1. Remote Repository merupakan repository server yang akan
   digunakan untuk menyimpan setiap perubahan pada local repository,
   sehingga dapat diakses oleh banyak user. 
2. Untuk menambahkan remote repository server, gunakan perintah
    git remote add origin [url]
![7-menambahkan remote repository server pada  local repository ](https://user-images.githubusercontent.com/73067481/96446184-45e5f180-123b-11eb-85db-355015cdbd1a.JPG)


==============Mengirim Perubahan Ke Server=============

1. Untuk mengirim perubahan pada local repository ke server gunakan perintah git push dengan cara
    git push -u origin master
    
![8-mengirim perubahan ke repositori server](https://user-images.githubusercontent.com/73067481/96446243-5a29ee80-123b-11eb-9984-05f138b5aa70.JPG)

2. Perintah ini akan meminta memasukkan username dan password pada akun github.com
3. untuk melihat hasilnya buka laman github.com, arahkan pada repositorinya.

==============Clone Repository==============

1. clone repository, pada dasarnya adalah meng-copy repository server
   dan secara otomatis membuat satu direktory sesuai dengan nama
   repositorynya (working directory).Untuk melakukan cloning, gunakan perintah git clone [url]
![9-membuat working directory yang diambil dari repositry server](https://user-images.githubusercontent.com/73067481/96446315-73329f80-123b-11eb-9ff3-d19eda876acd.JPG)

