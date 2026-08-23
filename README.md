# ALGORITMA K-NEAREST NEIGHBOR (KNN) UNTUK PENGENALAN TULISAN TANGAN HURUF KAPITAL X DAN Y 

Project Kecerdasan Buatan untuk melakukan klasifikasi tulisan tangan menggunakan algoritma K-Nearest Neighbor (KNN) menggunakan Jupiter Notebook.

## Deskripsi

Project ini bertujuan untuk memahami proses dasar klasifikasi citra menggunakan KNN, mulai dari preprocessing gambar, ekstraksi fitur, perhitungan jarak, hingga evaluasi akurasi tanpa menggunakan library KNN secara langsung.
Sistem digunakan untuk mengenali tulisan tangan berupa **huruf kapital X dan Y** dari citra digital.
Setiap gambar diproses menjadi citra biner berukuran 16 × 16 piksel, dengan ketentuan:
* Background putih → `1`
* Tulisan hitam → `0`

## Alur Sistem
```text
Dataset
   ↓
Pre-processing
   ↓
Grayscale
   ↓
Binerisasi
   ↓
Penebalan Garis
   ↓
Ekstraksi Nilai Pixel
   ↓
Perhitungan Jarak
   ↓
Sorting Jarak
   ↓
KNN (k = 1)
   ↓
Prediksi X / Y
   ↓
Perhitungan Akurasi
```

## Struktur Dataset

```text
dataset/
├── training/
│   ├── X/
│   │   ├── X_train_1.jpg
│   │   ├── X_train_2.jpg
│   │   └── ...
│   │
│   └── Y/
│       ├── Y_train_1.jpg
│       ├── Y_train_2.jpg
│       └── ...
│
└── testing/
    ├── X/
    │   ├── X_test_1.jpg
    │   └── ...
    │
    └── Y/
        ├── Y_test_1.jpg
        └── ...
```

## Teknologi

* **Python**
* **NumPy** — pengolahan array dan nilai piksel
* **Pillow (PIL)** — membaca dan melakukan preprocessing gambar
* **Jupyter Notebook** — Environment untuk eksekusi program

## 📄 License

This project was developed for educational purposes as part of a university final project.
