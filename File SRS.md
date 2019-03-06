<p><h2>1.	Pendahuluan</h2></p>
<p><h4>1.1	Tujuan</h4></p>
Dokumen Software Requirement Specification (SRS) merupakan dokumen spesifikasi perangkat lunak untuk membangun ”Aplikasi Ujian Online Di SMAN 1 Jatibarang Berbasis Web”. Dokumen ini dibangun untuk memudahkan dalam melakukan setiap kali ujian ataupun evaluasi per semester membantu guru dan siswa. Sehingga dokumen ini dapat dijadikan acuan teknis untuk membangun perangkat lunak ”ARG” (aplikasi random grup).<br/>
<p><h4>1.2	Lingkup Masalah</h4></p>
Ruang Lingkup dalam latar belakang yang dijelaskan diatas ini yaitu:<br/>
1.	Sistem ini hanya berupa prototipe, yang memberikan penataan atau pengaturan tentang ujian secara online.<br/>
2.	Lokasi yang menjadi tempat sampling adalah SMA N 1 Jaibarang. <br/>
3.	Prototipe aplikasi ini dibangun menggunakan PHP MyAdmin dan MySql sebagai databasenya.<br/> 
<p><h4>1.3	Definisi, akronim, singkatan</h4></p>
Akronim dan Singkatan :<br/>
•	HTML : HyperText Markup Language<br/>
Definisi :<br/>
•	HTML adalah Bahasa inti dari hampir semua konten Web. Sebagian besar dari apa yang Anda lihat pada layar browser anda adalah sebuah deskripsi, secara mendasar, menggunakan HTML.<br/>
•	use case adalah situasi dimana sistem anda digunakan untuk memenuhi satu atau lebih kebutuhan pemakaian anda.<br/>
<p><h4>1.4	Referensi</h4></p>
Referensi yang digunakan dalam pengembangan perangkat lunak ini adalah:<br/>
•	Praktikum Analisis dan Desain Sistem Informasi, 2009<br/>
•	Sistem Informasi Sekolah Terpadu, 2009<br/>
•	http://yaniwid.wordpress.com/2008/10/16/kebutuhan-fungsional-vs-non-fungsional/<br/>
•	UNSRI<br/>
<p><h4>1.5	Overview</h4></p>
Dokumen SRS ini dibagi menjadi tiga bagian utama, yaitu :<br/>
bagian pertama berisi penjelasan tentang dokumen SRS yang mencakup tujuan pembuatan dokumen ini, lingkup masalah yang diselesaikan oleh perangkat lunak yang dikembangkan, definisi, referensi dan deskripsi umum. Bagian kedua berisi penjelasan secara umum mengenai Aplikasi Random Grup yang akan dibangun, meliputi fungsi dari perangkat lunak, karakteristik pengguna, batasan dan asumsi yang diambil dala pembuatan perangkat lunak. Bagian ketiga berisi uraian kebutuhan perangkat lunak secara lebih rinci.<br/>

<h2>2. Gambaran Umum</h2><br>
<h4>2.1 Perspektif produk</h4>
<p>Aplikasi Ujian Online Berbasis Website di SMAN 1 Jatibarang adalah aplikasi yang menerapkan ujian menggunakan akses internet atau onlin. Dimana siswa dan siswi tidak perlu menggunakan peralatan ATK (Alat Tulis Kantor) tetapi hanya menggunakan electronik seperti laptop atau pun komputer, bahkan bisa untuk hp karena sudah berbasis website responsive dengan syarat dan ketentuan spesifikasi yang sudah ditentukan.</p>
<h4>2.1.1 Antarmuka sistem</h4>
<p>Antarmuka sistem pada aplikasi ini terdiri dari  developer, database dan user</p>
<h4>2.1.2 Antarmuka pengguna</h4>
<p>Aplikasi Ujian Online di SMAN 1 Jatibarang ini menggunakan antarmuka berbasis website dan pengguna mengoperasikannya menggunakan keyboard dan mouse dengan sistem operasi Windows. Rancangan antarmuka ini berfungsi untuk memperjelas mengenai menu program Aplikasi Ujian Online di SMAN 1 Jatibarang.</p>
<h4>2.1.3 Antarmuka perangkat keras</h4>
<h4>a. PC</h4>
- Monitor : sebagai sarana untuk menampilkan aplikasi kepada pemakai, yang mempunyai spesifikasi diantaranya: monitor mampu menampilkan grafis dengan kualitas warna yang baik (true color) untuk menampilkan laporan.<br>
- CPU : suatu perangkat keras microprocessor yang memahami dan melaksanakan suatu perintah dari perangkat lunak, sebut saja prosesor (pengolah data). Minimum requirement : Pentium IV, 1.7 Ghz processor or higher.<br>
- Memori (RAM) : sebuah tipe penyimpanan komputer yang isinya dapat diakses dalam waktu yang tetap tidak memperdulikan letak data tersebut dalam memori. Minimum requirement : 256 MB or higher.<br>
- Hardisk : sebuah komponen perangkat keras yang menyimpan data sekunder dan berisi piringan magnetis. Minimum Requirement : 5 Gb free Space Hard Drive<br>
Keyboard : Keyboard diperlukan sebagai sarana bagi pemakai untuk mengetikkan data masukan yang akan diproses perangkat lunak.<br>
- Mouse : Perangkat mouse digunakan sebagai sarana untuk memasukkan data input bagi perangkat lunak.
<h4>2.1.4 Antarmuka perangkat lunak</h4>
<p>Antarmuka yang digunakan pada pembuatan aplikasi yaitu : <br>
1. Sistem Operasi : Windows7 or Higher
2. Bahasa Pemrograman : HTML, PHP, Javascript<br>
3. Software Pengolah : Sublime Text<br>
4. Database Engine : Xampp<br>
5. Software Pendukung : Laragon</p>
<h4>2.1.5 Antarmuka komunikasi</h4>
<p>Antarmuka komunikasi yang digunakan pada aplikasi ini ini adalah internet</p>
<h4>2.1.6 Batasan memori</h4>
<ol>
	<li>RAM yang kami gunakan adalah 4Gb, tapi untuk kapassitas minimum 2 Gb</li>
	<li>Memori yang dibutuhkan untuk aplikasi minimal 20Mb</li>
</ol>
<h4>2.1.7 Operasi-operasi</h4>
<p>Operasi-operasi yang ada pada aplikasi ini yaitu :
<ol>
	<li>menyimpan</li>
	<li>membuka</li>
	<li>mengedit</li>
	<li>mengupdate</li>
	<li>mengeksekusi</li>
	<li>menghapus</li>
</ol></p>
<h4>2.1.8 Kebutuhan adaptasi</h4>
<ol>
	<li>Pemakaian data basa sebagai sarana penyimpanan data</li>
	<li>PL menggunakan bahasa Indonesia agar mudah dipahami oleh user</li>
</ol>
<h4>2.2 Fungsi-fungsi produk</h4>
<p>Fungsi Aplikasi Ujian Online Berbasis Website di SMAN 1 Jatibarang ini adalah menyediakan kemudahan dalam proses ujian tengah semester, ujian akhir semester, ujian harian dan ujian-ujian lainnya dengan harapan para siswa sudah terbiasa dengan pelaksanaan ujian secara online sebelum menghadapi ujian sekolah dan ujian nasional yang sudah menerapkan sistem online.</p>

<h4>2.3 Karakteristik pengguna</h4>
<p>Untuk mengoperasikan aplikasi ini tidak diperlukan tingkat pendidikan tinggi, namun pengguna dalam hal ini guru dan siswa cukup memahami cara menggunakannya saja.</p>

<h4>2.4 Batasan-batasan</h4>
<p>Hanya dapat dioperasikan pada OS Window 7 atau sistem operasi window di atas OS tersebut.</p>

<h4>2.5 Asumsi-asumsi dan keterkaitan</h4>
<p>Aplikasi Ujian Online Berbasis Website di SMAN 1 Jatibarang ini dapat dikembangkan lagi, seperti menambah beberapa fungsi yang lebih kompleks. Dapat pula dikombinasikan dengan mobile programming, agar user dapat lebih mudah mengoperasikan aplikasi ini melalui aplikasi mobile yang dapat diinstall pada smartphone mereka.</p>

<h4>2.6 Kebutuhan penyeimbang</h4>
<ol>
	<li>C-Requierements</li>
	<li>D-Requirements</li>
</ol>

<p><h2>3.	Kebutuhan lain yang spesifik</h2></p>
Kebutuhan Fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input, proses, dan output. Kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan ini adalah sebagai berikut:<br/>
1.	Sistem harus dapat mempermudah pengguna / user dalam pembagian kelompok.<br/>
2.	Sistem harus dapat mempermudah pengguna / user dalam menggunkan aplikasi ini.<br/>

<h2><p>4. Informasi pendukung</p></h2>
 Aplikasi kami memerlukan beberapa informasi pendukung seperti ;
 <ol>
 	<li>Data sekolah</li>
 	<li>Data siswa</li>
 	<lI>Data mata pelajaraan</lI>
 	<li>Data soal ujian</li>
 </ol>
 Informasi yang berupa data tersebut di perlukan untuk menyempurnakan aplikasi yang kami buat.