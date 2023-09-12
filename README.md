<h1>Spesifikasi Kebutuhan Perangkat Lunak Untuk GPS Tracking Motorcycle</h1>
<h3>Versi 1.0 Disetujui</h3>
<br>
<b>Disusun Oleh :</b>
<ul>
  <li>Putri Puspitasari (22091397097)</li>
  <li>Danu Teguh Heri Prasetyo (22091397100)</li>
  <li>Amallia Berliany Putri (22091397102)</li>
</ul>
<br>
<b>D4 Manajemen  Informatika Fakultas Vokasi Universitas Negeri Surabaya</b>
<b>2023</b>
 

Daftar Isi
1.	Pengantar	1
1.1	Tujuan	1
1.2	Konvensi Dokumen	1
1.3	Audiens Yang Dituju	2
1.4	Lingkup Produk	2
1.5	Referensi	3
2.	Deskripsi Keseluruhan	4
2.1	Perspektif Produk	4
2.2	Fungsi Produk	4
2.3	Kelas dan Karakteristik Pengguna	5
2.4	Lingkungan Pengembangan	7
2.5	Kendala Desain dan Implementasi	7
2.6	Dokumentasi Pengguna	8
2.7	Asumsi dan Dependensi	10
3.	Persyaratan Antarmuka	11
3.1	Antarmuka Pengguna	11
3.2	Antarmuka Perangkat Keras	15
3.3	Antarmuka Perangkat Lunak	15
3.4	Antarmuka Komunikasi	15
4.	Fitur Sistem	16
4.1	Lokasi secara Real-Time	16
4.2	Riwayat Lokasi	16
4.3	Temukan Lokasi	16
4.4	Terhuung dengan Sepeda motor	16
4.5	Notifikasi	16
5.	Persyaratan Fungsional Lainnya	17
5.1	Persyaratan Performa	17
5.2	Persyaratan Keamanan Pengguna	17
5.3	Persyaratan Keamanan GPS Tracking Motorcycle	18
5.4	Atribut Kualitas Perangkat Lunak	18
5.5	Proses Bisnis	20
6.	Persyaratan	21
 
Riwayat Perubahan

Nama	Tanggal	Alasan Perubahan	Versi
			
			
 

1.	Pengantar

1.1	Tujuan

Tujuan pembuatan GPS Tracking Motorcycle antara lain :

1.	Untuk meningkatkan keamanan pengendara dan sepeda motor
2.	Dapat melacak posisi sepeda motor secara real-time
3.	Meningkatkan efisiensi penggunaan sepeda motor
4.	Dapat meminimalisir risiko pencurian
5.	Dapat membantu menemukan posisi sepeda motor yang hilang
6.	Pemilik	kendaraan	dapat	merencanakan	rute	yang	lebih	efisien	dan menghindari kemacetan dengan adanya informasi lokasi yang akurat

1.2	Konvensi Dokumen

Aplikasi yang akan dikembangkan adalah GPS Tracking Motorcycle, sebuah aplikasi yang memungkinkan pemilik sepeda motor untuk melacak dan memantau pergerakan sepeda motornya secara real-time. Aplikasi ini memanfaatkan teknologi GPS (Global Positioning System) untuk menentukan posisi sepeda motor. GPS Tracking Motorcycle dapat melakukan hal-hal berikut ini :

1.	Sistem dapat menampilkan menu pendaftaran akun untuk login ke aplikasi
2.	Sistem dapat menampilkan menu login
3.	Sistem harus mampu melacak posisi sepeda motor secara real-time
4.	Sistem dapat menampilkan posisi sepeda motor pada peta
5.	Sistem harus mampu mengirimkan notifikasi pada pengguna jika terjadi situasi yang tidak diinginkan
6.	Sistem harus mampu mencatat riwayat perjalanan sepeda motor, seperti waktu, lokasi,dan rute yang ditempuh
7.	Sistem harus memiliki fitur manajemen pengguna
8.	Sistem dapat diintegrasikan dengan aplikasi lain
9.	Sistem dapat menganalisis data lokasi dan waktu
10.	Sistem harus mampu bergerak dengan berbagai jenis sepeda motor
11.	Sistem dapat memantau kecepatan motor
12.	Sistem harus bekerja dengan menggunakan daya baterai sepeda motor, sepertibaterai internal atau tenaga surya
13.	Sistem memiliki tampilan yang mudah dipahami
14.	Sistem dapat dioperasikan sesuai fungsinya dengan baik termasuk fitur-fitur yang diinginkan
15.	Sistem harus dapat diandalkan
16.	Sistem harus tersedia dan dapat diakses oleh pengguna kapan saja
17.	Sistem harus memiliki performa yang baik dan responsive
18.	Sistem dapat mengatasi pertumbuhan pengguna dan data yang semakin besar
19.	Sistem harus dilengkapi dengan dukungan teknis yang baik
20.	Sistem dapat menjamin keamanan data akun
21.	Sistem dapat diakses dengan smartphone
22.	Sistem harus meminim kesalahan dari masalah
 

1.3	Audiens Yang Dituju

Pengguna yang dituju untuk pengembangan aplikasi GPS tracking untuk sepeda motor dapat mencakup beberapa kelompok, antara lain :

1.	Pemilik Sepeda Motor: Pemilik sepeda motor adalah target utama untuk aplikasi GPS tracking. Mereka akan menggunakan aplikasi tersebut untuk melacak lokasi sepeda motor mereka dalam situasi tertentu, seperti pencurian atau jika mereka ingin memantau pergerakan sepeda motor mereka.

2.	Perusahaan Rental Sepeda Motor: Perusahaan rental sepeda motor dapat menjadi audiens yang potensial untuk aplikasi GPS tracking. Mereka dapat menggunakan aplikasi tersebut untuk melacak dan mengelola sepeda motor yang mereka sewakan kepada pelanggan mereka.

3.	Penyedia Layanan Kurir atau Pengiriman: Penyedia layanan kurir atau pengiriman juga dapat menjadi target audiens. Mereka dapat menggunakan aplikasi GPS tracking untuk melacak posisi sepeda motor kurir dan memantau pengiriman barang dengan lebih efisien.

4.	Klub atau Komunitas Sepeda Motor: Klub atau komunitas sepeda motor juga bisa menjadi audiens yang berpotensi. Mereka dSapat menggunakan aplikasi GPS tracking untuk mengorganisir perjalanan bersama atau acara lainnya, sehingga anggota dapat melihat posisi sepeda motor satu sama lain dalam waktu nyata.

5.	Pemilik Flotila Sepeda Motor: Jika ada pemilik bisnis atau organisasi yang memiliki flotilla sepeda motor, seperti layanan pengantaran makanan atau layanan kurir. Aplikasi ini dapat membantu mereka mengawasi sepeda motor dan meningkatkan efisiensi operasional.

1.4	Lingkup Produk

GPS tracking untuk sepeda motor melibatkan penggunaan teknologi Global Positioning System (GPS) untuk melacak lokasi, pergerakan, dan informasi relevan lainnya dari sepeda motor secara real-time. Hal ini menawarkan berbagai manfaat, termasuk pencegahan pencurian, manajemen armada, dan peningkatan keamanan. Berikut adalah beberapa aspek dan fitur utama terkait GPS tracking untuk sepeda motor :

1.	Pelacakan lokasi real-time: Sistem GPS tracking memungkinkan pemilik sepeda motor atau manajer armada untuk memantau lokasi sepeda motor secara real- time melalui satelit GPS. Informasi ini biasanya dapat diakses melalui platform berbasis web atau aplikasi mobile.
2.	Pencegahan dan pemulihan pencurian: GPS tracker menyediakan cara yang efektif untuk mencegah pencurian sepeda motor. Pada saat terjadinya pencurian, pemilik dapat melacak lokasi sepeda motor yang dicuri dan berkoordinasi dengan pihak berwenang untuk melakukan pemulihan.
3.	Geofencing: fitur yang memungkinkan pengguna untuk mengatur batas virtual atau geofence di sekitar area tertentu. Ketika sepeda motor yang dilengkapi dengan GPS tracker memasuki atau keluar dari batas-batas ini, sistem akan mengirimkan peringatan kepada pemilik atau manajer armada, memberikan notifikasi secara langsung.
 

4.	Riwayat rute: GPS tracking juga dapat menyimpan riwayat rute yang telah ditempuh oleh sepeda motor. Informasi ini dapat digunakan untuk analisis perjalanan, pemantauan kinerja, dan perencanaan perjalanan di masa depan.
5.	Fitur tambahan: Selain fitur utama yang disebutkan di atas, beberapa GPS tracker untuk sepeda motor juga dapat dilengkapi dengan fitur tambahan seperti pemantauan kecepatan, notifikasi kebocoran bahan bakar, pemadaman mesin dari jarak jauh, dan sebagainya.
6.	GPS tracking untuk sepeda motor memberikan kemudahan dan keamanan tambahan bagi pemilik sepeda motor atau perusahaan yang memiliki armada sepeda motor. Dengan memanfaatkan teknologi GPS, mereka dapat melacak dan mengawasi sepeda motor secara efektif dalam berbagai situasi.

1.5	Referensi

Dokumen ini merujuk pada hasil observasi yang berkaitan dengan kebutuhan dan mencakup data secara umum, diperlukannya dan penulis dokumen berdasarkan pada:

1.	https://moladin.com/blog/fungsi-gps-tracker-motor/
2.	https://gpsku.co.id/gps-motor/
3.	https://www.sologlobaltracker.com/mengenal-gps-tracker-fungsi-manfaat-dan- penggunaannya-dalam-kehidupan-sehari-hari/
4.	https://openlibrary.telkomuniversity.ac.id/pustaka/files/162743/jurnal_eproc/pera ncangan-gps-tracking-untuk-penyewaan-kendaraan-bermotor.pdf
5.	https://appmaster.io/id/blog/proses-pengembangan-aplikasi-gps-dan-contohnya
6.	https://cartrack.id/id/5-fitur-gps-tracker-yang-wajib-ada-dalam-sistem- pemantauan-kendaraan
 

2.	Deskripsi Keseluruhan

2.1	Perspektif Produk
2.2	Fungsi Produk
2.3	Kelas dan Karakteristik Pengguna
2.4	Lingkungan Pengembangan
2.5	Kendala Desain dan Implementasi
2.6	Dokumentasi Pengguna
2.7	Asumsi dan Dependens 

3.	Persyaratan Antarmuka

3.1	Antarmuka Pengguna
3.2	Antarmuka Perangkat Keras

3.3	Antarmuka Perangkat Lunak

3.4	Antarmuka Komunikas 

4.	Fitur Sistem

Sistem aplikasi GPS tracking untuk sepeda motor memiliki beberapa fitur penting yang mencakup :

4.1	Real-Time Location (Lokasi secara Real-Time) :

Fitur ini memungkinkan pengguna aplikasi untuk melihat lokasi sepeda motor secara langsung dan akurat dalam waktu nyata. Informasi lokasi yang terus diperbarui memungkinkan pengguna untuk melacak pergerakan sepeda motor secara aktif.

4.2	History Location (Riwayat Lokasi) :

4.3	Find Location (Temukan Lokasi) :

4.4	Connect to Motorcycle (Terhubung dengan Sepeda Motor) :
4.5	Notification (Notifikasi) :
 


5.	Persyaratan Fungsional Lainnya

5.1	Persyaratan Performa

5.2	Persyaratan Keamanan Pengguna
5.3	Persyaratan Keamanan GPS Tracking Motorcycle

5.4	Atribut Kualitas Perangkat Lunak

5.5	Proses Bisnis


 

6.	Persyaratan
Lampiran A : Glosarium

Istilah	Definisi
	
	
	
	
	
	

Lampiran B : Model Analisis
A.	DFD (Data Flow Diagram)
B.	ERD (Entity Relationship Diagram)
C.	CDM (Conceptual Data Model)
D.	PDM (Physical Data Model)
E.	Flowchart Login
F.	Use Case Diagram



 
 

Lampiran C : Daftar Fitur Yang Akan Ditentukan


Nomor Persyaratan	Nama Persyaratan	Halaman
		
		
		
		
		
		

