# Analisis dan Pembuktian Representasi Citra Digital Menggunakan Python

Repositori ini berisi tugas analisis citra digital menggunakan Python dan Jupyter Notebook. Analisis dilakukan untuk membuktikan bahwa gambar digital tersusun dari pixel yang memiliki nilai numerik, dapat direpresentasikan dalam bentuk array, dan dapat direkonstruksi kembali dari susunan angka tersebut.

## Identitas

- **Nama:** Ade Ayu Wandira
- **NIM:** 24260007
- **Semester:** 5
- **Mata Kuliah:** Aplikasi Berbasis Service

## Isi Repositori

- `analisis_citra.ipynb` : Notebook berisi kode dan hasil analisis citra digital.
- `foto/IMG_20240413_053916.jpg` : Foto yang digunakan sebagai objek analisis.
- `Laporan Analisis Citra Digital Ade Ayu Wandira (24260007).pdf` : Laporan hasil analisis citra digital.
- `README.md` : Dokumentasi repositori.

## Teknologi yang Digunakan

- **Python** untuk menjalankan proses analisis.
- **Pillow (PIL)** untuk membaca gambar dan metadata EXIF.
- **NumPy** untuk mengolah array dan nilai pixel.
- **Matplotlib** untuk menampilkan gambar dan membuat visualisasi pixel.
- **Pandas** untuk menyusun dan menampilkan data dalam bentuk tabel.
- **Folium** untuk mencoba menampilkan lokasi foto pada peta interaktif.

## Tahapan Analisis

Analisis dilakukan melalui 14 tahap, yaitu:

1. Import library yang dibutuhkan.
2. Membaca citra digital.
3. Menampilkan citra digital.
4. Memeriksa informasi gambar dan metadata EXIF.
5. Membaca metadata GPS.
6. Mengubah koordinat GPS menjadi derajat desimal.
7. Membuktikan bahwa citra tersusun dari pixel.
8. Melihat nilai pixel dalam bentuk angka.
9. Menentukan beberapa koordinat pixel yang akan dianalisis, mengambil nilai RGB, dan menampilkan visualisasi warnanya.
10. Menandai letak pixel yang dianalisis pada foto asli menggunakan titik merah dan label koordinat.
11. Mengubah gambar menjadi matriks angka.
12. Membentuk kembali gambar dari array angka.
13. Memeriksa kesamaan gambar asli dan hasil rekonstruksi.
14. Menampilkan kesimpulan hasil analisis citra digital.

## Hasil Analisis

| Parameter | Hasil |
|---|---|
| Format gambar | JPEG |
| Ukuran gambar | 3264 × 2448 pixel |
| Dimensi array | `(2448, 3264, 3)` |
| Jumlah pixel | 7.990.272 |
| Kanal warna | RGB |
| Tipe data pixel | `uint8` |
| Jumlah koordinat pixel yang dianalisis | 5 |
| Hasil rekonstruksi identik | `True` |
| Status metadata GPS | Tersedia |

Analisis lima koordinat pixel menunjukkan bahwa setiap pixel memiliki posisi dan nilai RGB yang dapat diperiksa. Nilai RGB disajikan dalam tabel dan visualisasi warna, sedangkan posisi pixel ditandai langsung pada foto asli.

Hasil pemeriksaan menggunakan `np.array_equal()` menghasilkan `True`. Hal ini menunjukkan bahwa array gambar hasil rekonstruksi memiliki nilai yang identik dengan array gambar asli. Metadata GPS juga berhasil dibaca dan dikonversi menjadi koordinat desimal.

## Kesimpulan

Analisis ini menunjukkan bahwa citra digital dapat direpresentasikan sebagai susunan pixel dengan nilai numerik RGB. Python dapat digunakan untuk membaca informasi gambar, memeriksa nilai RGB pada koordinat tertentu, memvisualisasikan warna dan posisi pixel, serta merekonstruksi gambar dari array angka. Pemeriksaan kesamaan membuktikan bahwa hasil rekonstruksi identik dengan gambar asli. Selain itu, metadata EXIF dapat digunakan untuk memperoleh informasi tambahan, termasuk koordinat GPS yang tersimpan pada foto.
