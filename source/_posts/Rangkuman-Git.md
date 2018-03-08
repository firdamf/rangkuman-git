---
title : GIT ALA - ALA 
---

> ***Hai, ini rangkuman mengenai kode 
atau perintah menggunakan Git tanpa ribet   ***

![](https://images.vogel.de/vogelonline/bdb/1286800/1286845/39.jpg)

---

#### 1. Buat Repositori Baru (create a new repository)

  Perintah untuk membuat repositori git baru:
  
* `get init` 

---

#### 2. Periksa Repositori (checkout a repository)

Perintah untuk membuat salinan kerja dari repositori lokal, dan untuk remote server gunakan perintah ini:
* `git clone / path / to / repository`  
* `git clone username @ host: / path / to / repository`

---

#### 3. Alur-Kerja (workflow)

[Repositori][1] lokal terdiri dari Working Directory(untuk menyimpan filenya),Index(pengolah datanya), dan HEAD(commit terakhirnya)

---

#### 4. Tambah dan commit (add & commit)

Untuk menambahkan/update ke index:
* `git add <filename>`
* `git add *`

Untuk memberi commit apa yang sudah di rubah diusahakan 
commit messagenya informatif perintahnya:
`git commit -m "Commit message"`

---

#### 5. Mengirim perubahan (pushing changes)

Perintah untuk me-remote mengirim perubahan:
* `git push origin master`  

Perintah untuk dihubungkan ke server jarak jauh
kalo [repositori][1]  nya belum dikloning:
* `git remote add origin <server>`

---

#### 6. Percabangan (branching)

Dalam membuat [repositori][1] , Branch master adalah branch utama dan ia bawaan, kita bisa membuat branch lain misalnya feature_x.

* `git checkout -b feature_x`  Untuk masuk ke branch feature_x 
* `git checkout master`  Untuk masuk ke branch master 
* `git push origin <cabang>` Untuk mengirim remote [repositori][1] 

---

#### 7. Perbarui & Gabung (update & merge)

Untuk update local [repositori][1]  dengan commit terbaru gunakan perintah:
* `git pull`
Untuk mengambil dan menggabungkan perubahan dengan remote:
* `git merge <branch>`
Untuk menggabungkan cabang lain ke cabang aktif:
* `git add <filename>`
Untuk melakukan pratinjau menggunakan:
* `git diff <source_branch> <target_branch>`

---

#### 8. Menandai (tagging)

Buat tag  dengan nama 1.0.0 dengan perintah:
* `git tag 1.0.0 1b2e1d63ff`

1b2e1d63ff adalah 10 karakter pertama dari identitas commit yang di referensikan ke tag.

---

#### 9. Log (log)

Perintah untuk melihat riwayat [repositori][1] 
* `git log`
Perintah untuk melihat komit
* `git log --author=bob`
Perintah untuk melihat compressed log  dalam commit 1 baris
* `git log --pretty=oneline`
Perintah untuk melihat ASCII art tree di semua branch yang didekorasi dengan nama tag dan branchnya
* `git log --graph --oneline --decorate --all`
Perintah untuk melihat file yang sudah diubah
* `git log --name-status`
Perintah untuk melihat lebih banyak parameter dalam git log
* `git log --help`

---

#### 10. Mengembalikan perubahan lokal (replace local changes)

Perintah untuk ke masa lalu jika ada yang ingin diubah
dengan konten terakhir dari HEAD :
* `git checkout -- <filename>`

Perubahan dan berkas baru yang ditambahkan ke indeks 
akan tetap tersimpan.

Perintah untuk menggagalkan perubahan dan komit lokal 
seutuhnya, ambil riwayat terakhir dari server dan arahkan
ke cabang master lokal: 
* `git fetch origin`
* `git reset --hard origin/master`

---

#### 11. Petunjuk berguna (useful hints)

    gitk
GUI git bawaan

    git config color.ui true
Menggunakan output git penuh warna

    git config format.pretty oneline
Menunjukkan log satu baris per komit

    git add -i
Menambah dengan interaktif

---

#### ***Lebih lengkapnya lihat disini***  [gitbook icip-icip](https://book.git-scm.com/)

---

[1]:https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository
















