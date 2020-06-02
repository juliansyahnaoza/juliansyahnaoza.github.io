​	Bourne Again Shell yang lebih sering kita sebut Bash, Bash ini merupakan salah satu program dalam GNU Project yang menjadi Shell yang paling banyak digunakan. Bash merupakan pengembangan Bourne Shell, namanya juga ambil dari penciptanya yaitu Stephen Bourne. Kemudian Bash dikembangkan oleh Brian Fox.

​	Primer pada sistem Linux dan juga disertakan pula di OS X Tiger yang sekarang disebut Mac OS. Bash juga memiliki bahasa programman yang baik serta interaktivitas yang mudah dipahami. Selain Bash, Shell yang ada ialah C-Shell dan Korn Shell. Perbedaan ketiganya terlihat pada format penyimpanan, yaitu bash(.sh), C-Shell(.ch), dan korn (.ksh).code

​	Yaitu menyusun atau mengelompokkan beberapa perintah shell (internal atupun eksternal command) menjadi kumpulan perintah yang melakukan tugas tertentu sesuai tujuan penyusunnya. Kelebihan shell di linux dibanding sistem operasi lain adalah bahwa shell di linux memungkinkan kita untuk menyusun serangkaian perintah seperti halnya bahasa pemrograman (interpreter language), melakukan proses I/O, menyeleksi kondisi, looping, membuat fungsi, dsb. adalah proses - proses yang umumnya dilakukan oleh suatu bahasa pemrograman, jadi dengan shell di linux kita dapat membuat program seperti halnya bahasa pemrograman, untuk pemrograman shell pemakai unix atau linux menyebutnya sebagai script shell.

### A. Seleksi IF

​      **Codelabs IF**

1. Buka terminal atau code editor anda,
2. ketikan command/perintah `vim namafile.sh` pada terminal anda, jika menggunkan code editor atau online shell scripting compiler makna cukup membuat skrip shell seperti anda membuat file text biasa pada notepad atau code editor anda, kemudian simpan dengan berekstensikan `.sh`pada akhir nama file shell anda .
3. kareana kita akan membuat pengkondisian pada if pada shellscripting berikut sourcode nya dibawah ini:

```shell
#!/bin/bash

clear
echo "DAFTAR SEMBAKO";
echo "-------------------------";
echo "1. Beras 5kg @Rp. 70.000";
echo "2. Minyak goreng 1 liter @Rp. 20.000";
echo "3. Gula 1 kg @Rp. 12.000";
echo "4. Garam Dapur @Rp. 3.000";
echo "5. Telur 12butir @Rp. 24.000";
echo "0. exit";

read -p "Barang anda [1-5] :" pil;

if [ $pil -eq 1];
	then
	echo "Banyak barang =";
	read jum
	let bayar=jum*70000;
elif [[ $pil -eq 2 ]]; 
	then
		echo "Banyak barang=";
		read jum
		let bayar=jum*20000;
	elif [[ $pil -eq 3 ]]; 
		then
		    echo "Banyak barang";
		    read jum
		    let bayar=jum*12000;
		elif [[ $pil -eq 4 ]]; 
			then
		echo "Banyak barang";
		read jum
		let bayar=jum*3000;
	elif [[ $pil -eq 5 ]]; 
		then
		echo "Banyak barang";
		read jum
		let bayar=jum*24000;
	elif [[ $pil -eq 6 ]]; 
		then
			exit 0
		else 
			echo "SORRY, TIDAK ADA BARANG";
			exit 1
		fi
		echo "Harga bayar = Rp. $bayar"
		echo "THX"
			#statements
			#statements


```

4. Saat anda telah memasukan skrip shell  dan membuka di terminal linux anda maka tampilanya sepeti dibawah ini: 

   ![](\assets\codelab_if.png)

#### output IF

1. Untuk menjalankan atau mengeksekusi file shell anda diterminal pastikan anda berada di direktori yang sama dengan dimana file shell anda disimpan.

2. kemudian ketikankan perintah `./nama_file.sh` kemudian enter, makan akan keluar seperti tampilan seperti pada gambar dibawah ini:

   ![](\assets\hasil_if.jpg)







## B. Membuat Window sedehana dengan fungsi `box();`

Di Programman Linux sangat dikenal pustaka/Library **ncurses**, ncurses adalah pustaka programman yang menyediakan antarmuka programman aprlikasi (API) yang memungkinkan programmer untuk menulis antarmuka pengguna (UI) berbasis teks dengan cara yang bebas terminal. Ini adalah toolkit(perlengkapan) untuk mengembangkan perangkat lunak aplikasi mirip GUI yang berjalan dibawah terminal.

#### Codelabs `box();`

1. Install linux pada perangkat komputer/laptop anda, atau gunakan Virtual Mechine. disini saya menggunkan linux dari salahsatu distro linux terkenal yaitu Ubuntu dan disini saya menggukan ubuntu dengan WSL (Windows Subsystem for Linux). 

2. Pastikan komputer/laptop terhubung ke internet agar bisa melakukan update package yang dibutuhkan untuk tugas ke repository ubuntu. Untuk melakukan Update package di ubuntu lakukan cara dinomor selanjutnya,

3. buka terminal pada ubuntu, login sebagi root atau SuperUser(SU) dengan mengetikan command(perintah) `apt-get update`

4. setelah itu instal pustaka/library **ncurses** dengan command/perintah `sudo apt-get install libncurses5-dev libncursesw5-dev`

5. setelah berhasil selesai menginstall library ncurses, bikin folder baru utk proyek baru dgn mengetikan command `mkdir namaFolder . `utk melihat folder yg baru dibikin ketikan printah `ls` artinya daftar file/folder yg ada di direktori yg sama. 

6. bikin file untuk membuat project baru dengan peintah `vim nama_file.cpp`, setelah jadi dan terbuka tekan tombol **insert** pada keyboard anda utk bisa menulis code, tekan tombol insert jika selesai menulis code sampai berubah dibagian bawah menjadi REPLACE kemudian tekan tombol esc pada keyboard hingga hilang tulisan REPLACE kemudian ketik sebagai berikut:

   **Penting**

   *- **Esc** tombol yang sangat penting utk keluar dari mode text didalam vim*

   *- **:q** (ya) untuk keluar editor(vim)*

   *- **:q!**  untuk keluar vim tanpa menyimpan data file*

   *- **:wq** untuk menyimpan file dan keluar exit*

7. berikut source code simple with box() function

```c++
#include <ncurses.h>
using namespace std;

int main(int argc, char ** argv)
{
        initscr();
        int height, width, start_y, start_x;
        height = 10;
        width = 20;
        start_y = start_x = 10;

        WINDOW * win = newwin(height, width, start_y, start_x);
        refresh();

        box(win, 0, 0);
        mvwprintw(win, 1, 1, "Naoza");
        wrefresh(win);
        int c = getch();
        endwin();

        return 0;
}

```

8. setelah menulis kode maka untuk menjalankanya perlu utk di kompile, mengkompile disini kita lakukan langsung dari terminal dengan megetikan perintah `gcc ncurses.c -lncurses` dan utk C++ maka perintahnya daalah gpp ncurses.cpp -lncurses

Penting**

*- **gcc** nama kompiler sesuai bahasa, utk dilist ini adalah kompiler utk C*

*- **gpp** nama kopiler utk C++*

*- **ncurses.c** nama file yg akan dikompile*

*- **lncurses** nama pustaka/ library ncurses*



##### **output box();** 

ini adalah output dari souce code diatas fungsi box();

![](\assets\box.png)
