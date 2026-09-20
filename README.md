# Analisis Penjualan & Break-Even Point (BEP) Gerai Donat

Repositori ini berisi proyek analisis data kinerja penjualan harian dan perhitungan *Break-Even Point* (BEP) dari beberapa gerai donat menggunakan bahasa pemrograman Python. Proyek ini disusun sebagai bagian dari tugas mata kuliah **Analisis Numerik**.


## Deskripsi Proyek
Analisis ini menggunakan dataset sintetis harian (`sintesis_data_donat_harian.csv`) yang mencakup operasional dari 5 gerai donat berbeda (Gerai A sampai Gerai E) selama periode waktu tertentu. Melalui pendekatan komputasi menggunakan Python, data ini diolah untuk mengevaluasi kesehatan finansial tiap gerai dengan membandingkan pendapatan kotor terhadap total biaya (biaya variabel dan biaya tetap harian) guna menentukan margin keuntungan (*balance*) serta titik impas operasionalnya.

---

## Tujuan Analisis
1. Melakukan eksplorasi data (*Exploratory Data Analysis*) terhadap catatan penjualan harian gerai donat.
2. Memahami komponen finansial gerai yang terdiri dari Harga Jual, Jumlah Terjual, Pendapatan Kotor, Biaya Variabel, dan *Fixed Cost* Harian.
3. Menganalisis tingkat profitabilitas harian (*balance*) di masing-masing gerai.
4. Memvisualisasikan hubungan antara jumlah unit penjualan dan pendapatan (*revenue*) menggunakan pustaka visualisasi data Python.

---

## Tech Stack & Library
Proyek ini dikembangkan menggunakan **Python** dengan bantuan beberapa pustaka (*libraries*) utama:
* **Pandas** : Manipulasi dan analisis struktur data tabular (*DataFrame*).
* **NumPy** : Komputasi numerik dan operasi array.
* **Matplotlib** : Visualisasi data berupa grafik sebar (*scatter plot*) penjualan vs pendapatan.
* **Scikit-Learn** : Pemodelan regresi linier (*Linear Regression*) untuk analisis tren.

---

## Ringkasan Statistik Data
Berdasarkan hasil eksekusi program pada data operasional gerai:
* **Total Sampel Data**: 450 catatan harian.
* **Daftar Gerai**: Gerai A, Gerai B, Gerai C, Gerai D, dan Gerai E.
* **Rentang Harga Jual**: Rp8.000 hingga Rp25.000 per unit.
* **Jumlah Terjual**: Berkisar antara 81 hingga 710 unit per hari.
* **Rata-rata Pendapatan Kotor**: Rp3.342.420 per hari.
* **Rata-rata Keuntungan/Balance**: Rp391.997 per hari (dengan catatan beberapa hari mengalami rugi/negatif sebelum melewati titik BEP).

---

## Hasil Analisis & Visualisasi
1. **Fluktuasi Kinerja Finansial**: Dari kolom `Balance (Rp)`, terlihat bahwa beberapa hari operasional mengalami kerugian (nilai negatif) dikarenakan jumlah unit terjual belum mampu menutup *Fixed Cost* harian dan biaya variabel. Sebaliknya, pada volume penjualan tinggi, gerai mampu menghasilkan keuntungan bersih hingga jutaan rupiah.
2. **Visualisasi Penjualan vs Revenue**: Berdasarkan grafik *scatter plot* yang dihasilkan per masing-masing gerai, terdapat korelasi linier yang positif dan kuat antara jumlah unit donat yang terjual dengan total pendapatan kotor (*revenue*) yang diperoleh. Semakin tinggi unit yang terjual, garis pendapatan naik secara proporsional sesuai dengan harga satuan masing-masing gerai.
