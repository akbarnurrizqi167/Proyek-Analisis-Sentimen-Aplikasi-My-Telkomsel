# 📊 Analisis Sentimen Ulasan Aplikasi MyTelkomsel

Proyek ini merupakan implementasi dari Natural Language Processing (NLP) untuk melakukan analisis sentimen terhadap ulasan pengguna aplikasi **MyTelkomsel** yang diambil dari Google Play Store. Klasifikasi sentimen dilakukan ke dalam tiga kategori: **positif**, **netral**, dan **negatif**.

---

## 📝 Deskripsi Proyek

Analisis sentimen adalah proses untuk mengidentifikasi opini atau emosi dari suatu teks. Dalam konteks ini, proyek bertujuan untuk:
- Memahami persepsi pengguna terhadap aplikasi MyTelkomsel.
- Mengklasifikasikan ulasan berdasarkan sentimen.
- Membangun model machine learning dan deep learning yang mampu memprediksi sentimen dari data ulasan.

---

## 🛠️ Alur Proyek

### 1. Web Scraping
Pengambilan data ulasan dari Google Play Store menggunakan Python. Data disimpan dalam format `.csv` untuk proses selanjutnya.

### 2. Preprocessing
Pembersihan dan normalisasi teks dilakukan dengan langkah-langkah:
- Menghapus karakter khusus dan emoji
- Menghapus stopwords
- Tokenisasi
- Lowercasing
- Normalisasi kata tidak baku

### 3. Pelabelan Data
Pelabelan dilakukan secara semi-manual dan dengan bantuan kamus sentimen, untuk menghasilkan data dengan tiga label: `positif`, `netral`, dan `negatif`.

### 4. Visualisasi Data
Distribusi label divisualisasikan, serta dibuat Word Cloud untuk memahami kata yang sering muncul dalam masing-masing kelas sentimen.

### 5. Ekstraksi Fitur
Transformasi teks menjadi fitur numerik menggunakan:
- TF-IDF (untuk model klasik)
- Tokenizer + Padding (untuk LSTM)

### 6. Pelatihan Model
Dilakukan 3 percobaan dengan kombinasi:
- SVM + TF-IDF (80/20 split)
- Random Forest + TF-IDF (70/30 split)
- LSTM + Tokenizer (80/20 split)

### 7. Evaluasi
Model diuji menggunakan metrik:
- Akurasi
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📈 Hasil

- **Jumlah Data**: 18.000+ ulasan  
- **Kelas**: Positif, Netral, Negatif  
- **Akurasi Tertinggi**: >92% (LSTM)  
- **Model Deep Learning**: LSTM dengan hasil optimal  
- **Visualisasi**: Word Cloud dan distribusi label  

---

## ✅ Kriteria yang Dipenuhi
✔️ Menggunakan algoritma Deep Learning (LSTM)
✔️ Akurasi training dan testing > 92%
✔️ Dataset terdiri dari 3 kelas sentimen
✔️ Dataset memiliki lebih dari 10.000 data ulasan
✔️ Menerapkan 3 skema pelatihan model
✔️ Menyertakan visualisasi data (Word Cloud)

## 🎯 Manfaat
1. Memberikan insight terkait kepuasan atau keluhan pengguna terhadap aplikasi
2. Menunjukkan pemahaman praktik NLP dan supervised learning dalam bahasa Indonesia
3. Dapat dikembangkan sebagai dasar monitoring opini pengguna terhadap produk digital

## 🧠 Teknologi yang Digunakan
- Python (pandas, sklearn, tensorflow, matplotlib, seaborn)
- Natural Language Toolkit (nltk)
- TensorFlow & Keras
- Scikit-Learn
- BeautifulSoup
- WordCloud


