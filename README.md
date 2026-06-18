# Eksperimen Operasi Dasar pada Sinyal 1D dan Citra 2D

link github :

**Nama Mahasiswa:** Suryatama Widyadhana

## Deskripsi Singkat Project

Proyek ini berisi implementasi eksperimen berbasis Python untuk menerapkan operasi dasar pengolahan sinyal digital, yaitu operasi penjumlahan, penggeseran (translasi), dan amplifikasi pada sinyal diskrit 1D serta matriks citra 2D. Proyek ini juga menguji konsep dasar sistem linier melalui pembuktian sifat homogenitas dan additivitas, sekaligus menyertakan analisis aplikatifnya di dunia nyata seperti pada kasus _audio mixing_ dan augmentasi data.

## Library yang Digunakan

- `NumPy`: Untuk komputasi operasi array matematis pada sinyal 1D.
- `Matplotlib`: Untuk memvisualisasikan plot gelombang diskrit dan menampilkan citra serta histogram.
- `OpenCV` (`cv2`): Untuk membaca, memanipulasi, dan mentransformasikan ruang warna pada citra 2D.

## Cara Menjalankan Notebook

1. Pastikan Python sudah terinstal dengan baik di perangkat Anda.
2. Buka terminal atau _command prompt_, lalu instal semua _library_ yang dibutuhkan dengan perintah:
   `pip install -r requirements.txt`
3. Buka file `operasi_sinyal_citra.ipynb` yang berada di dalam folder `notebook/` menggunakan Jupyter Notebook, Visual Studio Code, atau unggah ke Google Colab.
4. Jalankan (_Run All_) sel kode secara berurutan dari atas ke bawah untuk melihat hasil perbandingan dan visualisasi grafiknya.

## Struktur Folder Project

```text
operasi-dasar-sinyal-citra/
|-- notebook/
|   |-- operasi_sinyal_citra.ipynb
|-- images/
|   |-- citra_yang_digunakan.jpg
|-- report/
|   |-- laporan.pdf
|-- README.md
|-- requirements.txt

## Ringkasan Hasil Eksperimen
Eksperimen membuktikan bahwa fungsi linear dasar mendukung properti superposisi melalui pemenuhan syarat homogenitas (amplifikasi) dan additivitas (penjumlahan). Pada domain citra 2D, memanipulasi matriks piksel sering kali memicu risiko data yang melampaui batas maksimum kapasitas (misalnya >255). Oleh karena itu, pengolahan gambar selalu membutuhkan teknik mitigasi tambahan berupa pemotongan nilai (clipping) atau penyekalaan ulang (normalisasi) agar tidak memunculkan artifak warna.

## Kesimpulan Singkat
Memanipulasi nilai array dan matriks secara spasial maupun temporal melalui operasi aritmatika dan aljabar merupakan fondasi utama yang menyusun fungsionalitas sistem Pengolahan Sinyal Digital di dunia nyata, mulai dari simulasi delay sistem hingga filter manipulasi gambar.
```
