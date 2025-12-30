<img width="700" height="288" alt="image" src="https://github.com/user-attachments/assets/08ee6b09-7f81-407c-a407-a04147b4e120" />

Aplikasi untuk membantu dalam mengunduh data data di Website LPSE yang sumber/core prosesnya menggunakan https://github.com/wakataw/pyproc yang dibuat versi GUI nya

Petunjuk Penggunaan :

A. Input URL LPSE 

Cara memasukkan URL LPSE: 
1. Input CSV: Klik tombol "Pilih CSV" untuk memilih file CSV yang berisi daftar URL LPSE
2. Input Manual: Ketik atau Copy-Paste URL LPSE, contoh : https://spse.inaproc.id/pu

B. Pengaturan Download 

1. Tahun: Pilih tahun anggaran yang akan diunduh  
2. Workers: Jumlah worker untuk proses download (10-100)
3. Chunk: Jumlah data yang diproses per batch (10-100) 
4. Format: Format file output (xlsx/csv/json) 
5. Timeout: Batas waktu tunggu response server (30-90 detik) 

C. Opsi Tambahan 

1. Keep Index: Menyimpan file index untuk melanjutkan download yang terhenti 
2. Resume: Melanjutkan download dari posisi terakhir (hanya aktif jika Keep Index dicentang) 

D. Proses Download 

1. Klik tombol "Start Download" untuk memulai 
2. Proses akan secara langsung unduh untuk data "Tender" dan "Non Tender"
3. Progress bar akan menunjukkan kemajuan download 
4. Log output akan menampilkan detail proses 
5. Gunakan tombol "Stop Download" untuk menghentikan proses 

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

