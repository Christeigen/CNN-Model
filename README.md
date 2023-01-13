# CNN-Model
Dataset diperoleh melalui scrapping dari platform Shopee dengan menggunakan beberapa kata kunci yang berhubungan dengan fashion.
Data yang diperoleh kemudian dilabel secara manual berdasarkan ketentuan shopee sebagai berikut:
- Foto baju yang terpotong, pencahayaannya tidak jelas, bajunya terlipat, dan tidak merepresentasikan produk akan dikategorikan sebagai 1 (cukup baik)
- Foto baju yang ditampilkan dengan pencahayaan yang baik, seluruh bagian terlihat, namun belum memiliki model akan dikategorikan sebagai 2 (baik)
- Foto baju yang sudah memenuhi kriteria poin kedua dan memiliki model, akan dikategorikan sebagai 3 (sangat baik)

Dataset yang terkumpul sebanyak 3724 foto, dengan 1131 foto dengan kategori cukup baik, 1212 foto dengan kategori baik, dan 1381 foto dengan kategori sangat baik.
Foto dalam dataset diubah menjadi hitam putih, agar perbedaan warna tidak dijadikan sebagai indikator penilaian oleh artificial intelligence.
Karena jumlah dataset yang minim, dilakukan data augmentation dengan melakukan zoom in, zoom out, rotate, dan flip pada keseluruhan foto, dengan hasil akhir sebanyak 7448 foto yang dijadikan sebagai bahan train dan 4497 foto yang dijadikan test dari model kami
Dengan menggunakan algoritma CNN didapatkan akurasi sekitar 79%. Dalam implementasi kedepannya dapat menggunakan lebih banyak dataset untuk memperkuat dan menaikkan akurasi dari model.
