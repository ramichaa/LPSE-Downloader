# LPSE Data Downloader

![image](https://github.com/user-attachments/assets/ffac85de-ab57-4c4c-a96b-456ecb3e220e)

Aplikasi untuk membantu dalam mengunduh data data di Website LPSE yang sumber/core prosesnya menggunakan https://github.com/wakataw/pyproc yang dibuat versi GUI nya

### Cara Penggunaan ###
1. Download LPSE_Downloader versi terbaru
2. Buat file csv dengan nama daftar_lpse.csv dengan format : [url_lpse];[nama_file]
3. Jalankan aplikasi
4. Pilih file daftar_lpse.csv
5. Atur parameter sesuai kebutuhan
6. Klik "Start Download"

### Penjelasan Menu ###
1. **Workers** : Jumlah koneksi yang berjalan secara bersamaan saat mengunduh detil paket dengan maksimal 50 worker ( default 10 ).
2. **Chunk Size** : Jumlah daftar paket per halaman yang diunduh. Semakin besar jumlah tidak menjamin proses download semakin cepat. Gunakanlah jumlah data yang wajar sehingga tidak membebani server SPSE ( default 100 ).
3. **Output Format** : Silahkan dipilih xlsx, csv atau json
4. **Timeout (detik)** ; Waktu tunggu jika koneksi lambat , maksimal 90, minimal 30, default 60.
5. **Keep Index** : Jika di centang maka akan membentuk file idx (sqlite3 database) saat proses download tidak akan dihapus ketika proses selesai. Hapus centang jika ingin menghapus database tersebut.
6. **Tahun** : Tahun Anggaran data LPSE
7. **Jenis** : Tender dan Non Tender ( Pilih salah satu ).

