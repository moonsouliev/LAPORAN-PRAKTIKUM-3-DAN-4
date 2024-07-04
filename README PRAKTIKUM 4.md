### Praktikum 4: Analisis Tekstur Gambar Menggunakan GLCM

Gray Level Co-occurrence Matrix (GLCM) adalah salah satu metode untuk menganalisis tekstur gambar. Metode ini menghitung frekuensi pasangan pixel dengan intensitas tertentu yang muncul dalam gambar pada jarak dan sudut tertentu. GLCM kemudian dapat digunakan untuk menghitung berbagai fitur tekstur yang memberikan informasi tentang variasi dan pola dalam gambar.

#### Tujuan
Tujuan dari praktikum ini adalah untuk memahami dan menerapkan metode GLCM dalam analisis tekstur gambar. Kita akan menghitung beberapa fitur tekstur menggunakan GLCM dan menginterpretasikan hasilnya.

#### Teori Dasar
1. **Gray Level Co-occurrence Matrix (GLCM)**
   GLCM adalah matriks yang menunjukkan seberapa sering kombinasi piksel dengan nilai tertentu (intensitas) muncul dalam gambar. Matriks ini dibangun dengan mempertimbangkan pasangan piksel pada jarak dan sudut tertentu.

2. **Fitur Tekstur**
   Dari GLCM, kita dapat mengekstrak berbagai fitur tekstur yang dapat digunakan untuk menganalisis pola dalam gambar. Fitur-fitur ini meliputi:
   - **Contrast**: Mengukur intensitas kontras antara piksel dan tetangganya. Nilai kontras yang tinggi menunjukkan variasi intensitas yang besar dalam gambar.
   - **Dissimilarity**: Mengukur variasi lokal dalam gambar.
   - **Homogeneity**: Mengukur kedekatan distribusi elemen dalam GLCM ke diagonal GLCM. Nilai homogeneity yang tinggi menunjukkan gambar yang lebih halus.
   - **Energy**: Mengukur keseragaman distribusi GLCM. Nilai energy yang tinggi menunjukkan tekstur yang seragam.
   - **Correlation**: Mengukur hubungan linear antara piksel dalam jarak tertentu.

#### Langkah-langkah Analisis
1. **Membaca Gambar**: Gambar akan dibaca dan dikonversi ke dalam format HSV.
2. **Membangun GLCM**: Matriks GLCM akan dibangun dengan mempertimbangkan jarak dan sudut tertentu.
3. **Menghitung Fitur Tekstur**: Menggunakan GLCM yang telah dibangun, fitur-fitur tekstur seperti contrast, dissimilarity, homogeneity, energy, dan correlation akan dihitung.
4. **Interpretasi Hasil**: Hasil perhitungan fitur tekstur akan diinterpretasikan untuk memahami pola dan variasi dalam gambar.

#### Hasil dan Pembahasan
Hasil dari perhitungan fitur tekstur akan memberikan wawasan tentang variasi intensitas dan pola dalam gambar. Misalnya, nilai contrast yang tinggi menunjukkan adanya perbedaan intensitas yang signifikan, sedangkan nilai homogeneity yang tinggi menunjukkan gambar yang lebih halus dan seragam.

#### Kesimpulan
Metode GLCM adalah alat yang kuat untuk analisis tekstur gambar. Dengan menghitung fitur-fitur tekstur dari GLCM, kita dapat mengidentifikasi dan menginterpretasikan pola-pola dalam gambar yang tidak dapat dilihat dengan penglihatan langsung. Praktikum ini memberikan pemahaman dasar tentang bagaimana GLCM bekerja.
