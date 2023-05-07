# Laporan Proyek Machine Learning Predictive Analisys - Wahyu Krisna Aji

## Domain Proyek

Pinjaman bank adalah bagian integral dari kegiatan perbankan dan memiliki implikasi besar baik bagi peminjam maupun institusi keuangan. Status pinjaman yang tidak tepat dapat mengakibatkan risiko kredit yang tinggi, kerugian finansial, dan ketidakpuasan pelanggan. Oleh karena itu, penting untuk mengembangkan metode yang akurat dan efisien untuk memprediksi status pinjaman guna membantu pengambilan keputusan yang lebih baik di industri perbankan.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Dengan kemajuan teknologi, terjadi banyak peningkatan juga di sektor perbankan. Jumlah aplikasi pinjaman yang diajukan setiap hari semakin meningkat. Namun, bank harus mempertimbangkan kebijakan-kebijakan tertentu saat memilih pemohon untuk persetujuan pinjaman. Memeriksa setiap individu secara manual dan kemudian merekomendasikan untuk persetujuan pinjaman merupakan tugas yang sulit dan berisiko. Oleh karena itu, dalam penelitian ini, kami menggunakan teknik machine learning yang akan memprediksi individu yang dapat dipercaya untuk pinjaman berdasarkan catatan sebelumnya dari orang-orang yang telah disetujui untuk pinjaman sebelumnya.
  Tujuan utama dari penelitian ini adalah untuk memprediksi apakah persetujuan pinjaman kepada individu tertentu aman atau tidak. Dalam hal ini, kami akan menggunakan data historis pinjaman yang mencakup informasi seperti riwayat kredit, pendapatan, riwayat pekerjaan, dan aset untuk melatih model machine learning. Model ini akan mempelajari pola dari data tersebut dan membuat prediksi berdasarkan faktor-faktor tersebut.
  Penggunaan teknik machine learning dalam analisis status pinjaman bank memiliki beberapa keuntungan. Pertama, memungkinkan proses pengambilan keputusan yang lebih cepat dan efisien. Dengan menggunakan model prediktif, bank dapat mengotomatisasi proses evaluasi pinjaman dan mengurangi keterlibatan manusia. Hal ini akan menghemat waktu dan biaya operasional bagi bank.
  Kedua, penggunaan machine learning dapat meningkatkan akurasi prediksi status pinjaman. Dengan memanfaatkan algoritma machine learning yang canggih, model dapat mempelajari pola-pola yang kompleks dari data historis dan mengidentifikasi faktor-faktor yang paling berpengaruh dalam menentukan keberhasilan pinjaman. Ini akan membantu bank membuat keputusan yang lebih informasional dan mengurangi risiko kredit.
  Ketiga, pendekatan ini dapat membantu bank dalam meningkatkan layanan kepada pelanggan. Dengan memiliki model prediktif yang kuat, bank dapat memberikan keputusan pinjaman yang lebih cepat dan transparan kepada pelanggan. Hal ini akan meningkatkan kepuasan pelanggan dan memperkuat hubungan antara bank dan pelanggan.
  Namun, ada beberapa tantangan yang perlu diatasi dalam penggunaan machine learning untuk analisis status pinjaman bank. Salah satunya adalah keterbatasan data yang akurat dan lengkap. Dalam beberapa kasus, data historis yang tersedia mungkin tidak mencakup semua faktor yang relevan untuk prediksi status pinjaman. Selain itu, perlu diperhatikan juga masalah privasi dan keamanan data yang sensitif.
  Dalam proyek ini, kami akan menggunakan teknik machine learning seperti regresi logistik, pohon keputusan, atau algoritma klasifikasi lainnya untuk membangun model prediktif. Kami akan melatih model menggunakan dataset yang mencakup informasi pinjaman yang terverifikasi dan hasil status pinjaman dari peminjam sebelumnya. Setelah melatih model, kami akan menguji kinerjanya
- [Bank Loan Prediction System using Machine Learning](https://ieeexplore.ieee.org/abstract/document/9336801)

## Business Understanding

Pada bagian ini, kamu perlu menjelaskan proses klarifikasi masalah.

Bagian laporan ini mencakup:

### Problem Statements

Menjelaskan pernyataan masalah latar belakang:

- Pernyataan Masalah 1
- Pernyataan Masalah 2
- Pernyataan Masalah n

### Goals

Menjelaskan tujuan dari pernyataan masalah:

- Jawaban pernyataan masalah 1
- Jawaban pernyataan masalah 2
- Jawaban pernyataan masalah n

Semua poin di atas harus diuraikan dengan jelas. Anda bebas menuliskan berapa pernyataan masalah dan juga goals yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Menambahkan bagian “Solution Statement” yang menguraikan cara untuk meraih goals. Bagian ini dibuat dengan ketentuan sebagai berikut:

  ### Solution statements

  - Mengajukan 2 atau lebih solution statement. Misalnya, menggunakan dua atau lebih algoritma untuk mencapai solusi yang diinginkan atau melakukan improvement pada baseline model dengan hyperparameter tuning.
  - Solusi yang diberikan harus dapat terukur dengan metrik evaluasi.

## Data Understanding

Paragraf awal bagian ini menjelaskan informasi mengenai data yang Anda gunakan dalam proyek. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data).

Selanjutnya uraikanlah seluruh variabel atau fitur pada data. Sebagai contoh:

### Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:

- accepts : merupakan jenis pembayaran yang diterima pada restoran tertentu.
- cuisine : merupakan jenis masakan yang disajikan pada restoran.
- dst

**Rubrik/Kriteria Tambahan (Opsional)**:

- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data atau exploratory data analysis.

## Data Preparation

Pada bagian ini Anda menerapkan dan menyebutkan teknik data preparation yang dilakukan. Teknik yang digunakan pada notebook dan laporan harus berurutan.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Menjelaskan proses data preparation yang dilakukan
- Menjelaskan alasan mengapa diperlukan tahapan data preparation tersebut.

## Modeling

Tahapan ini membahas mengenai model machine learning yang digunakan untuk menyelesaikan permasalahan. Anda perlu menjelaskan tahapan dan parameter yang digunakan pada proses pemodelan.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Menjelaskan kelebihan dan kekurangan dari setiap algoritma yang digunakan.
- Jika menggunakan satu algoritma pada solution statement, lakukan proses improvement terhadap model dengan hyperparameter tuning. **Jelaskan proses improvement yang dilakukan**.
- Jika menggunakan dua atau lebih algoritma pada solution statement, maka pilih model terbaik sebagai solusi. **Jelaskan mengapa memilih model tersebut sebagai model terbaik**.

## Evaluation

Pada bagian ini anda perlu menyebutkan metrik evaluasi yang digunakan. Lalu anda perlu menjelaskan hasil proyek berdasarkan metrik evaluasi yang digunakan.

Sebagai contoh, Anda memiih kasus klasifikasi dan menggunakan metrik **akurasi, precision, recall, dan F1 score**. Jelaskan mengenai beberapa hal berikut:

- Penjelasan mengenai metrik yang digunakan
- Menjelaskan hasil proyek berdasarkan metrik evaluasi

Ingatlah, metrik evaluasi yang digunakan harus sesuai dengan konteks data, problem statement, dan solusi yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**:

- Menjelaskan formula metrik dan bagaimana metrik tersebut bekerja.

**---Ini adalah bagian akhir laporan---**

_Catatan:_

- _Anda dapat menambahkan gambar, kode, atau tabel ke dalam laporan jika diperlukan. Temukan caranya pada contoh dokumen markdown di situs editor [Dillinger](https://dillinger.io/), [Github Guides: Mastering markdown](https://guides.github.com/features/mastering-markdown/), atau sumber lain di internet. Semangat!_
- Jika terdapat penjelasan yang harus menyertakan code snippet, tuliskan dengan sewajarnya. Tidak perlu menuliskan keseluruhan kode project, cukup bagian yang ingin dijelaskan saja.
