![image](https://github.com/user-attachments/assets/65876ba7-b0ab-49db-8182-1e646b278252)

Aplikasi untuk membantu dalam mengunduh data data di Website LPSE yang sumber/core prosesnya menggunakan https://github.com/wakataw/pyproc yang dibuat versi GUI nya

Petunjuk Penggunaan :

A. Input URL LPSE 

Cara memasukkan URL LPSE: 
Input CSV: Klik tombol "Pilih CSV" untuk memilih file CSV yang berisi daftar URL LPSE 

B. Pengaturan Download 

1. Tahun: Pilih tahun anggaran yang akan diunduh 
2. Jenis: Pilih jenis lelang (Tender/Non-Tender) 
3. Workers: Jumlah worker untuk proses download (10-100) 
4. Format: Format file output (xlsx/csv/json) 
5. Timeout: Batas waktu tunggu response server (500-5000 detik) 

C. Opsi Tambahan 

1. Keep Index: Menyimpan file index untuk melanjutkan download yang terhenti 
2. Resume: Melanjutkan download dari posisi terakhir (hanya aktif jika Keep Index dicentang) 

D. Proses Download 

1. Klik tombol "Start Download" untuk memulai 
2. Progress bar akan menunjukkan kemajuan download 
3. Log output akan menampilkan detail proses 
4. Gunakan tombol "Stop Download" untuk menghentikan proses 

E. Format File CSV 

1. Jika menggunakan input CSV, format file harus: 
2. Menggunakan separator titik koma (;) 
   Kolom 1: URL LPSE 
   Kolom 2: Nama file output 

F. Tips 

1. Gunakan workers lebih sedikit (10-20) untuk koneksi lambat 
2. Aktifkan Keep Index untuk download data besar 
3. Pastikan URL LPSE valid dan bisa diakses 
4. Periksa folder output setelah download selesai 

