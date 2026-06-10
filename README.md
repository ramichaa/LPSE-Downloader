<img width="697" height="296" alt="image" src="https://github.com/user-attachments/assets/91a427d5-4ada-414a-9784-ebbd54c0cb8d" />

Aplikasi untuk membantu dalam mengunduh data data di Website LPSE yang sumber/core prosesnya menggunakan https://github.com/wakataw/pyproc yang dibuat versi GUI nya

Petunjuk Penggunaan 
1. Menentukan LPSE 
Gunakan salah satu cara berikut: 
Nama instansi, contoh: kutai barat. 
Kode instansi, contoh: kutaibaratkab atau kubar. 
URL lengkap, contoh: https://spse.inaproc.id/mahakamulukab. 
Klik Pilih CSV atau seret file CSV ke jendela aplikasi. 
Nama instansi dicocokkan otomatis dengan direktori resmi Portal SPSE Indonesia. Fitur ini berlaku untuk kota, kabupaten, provinsi, kementerian, lembaga, dan instansi lain yang terdaftar. 
Jika nama wilayah memiliki kota dan kabupaten dengan nama yang sama, tuliskan jenis wilayah secara lengkap. Contoh: Kota Semarang atau Kabupaten Semarang. Direktori disimpan sementara selama tujuh hari agar pencarian berikutnya lebih cepat. 

2. Format File CSV 
Gunakan pemisah titik koma (;) atau koma (,). Kolom pertama berisi alamat/nama LPSE dan kolom kedua berisi nama file output yang bersifat opsional. 
https://spse.inaproc.id/kutaibaratkab;LPSE_Kutai_Barat
mahakamulukab;LPSE_Mahakam_Ulu
         
Baris judul seperti url, host, atau lpse_host akan dilewati. URL ganda hanya diproses satu kali. 

3. Pengaturan Download 
Tahun: tahun anggaran paket yang akan diambil. 
Worker: jumlah proses detail yang berjalan bersamaan. 
Chunk: jumlah paket yang diproses dalam satu kelompok. 
Delay: jeda antarhalaman indeks agar server tidak terbebani. 
Format: jenis file hasil, seperti XLSX, CSV, atau JSON. 
Timeout: batas waktu menunggu respons server LPSE. 
Keep Index: menyimpan indeks paket untuk proses berikutnya. 
Resume: melanjutkan data yang sudah pernah diproses. 

4. Menjalankan Proses 
Klik Start. 
Aplikasi memproses data Tender terlebih dahulu. 
Jika Tender selesai tanpa kegagalan target, aplikasi otomatis melanjutkan ke Non-Tender. 
Panel Log Proses tampil selama download dan otomatis tersembunyi setelah seluruh proses selesai. 
Klik Stop untuk meminta proses dihentikan dengan aman. 

5. Jika Terjadi Masalah 
Pastikan alamat LPSE benar dan dapat dibuka melalui browser. 
Naikkan Timeout jika koneksi atau server LPSE lambat. 
Kurangi Worker jika server sering menolak atau memutus koneksi. 
Periksa pesan pada Log Proses untuk mengetahui target yang gagal. 
Data tidak lengkap dapat terjadi jika informasi sumber di LPSE memang belum tersedia.  

6. Tips 

1. Gunakan workers lebih sedikit (10-20) untuk koneksi lambat 
2. Aktifkan Keep Index untuk download data besar 
3. Pastikan URL LPSE valid dan bisa diakses 
4. Periksa folder output setelah download selesai 

