<p><h2>1.	Pendahuluan</h2></p>
Sistem ujian yang masih dilakukan secara manual termasuk dengan sistem koreksi ujiannya, membuat guru biasanya harus menambah jam kerja untuk membuat dan menilai soal ujian para mahasiswa secara manual. Dalam kemajuan teknologi informasi yang semakin pesat, ujian manual tidak lagi dapat dijadikan sebagai kegiatan rutin. Untuk itu dibutuhkan sebuah sistem ujian online sebagai solusi untuk mengoptimalkan sistem ujian manual.<br/>
Dalam perencanaan sistem ujian online digunakan analisis terstruktur yang terdiri dari tiga komponen yaitu, data flow diagram (DFD), kamus data dan spesifikasi proses. Basis data sistem ujian online dibuat berdasarkan pada tahapan analisis sistem sampai dengan normalisasi basis data. Informasi data ujian online diperoleh dari proses pelaksanaan ujian secara konvensional. Sehingga berdasarkan uraian diatas, maka dibuatlah dengan judul “Aplikasi Ujian Online BerbasisWebsite Responsive di SMA N 1 Jatibarang ”.<br/><br/>
<p><h4>1.1 Tujuan</h4></p>
Tujuan dari latar belakang diatas yaitu :<br/>
1.	Dapat membuat Aplikasi Ujian Online BerbasisWebsite Responsive di SMA N 1 Jatibarang secara sempurna.<br/>
2.	Aplikasi ini dapat digunakan sebagai forum komunikasi member dan juga dapat menyampaikan informasi secara realtime.<br/>
3.	Penulis dapat mengolah data yang banyak.<br/>
<p><h4>1.2 Lingkup</h4></p>
Ruang Lingkup dalam latar belakang yang dijelaskan diatas ini yaitu:<br/>
1.	Sistem ini hanya berupa prototipe, yang memberikan penataan atau pengaturan tentang ujian secara online.<br/>
2.	Lokasi yang menjadi tempat sampling adalah SMA N 1 Jaibarang. <br/>
3.	Prototipe aplikasi ini dibangun menggunakan PHP MyAdmin dan MySql sebagai databasenya.<br/> 
<p><h4>1.3 Definisi, akronim, dan singkatan</h4></p>
Akronim dan Singkatan :<br/>
•	HTML : HyperText Markup Language<br/>
Definisi :<br/>
•	HTML adalah Bahasa inti dari hampir semua konten Web. Sebagian besar dari apa yang Anda lihat pada layar browser anda adalah sebuah deskripsi, secara mendasar, menggunakan HTML.<br/>
•	use case adalah situasi dimana sistem anda digunakan untuk memenuhi satu atau lebih kebutuhan pemakaian anda.<br/>
<p><h2>2.	Referensi</h2></p>
Referensi yang digunakan dalam pengembangan perangkat lunak ini adalah:<br/>
•	Praktikum Analisis dan Desain Sistem Informasi, 2009<br/>
•	Sistem Informasi Sekolah Terpadu, 2009<br/>
•	http://yaniwid.wordpress.com/2008/10/16/kebutuhan-fungsional-vs-non-fungsional/<br/>
•	UNSRI<br/>

<h2>3. Penjelasan Dekomposisi</h2>
<h4>3.1 Dekomposisi Modul</h4>
<p>Kebutuhan fungsional (Functional Requirements) ini adalah kebutuhan utama yang diharapkan dari sistem ini, yang terkait langsung dengan sistem ini. Kebutuhan fungsional dari sistem ini adalah sebagai berikut:
<ol>
	<li>Pencatatan Hak Akses</li>
	<li>Pencatatan Nama aplikasi , Nama Kategori dan Nama Client</li>
	<li>Pencatatan Target Waktu , Jumlah Orang dan Biaya Aplikasi</li>
</ol>
Spesifikasi yang diharapkan pada Pencatatan Hak Akses :
<ol>
	<li>Membedakan antara Admin, Guru dan Siswa</li>
	<li>Sistem dapat memproses secara otomatis jika kita terdaftar sebagai admin memiliki hak akses penuh dan ketika kiita terdaftar sebagai guru dan siswa tidak memiliki hak akses penuh</li>
</ol>
Spesifikasi yang diharapkan pada Pancatatan Nama Aplikasi, Nama Kategori dan Nama Client :
<ol>
	<li>Mencatat nama aplikasi apa yang akna di buat dalam sebuah project</li>
	<li>Mencatat nama-nama kategori apa yang akan di buat di sebuah project</li>
	<li>Mencatat nama client yang mau di buat kan sebuah project</li>
</ol>
Spesifikasi yang diharapkan pada Pencatatan Target Waktu , Jumlah Orang dan Biaya Aplikasi :
<ol>
	<li>Sistem dapat memproses secara otomatis target waktu aplikasi yang akan di buat dalam sebuah project</li>
	<li>Sistem dapat memproses secara otomatis jumlah orang dalam project</li>
	<li>Sistem dapat memproses secara otomatis biaya dalam sebuah aplikasi yang akan di buat</li>
</ol>
</p>

<h4>3.2 Dekomposisi Proses Konkuren</h4>
<p>
	Konkurensi adalah proses-proses (lebih dari satu proses) yang terjadi pada saat bersamaan. Konkurensi merupakan landasan umum perancangan sistem operasi. Proses-proses disebut konkuren jika proses-proses berada pada saat yang sama. Pada proses-proses konkuren yang berinteraksi mempunyai beberapa masalah yang harus diselesaikan:
	<ol>
		<li>Mutual Exclusion</li>
		<li>Sinkronisasi</li>
		<li>Deadlock</li>
		<li>Startvation</li>
	</ol>
	Pada sistem dengan banyak proses (kongkuren), terdapat 3 katagori interaksi, yaitu:
	<ol>
		<li>Proses-proses Saling Tidak Peduli (Independen).<br>
		Proses-proses ini tidak dimaksudkan untuk bekerja untukmencapai tujuan tertentu. Pada multiprogramming dengan proses-proses independen, dapat berupa batch atau sesi interaktif, atau campuran keduanya.</li>

		<li>Proses-proses Saling Mempedulikan Secara Tidak Langsung.<br>
		Proses-proses tidak perlu saling mempedulikan identitas proses-proses lain, tapi sama-sama mengakses objek tertentu, seperti buffer masukan/keluaran. Proses-proses itu perlu bekerja sama (cooperation) dalam memakai bersama objek tertentu.
		</li>
		<li>Proses-proses konkuren mengharuskan beberapa hal yang harus ditangani, antara lain:<br>
		a. Sistem operasi harus mengetahui proses-proses yang aktif<br>
		b. Sistem operasi harus mengalokasikan dan mendealokasikan beragam sumber daya untuk tiap proses aktif. Sumber daya yang harus dikelola, antara lain:
		<ol>
			<li>Waktu pemroses.</li>
			<li>Memri</li>
			<li>Berkas-Berkas</li>
			<li>Perangkat I/O</li>
		</ol>
		c. Sistem operasi harus memproteksi data dan sumber daya fisik masing-masing proses dari gangguan proses-proses lain.<br>
		d. Hasil-hasil proses harus independen terhadap kecepatan relatif proses-proses lain dimana eksekusi dilakukan.
		</li>
	</ol>
</p>

<h4>3.3 Dekomposisi Data</h4>
3.3.1 Deskripsi Entri Data 1<br>
3.3.2 Deskripsi Entri Data 2<br>

<h2>4. Deskripsi Ketergantungan/Keterkaitan</h2>
<h4>4.1 Keterkaitan Inter Modul</h4>
<p>Ketika merancang sebuah Dependensi Inter-modul sistem, dapat dirancang dengan dua cara yang luas dan cara pertama adalah untuk merancang sistem yang lengkap dengan menggunakan sistem yang sudah diketahui dan mengimplementasikan fitur baru yang diperlukan untuk meningkatkan efektivitas sistem dan mengujinya di kondisi nyata. Cara alternatif akan merancang sistem dan biasanya karena biaya untuk menyiapkan antarmuka antara modul. Modul dari siaran berita Sistem SCC tergantung pada penyebaran informasi. Antar-modul dari penelitian ini adalah tampilan dari pengumuman dan itu termasuk database sistem. Kemudian seluruh informasi yang telah dimasukkan akan disimpan dalam database, yang berasal dari proses input sampai pengumuman menampilkan ke monitor lain.</p>
<h4>4.2 Keterkaitan Inter Proses</h4>
<p>Proses yang dilakukan oleh pengguna dalam melakukan ujian online akan mempengaruhi beberapa proses lainya seperti penentuan value, dan penjadwalan. Juga data akan tersimpan sebagai riwayat proses pemesanan.</p>
<h4>4.3 Keterkaitan Data</h4>
<p>Dependensi data didasarkan pada pengguna. Mereka adalah orang yang akan menggunakan sistem ujian online ini.</p>

<h3>5. Deskripsi Antarmuka</h3>

Deskripsi tiap-tiap antarmuka yang meliputi:

5.1 Antarmuka modul
	<ol>5.1.1 Modul Siswa
	Terdapat fiture login untuk siswa dan modul untuk memulai ujian online.<br/>
	5.1.2 Modul Guru
	Terdapat fiture login untuk guru dan modul untuk menambahkan soal.<br/>
	5.1.3 Modul Admin
	Terdapat fiture login untuk admin dan admin dapat memonitoring segala aktifitas di website ini.</lo>
	
5.2 Antarmuka proses
	<ol>5.2.1 Login
	Login adalah proses validasi user untuk dapat mengakses website ini.<br/> 
	5.2.2 Penambahan soal
	Merupakan proses yang dapat di lakukan guru untuk dapat memberikan soal kepada siswa<br/>
	5.2.3 Pengerjaan soal
	Merupakan proses yang dapat di lakukan siswa untuk mengerjakan soal yang diberikan oleh guru<br/>
	5.2.4 Logout
	Merupakan proses pada user untuk dapat keluar dari website

<h3>6. Desain Rinci</h3>

6.1 Desain Rinci Modul

Di sini dijelaskan semua rincian desain yang diperlukan dari tiap-tiap modul yang ada dari suatu aplikasi. Biasanya digambarkan dengan diagram-diagram seperti: diagram state; diagram sequence; dan lain-lain

6.2 Desain Rinci Data

Di sini dijelaskan semua rincian desain yang diperlukan dari tiap-tiap entitas data, dapat disajikan dalan bentuk diagram alir data, dan flow chart.