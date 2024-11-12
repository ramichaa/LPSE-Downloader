# LPSE-Downloader
Aplikasi untuk membantu dalam mengunduh data data di Website LPSE yang sumber/core prosesnya menggunakan https://github.com/wakataw/pyproc yang dibuat versi GUI nya

### Cara Penggunaan ###
1. Download LPSE_Downloader versi terbaru
2. Buat file csv dengan nama daftar_lpse.csv dengan format : [url_lpse];[nama_file]
3. Jalankan aplikasi
4. Pilih file daftar_lpse.csv
5. Atur parameter sesuai kebutuhan
6. Klik "Start Download"

### Penjelasan Menu ###
A.	Workers : Jumlah koneksi yang berjalan secara bersamaan saat mengunduh detil paket dengan maksimal 50 worker ( default 10 )
B.	Chunk Size : Jumlah daftar paket per halaman yang diunduh. Semakin besar jumlah tidak menjamin proses download semakin cepat. Gunakanlah jumlah data yang wajar sehingga tidak membebani server SPSE ( default 100 )
C.	Output Format : Silahkan dipilih xlsx, csv atau json
D.	Timeout (detik) ; Waktu tunggu jika koneksi lambat , maksimal 90, minimal 30, default 60
E.	Keep Index : Jika di centang maka akan membentuk file idx (sqlite3 database) saat proses download tidak akan dihapus ketika proses selesai. Hapus centang jika ingin menghapus database tersebut.
F.	Resume : Jika di centang maka argument ini untuk melanjutkan proses yang gagal (karena internet putus atau gangguan koneksi lainnya). Namun pastikan bahwa seluruh index sudah berhasil diunduh
