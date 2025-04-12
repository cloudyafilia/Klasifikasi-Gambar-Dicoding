# 👟 Klasifikasi Gambar Jenis Alas Kaki Menggunakan Deep Learning

## 📝 Penjelasan Proyek
  Dataset yang digunakan adalah dataset Kaggle yang tersedia secara publik dan berisi gambar berbagai jenis alas kaki seperti sepatu, sandal, dan boot. Dataset ini dapat diakses melalui link berikut:
[https://www.kaggle.com/datasets/hasibalmuzdadid/shoe-vs-sandal-vs-boot-dataset-15k-images]

  Proyek ini mengimplementasikan model klasifikasi gambar menggunakan arsitektur Convolutional Neural Networks (CNN) dengan TensorFlow dan Keras untuk mengidentifikasi jenis alas kaki berdasarkan gambar.

  Kelas yang dikenali dalam dataset ini antara lain:
- Boot
- Sandal
- Shoe

  Model dilatih menggunakan dataset citra alas kaki yang telah melalui preprocessing seperti augmentasi, normalisasi, dan penskalaan ulang untuk meningkatkan performa serta generalisasi.

---

## 📂 Struktur Proyek
1. `notebook.ipynb:` Notebook utama yang mencakup seluruh proses (pemrosesan data, pelatihan model, evaluasi, dan ekspor)
2. `saved_model/`: Model yang disimpan dalam format TensorFlow SavedModel
3. `tflite/`: Model dalam format TensorFlow Lite, cocok untuk perangkat edge
4. `tfjs_model/`: Model dalam format TensorFlow.js untuk digunakan di browser
5. `requirements.txt`: Daftar pustaka Python yang diperlukan

---

## 🧠 Fitur Utama

1. Dataset berisi lebih dari 10000 gambar alas kaki yang telah dilabeli
2. Pembagian data 80% untuk training, 10% untuk validasi, dan 10% untuk testing
3. Arsitektur CNN kustom dengan lapisan Conv2D, MaxPooling, Flatten, dan Dense
4. Augmentasi data (rotasi, zoom, pergeseran, dll) untuk meningkatkan generalisasi model
5. Model diekspor dalam tiga format untuk berbagai kebutuhan deployment

---

## 📊 Detail Pelatihan

1. Arsitektur Model: CNN Sequential
2. Target Akurasi: lebih dari 95%
3. Optimizer: Adam
4. Fungsi Loss: Categorical Crossentropy
5. Callback: EarlyStopping dan ReduceLROnPlateau untuk pelatihan yang optimal

---

## 🔍 Cara Menjalankan

1. Buka file `notebook.ipynb` di Google Colab atau Jupyter Notebook
2. Pastikan dataset sudah diunggah atau dipasang (mount)
3. Instalasi pustaka yang dibutuhkan
4. Jalankan setiap sel notebook secara berurutan
5. Ubah jalur dataset jika dijalankan secara lokal

---
