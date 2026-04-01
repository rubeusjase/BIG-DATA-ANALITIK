RINGKASAN



Project ini bertujuan untuk melakukan proses data ingestion dari berbagai sumber data seperti PostgreSQL, CSV, dan XLSX ke dalam data lake menggunakan MinIO.



Pipeline yang dijalankan meliputi:

\- Extraction (mengambil data dari berbagai sumber)

\- Validation (pengecekan kualitas data)

\- Standardization (normalisasi struktur data)

\- Storage (penyimpanan ke MinIO)



Seluruh proses berhasil dijalankan menggunakan Docker dan Python.





KENDALA



1\. Module yaml tidak ditemukan

Penyebab:

Dependency Python belum terinstall



Solusi:

Menjalankan perintah:

pip install -r requirements.txt





2\. PostgreSQL error (tidak berjalan)

Penyebab:

Belum ada konfigurasi password pada database



Solusi:

Mengisi file .env dengan POSTGRES\_PASSWORD

