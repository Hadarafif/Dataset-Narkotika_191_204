
# 📘 Dataset Narkotika (PN Pasuruan 2023–2025)

## 🧾 Deskripsi
Repositori **Dataset Narkotika** berisi hasil pengumpulan data putusan pengadilan dari situs resmi [putusan3.mahkamahagung.go.id](https://putusan3.mahkamahagung.go.id).  
Dataset difokuskan pada perkara **Narkotika dan Psikotropika** di **Pengadilan Negeri Pasuruan** dalam rentang waktu **2023–2025**.  

Data ini dikumpulkan untuk keperluan **penelitian hukum dan analisis data**, seperti klasifikasi jenis perkara, analisis amar putusan, atau pemetaan barang bukti.

---

## 📂 Struktur Repositori

```
📦 Dataset-Narkotika/
├── dataset/Narkotika.zip          # Dataset mentah hasil scraping (PDF)
├── Overview/Overview.xlsx        # Rekapitulasi hasil scraping dalam format Excel
└── README.md            # Dokumentasi proyek
```

---

## 📊 Deskripsi File

### `Overview.xlsx`
Berisi ringkasan hasil scraping dengan kolom utama:
- **Nomor Putusan** — ID perkara di sistem MA  
- **lembaga peradilan** — Tempat pengadilan 
- **Barang Bukti** — Daftar barang bukti yang ditemukan  
- **Amar Putusan** — Isi vonis hakim (misalnya pidana penjara, denda, rehabilitasi)  


### `dataset.zip`
Berisi dataset mentah  berupa PDF yang dapat digunakan untuk eksplorasi data atau analisis lanjutan seperti:
- Analisis teks amar putusan  
- Klasifikasi jenis hukuman  
- Pemetaan pola barang bukti dan lama hukuman  

---

## 🧠 Tujuan Dataset
Dataset ini disiapkan untuk:
- Penelitian bidang **Data Science** dan **Text Mining** pada dokumen hukum.  
- Analisis **TKI (Temu Kembali Informasi)** pada konteks hukum pidana.  
- Studi perbandingan terhadap **putusan perkara Narkotika dan Psikotropika** di PN Pasuruan.

---

## 🧩 Cara Menggunakan Dataset

1. **Ekstrak dataset**
   ```bash
   unzip dataset.zip -d dataset/
   ```

2. **Buka file `Overview.xlsx`**
   Dapat dibuka menggunakan:
   - Microsoft Excel / WPS Office  
   - Google Sheets  
   - Python (pandas)
     ```python
     import pandas as pd
     df = pd.read_excel("Overview.xlsx")
     df.head()
     ```

3. **Lakukan analisis**
   - Eksplorasi jumlah kasus per tahun  
   - Analisis teks amar putusan  
   - Visualisasi pola barang bukti  

---

## 📈 Contoh Statistik (Estimasi)

| Tahun | Jumlah Kasus | Rata-rata Lama Hukuman | PDF Valid |
|-------|---------------|------------------------|-----------|
| 2023  | 20            | 4,8 tahun              | ✅ 100% |
| 2024  | 18            | 5,1 tahun              | ✅ 100% |
| 2025  | 12            | 4,5 tahun              | ✅ 100% |

> Semua data dalam dataset ini memiliki file PDF putusan yang valid.

---

## 🧑‍💻 Penyusun
**M. Haidar Afif Al Azizi**  
NIM: 202210370311191  
Program Studi Informatika — Universitas Muhammadiyah Malang  

**Apriadzandy putra**  
NIM: 202210370311204  
Program Studi Informatika — Universitas Muhammadiyah Malang  

---

## 📜 Lisensi
Dataset ini dibuat **hanya untuk tujuan akademik dan penelitian**.  
