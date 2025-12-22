# Crowd_detection_ComputerVision_Final_project

Repositori ini berisi pengembangan sistem deteksi manusia pada citra lingkungan pusat perbelanjaan (mall) menggunakan Histogram of Oriented Gradients (HOG) sebagai metode ekstraksi fitur dan Support Vector Machine (SVM) sebagai metode klasifikasi.
Pendekatan yang digunakan adalah sliding window untuk mendeteksi keberadaan manusia pada berbagai area citra.

Saat ini, repositori difokuskan pada penyediaan struktur dataset, example data, serta perencanaan eksperimen. Implementasi model dan hasil eksperimen akan ditambahkan secara bertahap.

# Gambaran Umum Proyek

Tujuan proyek ini adalah menerapkan dan membandingkan beberapa pendekatan berbasis fitur untuk tugas deteksi manusia menggunakan metode computer vision klasik.
Setiap citra akan dipindai menggunakan sliding window, kemudian fitur diekstraksi dan diklasifikasikan sebagai manusia atau bukan manusia menggunakan SVM.

Pendekatan yang digunakan dalam proyek ini meliputi:
1. HOG + SVM
2. HOG + SIFT + SVM
3. OpenCV HOG + SVM

# Deskripsi Dataset:
Dataset yang digunakan merupakan dataset kustom yang disusun dari citra pengawasan mall. Dataset ini diorganisasikan ke dalam beberapa kategori untuk mendukung proses pelatihan, pengujian, dan visualisasi hasil. Karena keterbatasan penyimpanan GitHub, repositori ini hanya menyertakan contoh gambar dari setiap kategori. Dataset lengkap disediakan melalui Google Drive.

# Struktur Dataset:
a. positive_samples/
Potongan citra yang mengandung manusia dan digunakan sebagai data positif untuk pelatihan model.
b. negative_samples/
Potongan citra latar belakang tanpa manusia, digunakan sebagai data negatif.
c. raw_images/
Citra asli lingkungan mall sebelum dilakukan pemrosesan atau cropping.
d. test_images/
Citra yang digunakan untuk pengujian performa sistem deteksi.

# Results

# Dataset lengkap:
Dataset lengkap, model hasil pelatihan, serta hasil eksperimen penuh dapat diakses melalui Google Drive berikut:
https://drive.google.com/drive/folders/1YXt4e_HpvbYc7VrK1ymc4zh-q_DeH_qX
