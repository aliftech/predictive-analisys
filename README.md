# Laporan Proyek Machine Learning Predictive Analisys - Wahyu Krisna Aji

## Domain Proyek

Pinjaman bank adalah bagian integral dari kegiatan perbankan dan memiliki implikasi besar baik bagi peminjam maupun institusi keuangan. Status pinjaman yang tidak tepat dapat mengakibatkan risiko kredit yang tinggi, kerugian finansial, dan ketidakpuasan pelanggan. Oleh karena itu, penting untuk mengembangkan metode yang akurat dan efisien untuk memprediksi status pinjaman guna membantu pengambilan keputusan yang lebih baik di industri perbankan.

## Business Understanding

Proyek ini dibabgun untuk perusahaan dengan karakteristik bisnis sebagai berikut :

- Perusahaan yang bergerak dalam bidang perbankan dan industri finansial.

### Problem Statements

Beberapa tantangan yang perlu dipecahkan dalam masalah ini termasuk:

- Kompleksitas faktor-faktor penentu: Pengambilan keputusan kredit yang akurat memerlukan pemahaman mendalam tentang faktor-faktor yang mempengaruhi kemampuan seseorang untuk membayar kembali pinjaman. Faktor seperti riwayat kredit, pendapatan, riwayat pekerjaan, aset, dan variabel lainnya harus dianalisis dengan cermat untuk membuat prediksi yang akurat.

- Risiko kredit: Salah satu risiko utama yang dihadapi oleh bank adalah gagal bayar pinjaman. Mengidentifikasi aplikasi yang berpotensi berisiko tinggi dan mengurangi risiko kredit menjadi sangat penting untuk menjaga stabilitas keuangan bank.

### Goals

- Fokus pada area yang perlu diperbaiki: Dengan mengidentifikasi masalah dengan jelas, kita dapat menentukan area yang membutuhkan perhatian dan peningkatan. Hal ini membantu mengarahkan upaya dan sumber daya untuk memecahkan masalah yang paling penting dalam prediksi status pinjaman.

- Mengarahkan perancangan solusi: Pernyataan masalah membantu mengarahkan perancangan solusi yang sesuai. Dengan memahami masalah dengan baik, kita dapat merumuskan pendekatan, teknik, dan metode yang tepat untuk mengembangkan model prediktif yang akurat dan efisien.

- Menentukan tujuan yang jelas: Pernyataan masalah membantu menetapkan tujuan yang jelas dalam pengembangan model prediktif. Tujuan ini dapat mencakup meningkatkan akurasi prediksi, mengurangi risiko kredit, mempercepat proses pengambilan keputusan, atau meningkatkan efisiensi operasional. Dengan menetapkan tujuan yang jelas, kita dapat mengukur keberhasilan solusi yang diusulkan.

- Memotivasi penelitian dan pengembangan: Dengan merumuskan masalah dengan baik, kita dapat menghasilkan pemahaman yang lebih baik tentang urgensi dan pentingnya penelitian dan pengembangan solusi. Pernyataan masalah dapat menjadi landasan yang kuat untuk memotivasi upaya dalam mengembangkan model prediktif yang lebih baik dan lebih efisien.

- Untuk mencapai tujuan dalam prediksi status pinjaman dengan akurat dan efisien, kami mengusulkan solusi berikut:

  ### Solution statements

  - Penggunaan Teknik Machine Learning: Kami akan menerapkan teknik machine learning yang canggih, seperti regresi logistik, pohon keputusan, atau algoritma klasifikasi lainnya, untuk membangun model prediktif. Dengan memanfaatkan kekuatan machine learning, model kami akan dapat mempelajari pola-pola kompleks dari data historis pinjaman dan mengidentifikasi faktor-faktor yang paling berpengaruh dalam menentukan keberhasilan pinjaman.

  - Pengumpulan dan Analisis Data yang Komprehensif: Kami akan mengumpulkan data yang komprehensif tentang aplikasi pinjaman yang terverifikasi dan hasil status pinjaman dari peminjam sebelumnya. Data ini akan mencakup informasi seperti riwayat kredit, pendapatan, riwayat pekerjaan, aset, dan variabel lainnya yang relevan. Kami akan melakukan analisis mendalam terhadap data ini untuk mengidentifikasi pola dan tren yang berkaitan dengan status pinjaman yang sukses atau gagal.

  - Pemrosesan dan Pembersihan Data yang Tepat: Sebelum melatih model, kami akan melakukan pemrosesan dan pembersihan data yang tepat. Hal ini mencakup penanganan nilai yang hilang atau tidak valid, penghapusan outlier yang signifikan, dan normalisasi atau standarisasi data untuk mengoptimalkan kinerja model.

  - Validasi dan Evaluasi Model yang Teliti: Setelah melatih model, kami akan melakukan validasi dan evaluasi yang teliti terhadap kinerjanya. Kami akan membagi data menjadi subset pelatihan dan pengujian, dan menggunakan metrik evaluasi yang relevan seperti akurasi, presisi, recall, dan area di bawah kurva ROC untuk mengevaluasi kinerja model. Kami juga akan melakukan kros-validasi untuk mengukur robustness model terhadap data yang tidak terlihat sebelumnya.

  - Integrasi dengan Sistem Perbankan: Solusi kami akan diintegrasikan dengan sistem perbankan yang ada untuk mendukung proses pengambilan keputusan pinjaman. Model prediktif akan digunakan secara otomatis untuk mengevaluasi dan memberikan rekomendasi persetujuan pinjaman yang aman. Hal ini akan meningkatkan efisiensi operasional dan mengurangi keterlibatan manusia dalam proses evaluasi.

## Data Understanding

Dataset yang digunakan merupakan dataset Bank Loan Status yang diperoleh dari situs kaggle. Berikut merupakan link untuk mendownload dataset [Bank Loan Status Dataset](https://www.kaggle.com/datasets/zaurbegiev/my-dataset?select=credit_train.csv).

Berikut informasi pada dataset:

1. Dataset memiliki format csv(Comma Separated Value).
2. Dataset memiliki 100514 sampel dengan 19 fitur.
3. Dataset memiliki 6 fitur bertipe objek dan 13 fitur bertipe float64.
4. Terdapat missing value pada semua fitur.

### Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:

- Loan ID : merupakan id pinjaman,
- Customer ID : merupakan id pelanggan.
- Loan Status : merupakan status pinjaman.
- Current Loan Amount : jumlah pinjaman saat ini.
- Term : jangka waktu pembayaran pinjaman.
- Credit Score : merupakan kredit score dari peminjam.
- Annual Income : pendapatan tahunan peminjam.
- Years in current job : lama peminjam bekerja pada pekerjaan saat ini.
- Home Ownership : Status kepemilikan rumah peminjam.
- Purpose : tujuan pengajuan pinjaman.
- Monthly Debt : jumlah hutang bulanan peminjam.
- Years of Credit History : lamanya seorang peminjam memiliki riwayat kredit yang tercatat dalam catatan kredit.
- Months since last delinquent : jumlah bulan sejak terakhir kali seorang peminjam mengalami keterlambatan pembayaran (delinquent) dalam kewajiban keuangannya.
- Number of Open Accounts : jumlah total akun atau rekening keuangan yang aktif yang dimiliki oleh seorang peminjam pada saat tertentu.
- Number of Credit Problems : jumlah masalah kredit atau catatan negatif yang terkait dengan seorang peminjam dalam riwayat kredit mereka.
- Current Credit Balance : saldo total yang harus dibayar oleh seorang peminjam pada saat tertentu dalam hubungannya dengan rekening kredit mereka. Ini mencakup jumlah utang yang masih harus dilunasi pada kartu kredit, pinjaman, atau jenis rekening kredit lainnya.
- Maximum Open Credit : jumlah maksimum kredit yang disetujui atau tersedia untuk seorang peminjam pada saat tertentu. Ini mencerminkan batas maksimum yang diberikan oleh lembaga keuangan kepada peminjam untuk digunakan dalam bentuk pinjaman, kartu kredit, atau jenis rekening kredit lainnya.
- Bankruptcies : jumlah kebangkrutan yang dilaporkan oleh seorang peminjam dalam riwayat kredit mereka. Kebangkrutan mengacu pada situasi di mana individu atau perusahaan tidak mampu membayar utang mereka dan secara resmi dinyatakan pailit oleh pengadilan.
- Tax Liens : jumlah liabilitas pajak yang belum dibayar yang dimiliki oleh seorang peminjam. Liabilitas pajak dapat timbul ketika individu atau perusahaan gagal membayar pajak yang terutang kepada pihak berwenang, seperti pemerintah lokal atau badan pajak.

## Data Preparation

- One Hot Encoding

  One hot encoding adalah teknik mengubah data kategorik menjadi data numerik dimana setiap kategori menjadi kolom baru dengan nilai 0 atau 1. Fitur yang akan diubah menjadi numerik pada proyek ini adalah Loan Status, Term, dan Home Ownweship.

- Train Test Split

  Train test split aja proses membagi data menjadi data latih dan data uji. Data latih akan digunakan untuk membangun model, sedangkan data uji akan digunakan untuk menguji performa model. Pada proyek ini dataset sebesar 57142 dibagi menjadi 45713 untuk data latih dan 11429 untuk data uji.

- Normalization

  Algoritma machine learning akan memiliki performa lebih baik dan bekerja lebih cepat jika dimodelkan dengan data seragam yang memiliki skala relatif sama. Salah satu teknik normalisasi yang digunakan pada proyek ini adalah Standarisasi dengan sklearn.preprocessing.StandardScaler.

## Modeling

Pada penelitian ini, kami menggunakan tiga algoritma pemodelan, yaitu K-Nearest Neighbour (K-NN), Random Forest, dan AdaBoost. Berikut ini adalah penjelasan tentang setiap algoritma dan parameter yang digunakan dalam proyek ini:

- K-Nearest Neighbour (K-NN):

  Algoritma K-Nearest Neighbour bekerja dengan membandingkan jarak antara sampel yang akan diprediksi dengan sampel pelatihan yang ada. Jumlah tetangga terdekat (k) yang dipilih akan mempengaruhi prediksi.
  Pada proyek ini, kami menggunakan sklearn.neighbors.KNeighborsRegressor untuk membangun model K-NN. Kami menggunakan X_train dan y_train sebagai input untuk membangun model.
  Parameter yang digunakan dalam proyek ini adalah n_neighbors, yang merupakan jumlah tetangga terdekat yang akan dipertimbangkan.

- Random Forest:

  Algoritma Random Forest adalah teknik ensemble learning yang membangun banyak decision tree secara paralel pada waktu pelatihan.
  Pada proyek ini, kami menggunakan sklearn.ensemble.RandomForestRegressor untuk membangun model Random Forest. Kami menggunakan X_train dan y_train sebagai input untuk membangun model.
  Beberapa parameter yang digunakan dalam proyek ini adalah n_estimators, yang merupakan jumlah maksimum estimator atau decision tree dalam ensemble, max_depth, yang menentukan kedalaman maksimum setiap tree, dan random_state, yang mengontrol seed acak yang diberikan pada setiap base_estimator pada setiap iterasi boosting.

- AdaBoost:

  Algoritma AdaBoost (Adaptive Boosting) adalah teknik ensemble learning yang secara adaptif meningkatkan performa prediksi dengan menggabungkan beberapa model sederhana secara berurutan.
  Pada proyek ini, kami menggunakan sklearn.ensemble.AdaBoostRegressor untuk membangun model AdaBoost. Kami menggunakan X_train dan y_train sebagai input untuk membangun model.
  Beberapa parameter yang digunakan dalam proyek ini adalah n_estimators, yang merupakan jumlah maksimum estimator atau weak learners yang akan digunakan dalam ensemble, learning_rate, yang memperkuat kontribusi setiap regressor, dan random_state, yang mengontrol seed acak yang diberikan pada setiap base_estimator pada setiap iterasi boosting.
  Dengan menggunakan tiga algoritma tersebut dan parameter yang sesuai, penelitian ini bertujuan untuk membangun model prediktif yang akurat untuk memprediksi status pinjaman dengan menggunakan metode machine learning.

## Evaluation

Metrik yang digunakan dalam proyek ini adalah Mean Squared Error (MSE). MSE adalah metrik evaluasi yang umum digunakan dalam masalah regresi untuk mengukur sejauh mana perbedaan antara nilai prediksi dan nilai sebenarnya. Metrik MSE dihitung dengan membandingkan nilai prediksi yang dihasilkan oleh model dengan nilai sebenarnya dari target variabel. Perhitungan MSE melibatkan mengkuadratkan selisih antara nilai prediksi dan nilai sebenarnya, kemudian mengambil rata-rata dari seluruh perbedaan kuadrat tersebut.
Berikut formulan MSE :

<div><img src="https://user-images.githubusercontent.com/107544829/188412654-f5dc0ae1-901b-470e-aae5-1f6b5fb68b4d.png" width="300"/></div>

Berikut hasil evaluasi pada proyek ini :

- Akurasi
  | model | accuracy |
  |----------|----------|
  | knn | 148405.2 |
  | boosting | 118354.3 |
  | rf | 128170.4 |

<div><img src="https://github.com/aliftech/predictive-analisys/blob/master/image/evaluation.png"/></div>
