# Capstone-3-Travel-Insurance-Machine-Learning-Classification

Capstone Module 3 (Machine Learning)

Membuat Machine Learning untuk mengelola dan membuat pemodelan dari data yang telah diberikan.
Data yang akan digunakan adalah data Travel Insurance

sumber data : [Data Travel Insurance](https://drive.google.com/file/d/1emDTGFvku7UuuVT3W-EmEvg3i61QrIU-/view)


### **Contents**

1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

### **Business Problem Understanding**

**Context**

Asuransi perjalanan adalah asuransi yang memberikan perlindungan terhadap segala risiko yang mungkin terjadi ketika seseorang melakukan perjalanan, baik di dalam negeri maupun di luar negeri. Asuransi ini diutamakan bagi orang-orang yang kerap memiliki mobilitas tinggi, seperti bepergian ke luar kota hingga ke luar negeri. Kepemilikan perlindungan ini berfungsi untuk menekan dampak finansial dari risiko kerugian yang mungkin terjadi saat perjalanan tersebut. source: https://www.qoala.app/id/blog/asuransi/umum/apa-itu-asuransi-perjalanan/

Bebebrapa manfaat yang didapatkan dari asuransi perjalanan atau Travel Insurance adalah Ganti Rugi Atas Kerusakan atau Kehilangan Bagasi, Ganti Rugi Keterlambatan atau Pembatalan Perjalanan, Biaya Pengobatan yang Ditanggung, Santunan Kecelakaan dan Kematian, Menanggung Kerugian Finansial Akibat Faktor Lain (Segala bentuk kerugian baik fisik, mental, serta finansial akan ditanggung oleh pihak asuransi).


**Problem Statement**

Salah satu tantangan terbesar bagi pihak jasa Travel Insurance adalah pemecahan masalah untuk dapat memiliki model bisnis yang menguntungkan secara finansial bagi pemilik jasa, serta dapat memberikan pengalaman positif terhadap pengguna jasa.

Mengingat bahwa harga penawaran harus ideal, untuk menentukan harga jasa mereka, dengan hanya memberikan petunjuk minimal dengan tujuan memungkinkan Jasa Travel Insurance dapat menawarkan benefit yang diberikan dengan membandingkan kelebihan dengan jasa serupa di beberapa penyedia jasa Travel Insurance lainnya. Dari alasan tersebut digunakan untuk mendapatkan harga yang kompetitif. Penyedia Jasa Travel Insurance dapat memasukkan harga yang lebih tinggi untuk fasilitas tambahan apa pun yang mereka anggap perlu. Dengan bertambahnya penyedia jasa Travel Insurance, untuk menentukan harga yang tepat dan dapat tetap kompetitif yang akan ditawarkan sangatlah penting. Setelah pengguna jasa menggunakan jasa travel insurance maka langkah selanjutnya adalah mereka akan menentukan apakah mereka akan melakukan claim terhadap jasa tersebut ataupun tidak. 


**Goals**

Berdasarkan permasalahan tersebut, Penyedia jasa Travel Insurance harus atau sudah memiliki 'tool' yang dapat memprediksi serta membantu mereka mereka (dalam hal ini Travel Insurance) untuk dapat **Mengetahui Klasiifikasi Bagi Pengguna yang Claim Asuransi Pada Penyedia Jasa Travel Insurance**. Adanya perbedaan pada klasifikasi tersebut dapat menentukan profit bagi penyedia jasa Travel Insurance.


**Analytic Approach**

Dari pembahasan diatas maka yang saya akan lakukan  adalah menganalisis data untuk dapat menemukan pola dari fitur-fitur yang ada, yang membedakan Travel Insurance satu dengan yang lainnya. 

Selanjutnya, saya akan membangun suatu model Klasifikasi yang akan membantu Penyedia jasa Travel Insurance untuk dapat menyediakan 'tool' prediksi yang mana dapat menentukan klasifikasi mana yang akan dikelompokan bagi pengguna jasa.


**Metric Evaluation**

Metrik Evaluasi yang akan digunakan adalah Precision, Recall, F1 Score. Dan difokuskan kepada Recall

Claim Yes = Positif
Kesalahan Tipe I (False Positif) - Menerima hipotesis nol palsu (Penumpang Aktual Tidak Claim tetapi diprediksi Claim)

Kesalahan Tipe II (False Negatif) - Menolak hipotesis nol yang benar (Penumpang Aktual Claim Diprediksi Tidak Claim)

Fokusnya adalah untuk mengetahui kesalahan Tipe I dan II karena akan menyebabkan lebih banyak kerugian.
Oleh karena itu nilai Recall yang tinggi, tanpa mengorbankan nilai presisi yang rendah akan menjadi tujuannya. Menyeimbangkan recall dan precssion 


# QUICK EDA FOR FEATURE SELECTION

### Hipotesa Awal :

- Agency Type Berpengaruh terhadap Claim
- Duration Berpengaruh terhadap Claim
- Net Sales berpengaruh terhadap Claim
- Commision (In Value) Berpengaruh terhadap Claim

