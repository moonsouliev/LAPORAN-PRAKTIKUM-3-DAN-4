# Viana Salsabila Fairuz Syahla
# 202231027
# Praktikum 3: Deteksi Tepi dan Garis

Praktikum ini berfokus pada teori di balik deteksi tepi dan garis pada gambar menggunakan algoritma pemrosesan citra. Kami menggunakan berbagai teknik dari OpenCV untuk memproses gambar dan mendeteksi fitur penting.

Deteksi tepi dan garis adalah dua tugas penting dalam pemrosesan citra yang digunakan untuk mengekstraksi informasi geometris dari gambar. Tepi biasanya mewakili batas antara dua wilayah yang berbeda dalam gambar, sementara garis dapat mewakili struktur linear yang signifikan.

## Deteksi Tepi

Deteksi tepi bertujuan untuk mengidentifikasi titik-titik dalam gambar di mana intensitas berubah secara drastis. Algoritma yang umum digunakan untuk deteksi tepi adalah algoritma Canny.

### Algoritma Canny

Algoritma Canny adalah metode multi-tahap yang digunakan untuk mendeteksi tepi dalam gambar. Tahapan utamanya meliputi:

1. **Pengaburan**: Menghaluskan gambar menggunakan filter Gaussian untuk mengurangi noise.
2. **Gradien Intensitas**: Menghitung gradien intensitas gambar untuk menemukan arah dan besar perubahan intensitas.
3. **Non-Maximum Suppression**: Menekan semua piksel yang bukan merupakan maksimum lokal di sepanjang arah gradien.
4. **Double Thresholding**: Menerapkan dua ambang batas untuk mengidentifikasi tepi kuat dan lemah.
5. **Edge Tracking by Hysteresis**: Menghubungkan tepi lemah yang terhubung dengan tepi kuat.

### Perkiraan Nilai Ambang Batas

Pemilihan nilai ambang batas atas dan bawah sangat penting dalam algoritma Canny. Ambang batas yang terlalu rendah akan menyebabkan banyak noise terdeteksi sebagai tepi, sementara ambang batas yang terlalu tinggi akan menghilangkan banyak tepi sebenarnya. Nilai ambang batas biasanya dipilih berdasarkan eksperimen atau menggunakan metode otomatis.

## Deteksi Garis

Setelah tepi terdeteksi, langkah selanjutnya adalah mendeteksi garis dalam gambar menggunakan Transformasi Hough.

### Transformasi Hough

Transformasi Hough adalah teknik yang digunakan untuk mendeteksi bentuk geometris, seperti garis, dalam gambar biner (gambar yang hanya berisi piksel hitam dan putih). Prinsip dasar Transformasi Hough adalah mengkonversi masalah deteksi garis dari domain gambar ke domain parameter.

1. **Ruang Hough**: Setiap garis dalam gambar direpresentasikan sebagai satu titik dalam ruang parameter (ρ, θ).
2. **Voting**: Setiap piksel tepi dalam gambar memberikan suara pada semua kemungkinan garis yang melewatinya dalam ruang parameter.
3. **Deteksi Puncak**: Garis yang paling signifikan dalam gambar diidentifikasi sebagai puncak dalam ruang parameter.

### Parameter Transformasi Hough

- **ρ (rho)**: Jarak dari titik asal (biasanya sudut kiri atas gambar) ke garis.
- **θ (theta)**: Sudut antara sumbu x dan garis yang tegak lurus terhadap garis yang akan dideteksi.
- **Threshold**: Jumlah suara minimum yang diperlukan untuk menganggap suatu garis ada.

## Kesimpulan

Dalam praktikum ini, kami mempelajari teori di balik deteksi tepi menggunakan algoritma Canny dan deteksi garis menggunakan Transformasi Hough. Pemahaman yang baik tentang parameter dan tahapan dalam kedua algoritma ini sangat penting untuk mengoptimalkan deteksi fitur dalam gambar.


