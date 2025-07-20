# 📊 Analysis of Tuna Fish Quantity Trends in the Tokyo Wholesale Market 🐟

## 📁 Deskripsi Singkat

Proyek ini bertujuan untuk menganalisis data historis jumlah ikan tuna (Bluefin Tuna) yang dijual di Pasar Grosir Tokyo, menggunakan pendekatan data analitik dan model AI (Large Language Model - LLM). Analisis ini membantu mengidentifikasi pola musiman, fluktuasi quantity, serta memberikan rekomendasi untuk konsumen, nelayan, dan pembuat kebijakan.

---

## 📦 Dataset

- **Nama**: Tokyo Wholesale Tuna Prices
- **Sumber**: [Kaggle - Tokyo Tuna Dataset](https://www.kaggle.com/datasets/tcashion/tokyo-wholesale-tuna-prices)
- **Ukuran**: Kecil (~200 baris), cocok untuk analisis time series ringan
- **Fitur utama**:
  - `year`, `month` → tahun dan bulan penjualan
  - `value` → jumlah ikan tuna
  - `species`, `fleet`, `state`, `measure` sebagai atribut tambahan

---

## 🎯 Tujuan Proyek

- Mengidentifikasi tren jumlah ikan tuna dari waktu ke waktu
- Menemukan insight menarik dari pola quantity
- Memberikan rekomendasi berbasis data menggunakan dukungan AI (IBM Granite LLM)

---

## ⚙️ Langkah-langkah Analisis

1. 📥 Impor dataset & konversi waktu (`year` + `month` → `date`)
2. 📊 Hitung statistik deskriptif (mean, max, min)
3. 📈 Visualisasi tren jumlah ikan dari waktu ke waktu
4. 🤖 Prompt ke LLM untuk merangkum insight & membuat rekomendasi

---

## 💡 Insight & Temuan

- Rata-rata quantity per bulan: **≈ {mean_val:.2f}**
- Quantity tertinggi: **{max_val:.2f}**, pada **{max_row['month']}/{max_row['year']}**
- Quantity terendah: **{min_val:.2f}**, pada **{min_row['month']}/{min_row['year']}**
- Terdapat pola musiman yang berulang, cocok digunakan untuk perencanaan pasokan

> _Detail insight dan grafik tren bisa dilihat di notebook._

---

## ✅ Rekomendasi

- **Konsumen**: Pertimbangkan untuk membeli saat quantity tinggi (harga cenderung turun)
- **Nelayan**: Optimalkan penangkapan di bulan dengan quantity tinggi
- **Pemerintah**: Pantau tren untuk mengatur kuota dan menjaga keseimbangan stok

---

## 🧠 Dukungan AI (LLM)

- **Model**: IBM Granite 3.3–8B Instruct via Replicate
- **Penggunaan**:
  - Merangkum insight statistik menjadi teks deskriptif
  - Menyusun rekomendasi otomatis dalam bahasa alami
- **Contoh Prompt**:
  > “What suggestions can be given based on data on the number of tuna fish?”

---

## 🖼️ Visualisasi

![Contoh grafik tren](path/to/grafik.png)

---

## 👩‍💻 Teknologi yang Digunakan

- Python (Pandas, Seaborn, Matplotlib)
- Langchain + Replicate (LLM Integration)
- Google Colab

---

## 📎 File Terkait

- `tokyo_wholesale_tuna_prices.csv` — Dataset utama
- `notebook.ipynb` — Analisis & prompt LLM
- `README.md` — Ringkasan proyek

---

## 📬 Kontak

- **Nama**: Asfita Saldarisya N.
- **Capstone Hacktiv8 2025**
