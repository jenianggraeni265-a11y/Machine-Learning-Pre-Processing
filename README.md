#  Netflix Data Preprocessing & Exploratory Data Analysis (EDA)

##  Project Overview

Proyek ini bertujuan untuk melakukan **data preprocessing** dan **exploratory data analysis (EDA)** pada dataset konten Netflix. Dataset ini mencakup informasi mengenai film dan TV show, seperti judul, sutradara, negara asal, tanggal penambahan, rating, durasi, dan genre.

Analisis ini dilakukan untuk memahami karakteristik data serta menemukan pola dan insight yang relevan.



## 📂 Dataset

Dataset yang digunakan adalah:

* `netflix_titles.csv`

Dataset ini berisi:

* Informasi konten (Movie / TV Show)
* Metadata seperti director, cast, country
* Informasi waktu (date added)
* Genre dan rating



## ⚙️ Data Preprocessing

Tahapan preprocessing yang dilakukan:

### 1. Data Understanding

* Melihat struktur dataset menggunakan `head()` dan `info()`
* Mengidentifikasi tipe data dan missing values

### 2. Handling Missing Values

* Kolom `director`, `cast`, dan `country` diisi dengan `"Unknown"`
* Baris dengan missing pada `date_added` dihapus

### 3. Data Cleaning

* Menghapus data duplikat menggunakan `drop_duplicates()`

### 4. Data Transformation

* Mengubah `date_added` menjadi format datetime
* Membuat kolom baru:

  * `year_added`
  * `month_added`
* Mengubah `listed_in` menjadi list (split genre)
* Encoding variabel `type` (Movie = 0, TV Show = 1)



##  Exploratory Data Analysis (EDA)

Beberapa analisis yang dilakukan:

###  Distribusi Tipe Konten

Mayoritas konten di Netflix adalah **Movie** dibandingkan TV Show.

###  Tren Penambahan Konten

Terjadi peningkatan signifikan jumlah konten terutama setelah tahun 2015.

###  Negara Produksi

Sebagian besar konten berasal dari **Amerika Serikat**.

###  Distribusi Rating

Konten didominasi oleh rating **TV-MA** dan **TV-14**, yang menunjukkan target penonton dewasa.

###  Analisis Genre

Genre paling populer:

* Drama
* Comedy



## 📌 Key Insights

* Netflix lebih banyak menyediakan film dibandingkan TV show
* Pertumbuhan konten meningkat pesat setelah 2015
* Amerika Serikat menjadi kontributor utama
* Genre drama dan komedi mendominasi
* Mayoritas konten ditujukan untuk penonton dewasa




Project ini dibuat untuk keperluan pembelajaran data preprocessing dan eksplorasi data dalam konteks analisis data nyata.

---
