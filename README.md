# 📱 Sentiment Analysis on MyTelkomsel App Reviews

Proyek ini merupakan implementasi Natural Language Processing (NLP) untuk melakukan **analisis sentimen** terhadap ulasan pengguna aplikasi **MyTelkomsel** yang diambil dari Google Play Store. Tujuan utama dari proyek ini adalah mengidentifikasi opini pengguna terhadap aplikasi berdasarkan ulasan yang mereka berikan, apakah bersifat **positif**, **netral**, atau **negatif**.

---

## 🚀 Fitur Utama

- ✅ Scraping data ulasan MyTelkomsel secara otomatis
- ✅ Pra-pemrosesan teks untuk membersihkan dan menyiapkan data
- ✅ Labeling sentimen (positif, netral, negatif)
- ✅ Visualisasi data seperti Word Cloud dan distribusi label
- ✅ Pelatihan model dengan berbagai algoritma (SVM, Random Forest, LSTM)
- ✅ Evaluasi model dan inference untuk klasifikasi ulasan baru
- ✅ File `requirements.txt` dan struktur proyek siap pakai

---

## 🛠 Teknologi yang Digunakan

- Python 3.11+
- pandas, numpy
- scikit-learn
- TensorFlow / Keras
- matplotlib, seaborn
- wordcloud
- Google Play Scraper (custom atau `google-play-scraper`)

---

## 📊 Visualisasi

Beberapa Word Cloud yang dihasilkan dari dataset:

![Word Cloud All](assets/wordcloud_all.png)

---

## 🔍 Akurasi Model

| Algoritma | Akurasi (Testing) | Akurasi (Training) |
|-----------|-------------------|---------------------|
| SVM       | 89.21%            | 90.45%              |
| RandomForest | 87.83%         | 99.20%              |
| LSTM      | 85.08%            | 91.61%              |

---

## 🧪 Inference

Contoh hasil prediksi sentimen:

```text
Input: "Aplikasi lambat dan sering force close."
Prediksi: Negatif
