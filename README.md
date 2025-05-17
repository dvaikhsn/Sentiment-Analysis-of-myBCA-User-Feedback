# Analisis Sentimen Ulasan Pengguna Aplikasi myBCA

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap ulasan pengguna aplikasi **myBCA** menggunakan teknik **Natural Language Processing (NLP)**. Ulasan diklasifikasikan ke dalam tiga kategori sentimen: **positif**, **netral**, dan **negatif** untuk memberikan wawasan terhadap pengalaman pengguna dan sebagai bahan evaluasi pengembangan aplikasi.

## 🎯 Tujuan Proyek

- Mengumpulkan dan membersihkan data ulasan pengguna aplikasi myBCA.
- Melakukan preprocessing teks menggunakan teknik NLP.
- Membangun model machine learning untuk klasifikasi sentimen.
- Mengevaluasi performa model dan menyajikan hasil dalam bentuk visualisasi.

## 📁 Dataset

- Sumber: Ulasan pengguna aplikasi **myBCA** dari Google Play Store (melalui scraping atau file CSV).
- Jumlah data: ±20.000 ulasan
- Label sentimen: `Positif`, `Netral`, `Negatif` 


## 🧹 Tahapan Preprocessing

- Mengubah huruf menjadi huruf kecil (lowercasing)
- Menghapus tanda baca dan stopwords
- Tokenisasi
- Lematisasi
- Encoding label sentimen

## 🤖 Model yang Digunakan

- Logistic Regression  
- Random Forest 
- Support Vector Machine (SVM)

## 📊 Evaluasi

- Akurasi Training Logistic Regression: 87%
- Akurasi Training Random Forest: 89%
- Akurasi Training Support Vector Machine: 91%

## 📈 Hasil 
Berdasarkan ke 3 model machine learning tersebut didapatkan analisis:
1. Algoritma Logistic Regression
Akurasi yang didapatkan dari algoritma ini yaitu 87.18%. Berdasarkan performa cukup baik dan stabil di semua kelas. Kemudian algoritma ini juga ringan dan cepat untuk dilatih.
Kekurangannya adalah kurang untuk mengenali kelas Negatif (recall hanya 0.78),artinya masih ada banyak ulasan negatif yang salah ketika diklasifikasikan.

2. Algoritma Random Forest
Akurasi yang didapatkan dari algoritma ini yaitu 89.75%. Berdasarkan performa ada peningkatan dari algoritma Logistic Regression. Yaitu lebih baik dalam mendeteksi kelas Negatif (recall 0.86) dan Positif (recall 0.91).
Kekurangannya adalah kalo datasetnya banyak/besar pasti lebih lambat ketika proses latihnya dibandingkan algoritma Logistic Regression.

3. Algoritma Support Vector Machine (SVM)
Akurasi yang didapatkan dari algoritma ini yaitu 91.79%. Berdasarkan performa, algoritma ini paling akurat di antara dua algoritma sebelumnya. Kemudian algorima ini sangat baik dalam mengenali semua kelas, terutama Positif (precision 0.97).
