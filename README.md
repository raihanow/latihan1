# latihan1


# Tutorial Penggunaan Git

#

# Apa itu Git?

Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.
Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja
# Menambahkan Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user name dan user email
konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.
apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
Lakukan "git config --global user.name dan emal " supaya bisa login github ketika push
![1](https://user-images.githubusercontent.com/46749148/51843478-acc7c680-2345-11e9-8120-032769188397.jpg)

# Perintah Dasar Git

- **git init**: perintah untuk membuat repository local
- **git add**: perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
- **git commit**: perintah untuk menyimpan perubahan kedalam database git.
- **git push -u origin master**: perintah untuk mengirim perubahan pada repository local menuju server repository.
- **git clone [url]**: perintah untuk membuat working directory yang diambil dari repositry sever.
- **git remote add origin [url]**: perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)

# Membuat Repository Local

- Open gitbash, ketik cd /D
- Buat direktory project praktikum pertama dengan nama Latihan Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)
- direktory aktif menjadi: D/latihan1
- "latihan1" kemudian masuk ke direktory tersebut
![new](https://user-images.githubusercontent.com/46749148/51845162-8efc6080-2349-11e9-81d1-2590b92af067.jpg)

- Ketik "echo" untuk membuat file README.md 
- Lalu Lakukan "**git init**" untuk menjadikan repository lokal
![3](https://user-images.githubusercontent.com/46749148/51843929-a0903900-2346-11e9-8a45-8364d91d5582.jpg)

- kemudian tambahkan file tersebut ke repository dengan " **git add** README.md "
![4](https://user-images.githubusercontent.com/46749148/51844329-8c990700-2347-11e9-9292-aa6ac0677049.jpg)

- file yang berhasil ditambahkan akan terlihat seperti di gambar, dengan "ls -l"
![5](https://user-images.githubusercontent.com/46749148/51844382-b9e5b500-2347-11e9-8f4b-97212e51dc63.jpg)

- Untuk Menyimpan perubahan sebuah file ke repository local gunakan perintah  **git commit -m**  "Nama perintahnya"
![commit](https://user-images.githubusercontent.com/46749148/51844413-ca962b00-2347-11e9-9451-155bcb1d30db.jpg)


# Membuat Repository Server

- Server reopsitory yang akan kita gunakan adalah http://github.com
- Anda harus mempunyai akun terlebih dahulu.
<img width="960" alt="login" src="https://user-images.githubusercontent.com/46749148/51846100-82790780-234b-11e9-88a3-c031253ad9c4.png">

- Pada laman github, dari menu (icon +) klik New Repository
<img width="960" alt="new repository" src="https://user-images.githubusercontent.com/46749148/51846345-fe734f80-234b-11e9-82f4-09c59fd6833b.png">

- Isi nama repositorynya, misal: latihan1, lalu klik tombol Create repository
<img width="960" alt="repository" src="https://user-images.githubusercontent.com/46749148/51846531-5316ca80-234c-11e9-8969-b3d4b42e4327.png">


# Menambahkan Remote Repository

- Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
- Untuk menambahkan remote repository server, gunakan perintah **git remote add origin [url]**
![7](https://user-images.githubusercontent.com/46749148/51846799-e18b4c00-234c-11e9-86bf-658adf1fab5e.jpg)


# Push (Mengirim perubahan ke server)

- Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
- Gunakan printah **git push -u origin master**
![hh](https://user-images.githubusercontent.com/46749148/51848030-7000cd00-234f-11e9-81ef-2eb65702b079.jpg)

- Perintah ini akan meminta memasukkan username dan password pada akun github.com
![ll](https://user-images.githubusercontent.com/46749148/51847744-ea7d1d00-234e-11e9-8256-f772aa825b77.jpg)

- Proses push berhasil, maka akan muncul gambar seperti ini
![8](https://user-images.githubusercontent.com/46749148/51848383-11881e80-2350-11e9-8260-b21921c3a8d6.jpg)



# Melihat Hasil nya pada Repository

- Buka laman github.com, lalu refresh page.
- Maka perubahan akan terlihat pada laman tersebut.
<img width="960" alt="last" src="https://user-images.githubusercontent.com/46749148/51848471-3d0b0900-2350-11e9-8759-8871970aabb2.png">
