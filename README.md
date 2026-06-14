# Tugas Praktikum - IF603 PJJ Informatika

Repository ini berisi kumpulan berkas Jupyter Notebook (`.ipynb`) untuk memenuhi tugas mata kuliah **IF603** pada program studi **PJJ Informatika**.

## 1. Identitas Mahasiswa
* **Nama** : Raka Anggie Saputra
* **NIM** : 240401010148
* **Prodi**: PJJ Informatika
* **Kelas**: IF603

---

## 2. Ketentuan dan Aturan Tugas
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

---

## 3. Struktur dan Rangkuman Berkas Notebook

Repository ini terbagi ke dalam beberapa pertemuan praktikum dengan fokus materi sebagai berikut:

### 📑 Pertemuan 1: Dasar-Dasar Pemrograman Python
* **Fokus Utama:** Pengenalan sintaksis dasar Python.
* **Isi Konten:** * Pencetakan teks output dasar (`print()`).
  * Pendeklarasian variabel (String dan Integer) serta penerapan *f-string*.
  * Struktur data `list` dan perulangan `for` menggunakan fungsi `enumerate()`.
  * Pembuatan fungsi (*function*) khusus bernama `perkenalan()` dengan karakter pemisah pipa (`|`).

### 📑 Pertemuan 2: Eksplorasi & Manipulasi Data Awal (Titanic Dataset)
* **Fokus Utama:** Dasar-dasar *Data Wrangling* menggunakan pustaka Pandas dan NumPy.
* **Isi Konten:**
  * Memuat dataset eksternal langsung dari URL GitHub.
  * Eksplorasi dimensi data (891 baris, 12 kolom) dan pengecekan *missing values*.
  * Penyaringan (*filtering*) spesifik data penumpang wanita kelas 1.
  * Pengelompokan data (`.groupby()`) dan agregasi statistik tingkat keselamatan per kelas.

### 📑 Pertemuan 3: Visualisasi Data Statistik
* **Fokus Utama:** Pembuatan grafik menggunakan Matplotlib.
* **Isi Konten:**
  * Pengelompokan data berdasarkan kelas tiket (*Pclass*).
  * Visualisasi hubungan antara kelas tiket penumpang dan rata-rata tingkat keselamatan menggunakan grafik batang (*Bar Chart*).
  * Kustomisasi estetika grafis seperti judul (`plt.title`) dan label sumbu koordinat.

### 📑 Pertemuan 4: Pemodelan Klasifikasi Awal (Machine Learning)
* **Fokus Utama:** Alur kerja dasar pembuatan model prediktif dengan Scikit-Learn.
* **Isi Konten:**
  * Pembersihan singkat baris kosong pada kolom 'Age'.
  * Penentuan fitur prediktor (`Pclass`, `Age`) dan target (`Survived`).
  * Pembagian data (*Data Splitting*) menjadi 80% Data Latih dan 20% Data Uji.
  * Pelatihan algoritma `LogisticRegression` dan evaluasi akurasi menggunakan `accuracy_score` (Skor: ~64.3%).

### 📑 Pertemuan 5: Pembersihan Data Lanjutan (Data Cleaning)
* **Fokus Utama:** Strategi penanganan data yang hilang (*missing values*).
* **Isi Konten:**
  * Identifikasi komprehensif nilai kosong pada seluruh kolom.
  * Imputasi data numerik pada kolom 'Age' menggunakan nilai tengah (*median*).
  * Imputasi data kategorikal pada kolom 'Embarked' menggunakan nilai yang paling sering muncul (*modus*).

### 📑 Pertemuan 6: Rekayasa Fitur (Feature Engineering)
* **Fokus Utama:** Transformasi data kategorikal menjadi bentuk numerik biner.
* **Isi Konten:**
  * Penerapan teknik *One-Hot Encoding* menggunakan fungsi `pd.get_dummies()` pada kolom 'Sex' dan 'Embarked'.
  * Penggabungan dataset hasil transformasi menggunakan fungsi `pd.concat()` secara horizontal.

### 📑 Pertemuan 7: Evaluasi Model Tingkat Lanjut
* **Fokus Utama:** Analisis performa model klasifikasi secara visual.
* **Isi Konten:**
  * Rekonstruksi alur prediksi model Regresi Logistik.
  * Perhitungan matriks evaluasi melalui fungsi `confusion_matrix`.
  * Visualisasi matriks performa prediktif secara interaktif menggunakan kelas `ConfusionMatrixDisplay`.

---

## 4. Prasyarat Pustaka (Prerequisites)
Untuk menjalankan notebook yang ada di dalam repository ini, pastikan Anda telah memasang pustaka Python berikut:
```bash
pip install pandas numpy matplotlib scikit-learn
