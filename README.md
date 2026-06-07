# Olist Customer Experience Analysis

## Tujuan
Menganalisis kepuasan pelanggan platform e-commerce Olist 
2016–2018 mencakup data cleaning, join multi-tabel, 
dan visualisasi dashboard.

## Tools
- Python (Pandas, NumPy): data cleaning & joining
- Google Colab: environment
- Looker Studio: dashboard visualisasi

## Dataset
- Sumber: Brazilian E-Commerce Public Dataset (Kaggle/Olist)
- 96.352 transaksi | 7 kolom | Periode 2016–2018
- Menggabungkan 4 tabel: orders, reviews, payments, customers

## Proses Cleaning
- Filter hanya order dengan status delivered (96.478 baris)
- Konversi 5 kolom timestamp ke datetime
- Hitung delivery delay (estimasi vs aktual pengiriman)
- Kategorisasi delivery status (tepat waktu vs terlambat)
- Join 4 tabel menjadi satu dataset terintegrasi
- Drop missing values (655 baris)

## Insight Utama
- 93,35% order terkirim tepat waktu
- Order terlambat mendapat review score 2,27 vs tepat waktu 4,29
- Credit card mendominasi 75,9% metode pembayaran
- State RJ memiliki order terbanyak namun review score rendah (3,96)

## Recommendation
- Prioritaskan perbaikan pengiriman di state RJ
- Tetapkan SLA maksimum keterlambatan
- Kembangkan notifikasi keterlambatan 

## Dashboard
https://datastudio.google.com/reporting/55aba421-7805-41d5-bf83-4588d1a0a190
