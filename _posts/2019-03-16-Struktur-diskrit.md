---
title: Struktur Diskrit 
updated: 2019-03-16 12:24
comments: true
---

## Daftar Isi

>Kata Pengantar iii
1 Pendahuluan 1
1.1 Apakah Matematika Diskrit itu? 
1.2 Mengapa Belajar Matematika Diskrit? 
1.3 Apa Isi Struktur Diskrit? 
2 Himpunan 5
2.1 Notasi Himpunan 
2.2 Keanggotaan Himpunan 
2.3 Diagram Venn 
2.4 Kesamaan Dua Himpunan 
2.5 Himpunan Berhingga dan Kardinalitas 
2.6 Himpunan Bagian dan Himpunan Kuasa 
2.7 Operasi Himpunan 
2.8 Sifat-sifat Operasi Himpunan 
2.9 Hasil Kali Himpunan 
3 Barisan 15
3.1 Barisan dan Himpunan 
3.2 Fungsi Karakteristik 
3.3 Representasi Himpunan 
4 Logika 19
4.1 Pernyataan (Proposisi) 
4.2 Pernyataan Bersyarat 
4.3 Inversi, Konversi, dan Kontraposisi 
4.4 Ekivalensi Logis dan Tautologi 
4.5 Sifat-sifat Operasi Pernyataan 
4.6 Pernyataan Berkuantor 
4.7 Argumentasi Logis 
4.8 Operasi Bit pada Komputer 
5 Teknik Membilang 35
5.1 Prinsip Perkalian 
5.2 Prinsip Sarang Merpati 
5.3 Permutasi 
5.4 Kombinasi 
6 Fungsi 41
6.1 Fungsi Kebalikan .
6.2 Komposisi Fungsi 
7 Relasi 45
7.1 Representasi Relasi 
8 Pengantar Teori Graf 49
9 Pohon 51
10 Bilangan Bulat 53
10.1 Pendahuluan 
10.2 Aksioma Bilangan Bulat 
10.3 Sifat-sifat Bilangan Bulat 
10.4 Latihan .
11 Induksi Matematika 59
11.1 Induksi Matematika 
11.2 Latihan 
12 Matriks 63
13 Aljabar Bool 65


## Bab 1

**Pendahuluan**

1.1 Apakah Matematika Diskrit itu?

Matematika diskrit adalah bagian dari matematika yang mempelajari objek-
objek diskrit. Di sini objek-objek diskrit diartikan sebagai objek-objek yang
berbeda dan saling lepas. Matematika diskrit memiliki aplikasi di hampir
semua bidang kehidupan, seperti ilmu komputer, kimia, botani, zoologi, lin-
guistik, geogra¯, dan bisnis. Masalah-masalah seperti

* Ada berapa cara membuat password untuk sebuah sistem komputer?
* Bagaimana mengurutkan sebuah himpunan bilangan bulat dari terkecil
hingga terbesar?
* Berapa besar peluang memenangkan sebuah undian?
* Bagaimana menemukan lintasan terpendek antara dua kota dengan
angkutan umum?

merupakan contoh kajian dalam matematika diskrit. Secara lebih umum,
matematika diskrit digunakan untuk
* menghitung banyak objek
* mempelajari hubungan antara himpunan-himpunan berhingga
* menganalisis proses yang melibatkan langkah-langkah yang banyaknya berhingga

Lima tema dalam matematika diskrit berikut tujuan masing-masing adalah
1. Penalaran matematika: memberikan pemahaman tentang penalaran
matematika dalam membaca, memahami, dan membangun argumen
matematika.
2. Analisis kombinatorial: memberikan keterampilan menghitung banyak
objek sebagai salah satu kemampuan dasar untuk memecahkan masalah.
3. Struktur diskrit: memberikan pemahaman tentang struktur diskrit se-
bagai salah satu struktur matematika abstrak yang digunakan untuk
menyajikan objek-objek diskrit dan hubungan di antara objek-objek
itu.
4. Aplikasi dan Pemodelan: memperkenalkan aplikasi matematika diskrit
dan pemodelan matematika sebagai salah satu kemampuan pemecahan
masalah yang sangat penting.
5. Berpikir algoritmik: memberikan kemampuan membuat algoritma dan
veri¯kasinya serta menganalisis memori komputer dan waktu yang dibu-
tuhkan untuk melakukan algoritma itu.

## 1.2 Mengapa Belajar Matematika Diskrit?

Beberapa alasan penting belajar matematika diskrit adalah sebagai berikut:

1. matematika diskrit memberikan kemampuan membaca, memahami dan
membangun argumen matematika.

2. matematika diskrit merupakan pintu gerbang untuk mempelajari mata
kuliah lanjutan dalam logika, teori himpunan, teori bilangan, aljabar
linier, aljabar abstrak, kombinatorika, teori graf,dan teori peluang.

3. matematika diskrit memberikan landasan matematika untuk mata ku-
liah ilmu komputer seperti struktur data, algoritma, teori basis data,
teori automata, keamanan komputer (computer security), dan sistem
operasi.

4. matematika diskrit memberikan latar belakang matematika yang diper-
lukan dalam pemecahan masalah riset operasi (operations research)
seperti teknik optimisasi diskrit.

## 1.3 Apa Isi Struktur Diskrit?

Struktur diskrit mempelajari struktur matematika yang memiliki objek atau
elemen diskrit. Struktur atau sistem matematika dide¯nisikan sebagai kolek-
si objek dengan operasi yang terde¯nisi pada objek itu serta sifat-sifatnya.
Struktur diskrit berisi pokok bahasan: Himpunan, Barisan, Fungsi, Logika,
Teknik Membilang (counting techniques), Relasi, Graf, dan Pohon.


## Bab 2

### Himpunan

#### 2.1 Notasi Himpunan

Himpunan adalah koleksi objek yang terde¯nisi dengan jelas; artinya, kita
selalu dapat menentukan apakah sebuah objek termasuk dalam koleksi atau
tidak.
Nama himpunan ditulis dengan menggunakan huruf besar
A;B;H; S; U; : : : ;
sedangkan anggota himpunan ditulis dengan huruf kecil
a; b; h; s; u; : : : :

Contoh 2.1. Beberapa contoh himpunan.
1. A adalah himpunan bilangan asli yang kurang dari 10.
2. B adalah himpunan huruf hidup dalam abjad bahasa Indonesia.
3. C adalah himpunan kuadrat bilangan asli.
4. K adalah himpunan mahasiswa yang memiliki IPK lebih dari 3.
5. M adalah himpunan mahasiswa Universitas Sriwijaya.

2.2 Keanggotaan Himpunan
Untuk menyatakan bahwa sebuah objek a adalah anggota sebuah himpunan
A kita menggunakan notasi
a 2 A:

Sedangkan notasi
a =2 A
berarti a bukan anggota himpunan A.
Contoh 2.2. Jika A dan B adalah himpunan-himpunan pada Contoh 2.1,
maka 2 2 A; 10 =2 A; a =2 A; b =2 B; i 2 B; 3 =2 B.
Himpunan dari semua objek pembicaraan disebut himpunan semesta dan
biasanya dilambangkan dengan U. Sedangkan himpunan yang tidak mem-
punyai anggota disebut himpunan kosong dengan notasi ;.
Contoh 2.3. U = N, himpunan semua bilangan asli.
Contoh 2.4. Himpunan bilangan ganjil yang habis dibagi dua adalah him-
punan kosong.
Ada dua cara untuk menuliskan anggota sebuah himpunan. Cara pertama
adalah dengan menuliskan atau mendaftarkan semua anggota himpunan itu.
Contoh 2.5. Himpunan A, B, dan C pada Contoh 2.1 dapat ditulis sebagai

>A = f1; 2; 3; 4; 5; 6; 7; 8; 9g
>B = fa; i; u; e; og
>C = f1; 4; 9; 16; 25; : : :g

Perhatikan bahwa pada penulisan ini anggota himpunan dipisahkan oleh ko-
ma dan diapit oleh kurung kurawal. Tiga titik dalam himpunan C boleh
dibaca dan seterusnya, yang berarti masih banyak anggota lain. Kesulitan
akan timbul bila anggota himpunan sangat banyak, seperti himpunan M pa-
da Contoh 2.1.
Cara kedua adalah dengan menggunakan notasi pembangun him-
punan, yaitu membuat diskripsi mengenai sifat-sifat anggota himpunan
yang bersangkutan.
Contoh 2.6. Himpunan-himpunan pada Contoh 2.1 dapat ditulis sebagai

>A = fx j x < 10; x 2 Ng
>B = fx j x adalah huruf hidup dalam abjad bahasa Indonesiag
>C = fx2 j x 2 Ng
>K = fx j x adalah mahasiswa yang memiliki IPK lebih dari 3g
>M = fx j x adalah himpunan mahasiswa Universitas Sriwijayag

Dalam bahasa Inggris tanda "j" dibaca "where". Dalam bahasa Indonesia
tanda ini bisa dibaca "di mana" walaupun menurut kaidah bahasa Indonesia
hal ini kurang tepat.

## 2.3 Diagram Venn

Himpunan dapat digambarkan dengan diagram Venn. Dalam diagram ini
himpunan semesta digambarkan sebagai empat persegi panjang sedangkan
himpunan-himpunan di dalamnya digambarkan sebagai lingkaran atau ben-
tuk geometri lain. Anggota himpunan biasanya dinyatakan sebagai titik.

Gambar 2.1 menyajikan beberapa contoh diagram Venn.
![diagram venn](/assets/DV.png)

## 2.4 Kesamaan Dua Himpunan

Dua himpunan A dan himpuan B dikatakan sama, yaitu
A = B
bila kedua himpunan itu memiliki anggota yang persis sama. Dengan kata
lain, setiap anggota A adalah anggota B dan setiap anggota B adalah juga
anggota A.

>Contoh 2.7. Misalkan S = f1; 3; 5g dan T = f5; 1; 3g. Meskipun anggota
himpunan S dan T ditulis dalam urutan yang berbeda, S = T.

## 2.5 Himpunan Berhingga dan Kardinalitas

Himpunan dengan anggota yang banyaknya berhingga seperti himpunan A
dan B pada Contoh 2.5 disebut himpunan berhingga. Banyak anggota
sebuah himpunan berhingga disebut kardinalitas. Notasi n(A) atau jAj di-
gunakan untuk menyatakan kardinalitas himpunan A. Pada Contoh 2.5,
n(A) = 9 dan n(B) = 5. Sedangkan himpunan dengan anggota yang
banyaknya tak hingga seperti himpunan C pada Contoh 2.5 disebut him-
punan tak hingga.



># Konten akan terus bertambah sesuai Daftar Isi !
