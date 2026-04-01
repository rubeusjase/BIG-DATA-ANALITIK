\# Minilab Big Data \& Analitik — Tahap 1



\## Deskripsi

Project ini merupakan implementasi minilab big data untuk proses data ingestion dari berbagai sumber (RDBMS dan file) ke dalam data lake menggunakan MinIO.



\---



\## Komponen yang Digunakan

\- Docker

\- PostgreSQL (RDBMS)

\- MinIO (Object Storage)

\- Python (Ingestion Pipeline)



\---



\## Cara Menjalankan (Versi Personal)



1\. Buka Docker Desktop dan pastikan sudah running



2\. Masuk ke folder project: cd "C:\\Users\\akjas\\OneDrive\\Documents\\kuliah\\SEMESTER 6\\BDA\\minilab-bigdata"



3\. Jalankan container:docker compose up -d



4\. Cek container: docker ps



5\. Install dependency: pip install -r requirements.txt



6\. Jalankan ingestion: python -m ingestion.main\_ingest



7\. Buka MinIO: http://localhost:9000



4\. Cek container:



Login:

\- user: minioadmin

\- password: minioadmin123



\---



\## Pengalaman Implementasi



Selama menjalankan project ini, saya mempelajari bahwa deployment menggunakan Docker memungkinkan proses instalasi komponen seperti database dan storage dilakukan secara otomatis tanpa perlu instalasi manual.



Selain itu, pipeline ingestion berjalan secara terstruktur mulai dari proses extraction, validation, standardization, hingga storage ke MinIO.



Saya juga memahami bahwa setiap kali ingestion dijalankan, data akan disimpan dengan timestamp sehingga tidak terjadi overwrite.



\---



\## Status

\- Deployment: Berhasil

\- Ingestion: Berhasil

\- Data tersimpan di MinIO

\- Testing: 18 passed

