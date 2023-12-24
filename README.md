# Klasifikasi Gambar Tangan: Kertas, Gunting, Batu dengan TensorFlow


## Deskripsi
Projek ini merupakan implementasi klasifikasi gambar tangan menggunakan TensorFlow. Model ini dibuat menggunakan Convolutional Neural Network (CNN) untuk mengenali gestur kertas, gunting, dan batu.

## Dataset
Dataset yang digunakan dapat diunduh dari [tautan ini](https://github.com/dicodingacademy/assets/releases/download/release/rockpaperscissors.zip). Dataset ini terdiri dari gambar-gambar dalam kategori kertas, gunting, dan batu.

Dataset yang digunakan dapat diunduh dan diekstrak menggunakan kode berikut:

``` python
!wget --no-check-certificate \
  https://github.com/dicodingacademy/assets/releases/download/release/rockpaperscissors.zip \
  -O /tmp/rockpaperscissors.zip
  
import zipfile, os
local_zip = '/tmp/rockpaperscissors.zip'
zip_ref = zipfile.ZipFile(local_zip, 'r')
zip_ref.extractall('/tmp')
zip_ref.close()

base_dir = '/tmp/rockpaperscissors/rps-cv-images'
train_dir = '/content/output/train'
validation_dir = '/content/output/val' 

``` 
## Langkah-Langkah Eksekusi

### 1. Persiapan Lingkungan
Pastikan Anda telah menginstal TensorFlow dan Jupyter Notebook.

### 2. Persiapan Dataset
- Unduh dataset dari tautan yang disediakan di atas.
- Ekstrak file `rockpaperscissors.zip` dan atur struktur direktori seperti yang dijelaskan di atas.
- Atau gunakan kode di atas untuk mengunduh dan mengekstrak dataset.

### 3. Jalankan Notebook
- Buka Jupyter Notebook dengan menjalankan `Submission_ML.ipynb`.
- Ikuti langkah-langkah pada notebook untuk melatih model, mengevaluasi performa, dan menggunakan model untuk klasifikasi gambar tangan.

## Fitur Tambahan

Selain klasifikasi gambar tangan dari dataset yang ada, notebook ini juga menyediakan fitur untuk mengunggah gambar dan mendapatkan prediksi klasifikasi untuk gambar yang diunggah.

## Referensi

- [Dicoding Academy - Belajar Machine Learning untuk Pemula](https://www.dicoding.com/academies/184)
- Buku: Deep Learning with TensorFlow

## Catatan
File ini juga dapat dijalankan di Google Colab

