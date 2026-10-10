# Analisis dan Pembuktian Representasi Citra Digital Menggunakan Python

Repositori ini berisi tugas analisis citra digital menggunakan Python dan Jupyter Notebook. Tujuannya adalah membuktikan bahwa gambar digital tersusun dari pixel yang memiliki nilai numerik dan dapat direkonstruksi kembali dari array angka.

## Identitas

- **Nama:** Ade Ayu Wandira
- **NIM:** 24260007
- **Semester:** 5
- **Mata Kuliah:** Aplikasi Berbasis Service

## Isi Repositori

- `analisis_citra.ipynb` : Notebook berisi kode dan hasil analisis citra digital.
- `foto/IMG_20240413_053916.jpg` : Gambar yang digunakan sebagai objek analisis.
- `Laporan Analisis Citra Digital Ade Ayu Wandira (24260007).pdf` : Laporan lengkap hasil analisis.
- `README.md` : Dokumentasi repositori.

## Teknologi yang Digunakan

- **Python** untuk menjalankan analisis.
- **Pillow (PIL)** untuk membaca gambar dan metadata EXIF.
- **NumPy** untuk mengolah array dan nilai pixel.
- **Matplotlib** untuk menampilkan gambar.
- **Pandas** untuk menyajikan data dalam bentuk tabel.
- **Folium** untuk mencoba menampilkan lokasi foto pada peta interaktif.

## Tahapan Analisis

Analisis dilakukan melalui 13 tahap, meliputi:

1. Membaca dan menampilkan citra digital.
2. Memeriksa informasi gambar dan metadata EXIF.
3. Membaca metadata GPS dan mengonversi koordinat ke derajat desimal.
4. Mengubah gambar menjadi array NumPy.
5. Memeriksa nilai pixel dan kanal warna RGB.
6. Menampilkan sebagian pixel dalam bentuk tabel dan matriks.
7. Membentuk kembali gambar dari array angka.
8. Memeriksa kesamaan gambar asli dan hasil rekonstruksi.
9. Menampilkan ringkasan hasil analisis citra dan metadata GPS.

## Hasil Analisis

| Parameter                  | Hasil             |
| -------------------------- | ----------------- |
| Format gambar              | JPEG              |
| Ukuran gambar              | 3264 × 2448 pixel |
| Jumlah pixel               | 7.990.272         |
| Kanal warna                | RGB               |
| Tipe data                  | `uint8`           |
| Hasil rekonstruksi identik | `True`            |
| Status metadata GPS        | Tersedia          |

Hasil analisis membuktikan bahwa gambar digital dapat direpresentasikan sebagai array numerik dengan tiga kanal warna RGB. Pemeriksaan menggunakan `np.array_equal()` menghasilkan `True`, yang menunjukkan bahwa gambar hasil rekonstruksi memiliki nilai pixel yang identik dengan gambar asli.

## Kesimpulan

Citra digital dapat direpresentasikan sebagai susunan pixel dengan nilai numerik RGB. Melalui Python, nilai pixel dapat dianalisis dalam bentuk array dan matriks, kemudian digunakan untuk merekonstruksi gambar. Hasil pemeriksaan menunjukkan bahwa gambar hasil rekonstruksi identik dengan gambar asli. Analisis ini juga menunjukkan bahwa metadata EXIF dapat menyimpan informasi tambahan, termasuk koordinat GPS.
