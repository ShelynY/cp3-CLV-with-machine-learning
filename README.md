CUSTOMER LIFETIME VALUE

Contents

1. Business Problem Understanding
2. Data Understanding
3. Data Preprocessing
4. Modeling
5. Conclusion
6. Recommendation

1. Business Problem Understanding
1.1. Background

Customer lifetime value atau CLV adalah suatu ukuran seberapa berharga suatu customer terhadap perusahaan. Dari nilai tersebut, perusahhan dapat menentukan berapa keuntungan yang didapatkan dari satu penumpang dan biaya yang dikeluarkan untuk memperoleh customer baru atau mempertahankan customer lama. Angka ini cukup penting diketahui oleh suatu perusahaan jika perusahaan ingin secara efektif menargetkan pemasaran kepada pelanggan yang berharga dan bagaimana pelanggan perusahaan tersebut berubah kedepannya.

Sebuah perusahaan yang bergerak di bidang asuransi mobil ingin meningkatkan pendapatan dan profitabilitasnya. Untuk mencapai tujuan ini, perusahaan melakukan evaluasi berdasarkan data pelanggan untuk menentukan aspek-aspek yang dapat berpengaruh pada peningkatan profit. Stakeholder utama dalam proyek ini adalah CEO perusahaan asuransi. CEO membutuhkan nilai CLV untuk merencanakan strategi marketing. Dengan mengetahui nilai CLV, perusahaan dapat mengidentifikasi pelanggan yang memberikan kontribusi profit tertinggi dan fokus pada retensi mereka. Strategi ini membantu mengurangi biaya akuisisi pelanggan baru dan meningkatkan efisiensi pemasaran. Dengan memahami nilai jangka panjang dari setiap pelanggan, perusahaan dapat menyusun strategi pemasaran yang lebih terarah, memaksimalkan pendapatan dari setiap pelanggan, dan akhirnya meningkatkan profitabilitas keseluruhan perusahaan.
1.2. Problem Statement

CEO dari perusahaan asuransi mobil ingin meningkatkan income dengan membuat strategi marketing yang lebih tepat sasaran dan efisien. Perusahaan asuransi tersebut membutuhkan tool untuk memprediksi nilai CLV yang akurat agar dapat menyingkat waktu dan biaya yang dibutuhkan untuk marketing lebih sedikit.
1.3. Goal

Berdasarkan permasalahan tersebut,perusahaan asuransi ini memerlukan model Machine Learning yang dapat memprediksi CLV, sehingga dapat membuat startegi pemasaran yang tepat. Tujuan dari proyek ini adalah untuk mengembangkan model ML prediksi CLV berdasarkan dataset yang tersedia. Model prediksi ini diharapkan dapat membantu perusahaan untuk membuat strategi pemasaran sehingga dapat meningkatkan income perusahaan.
1.4 Analytic Approach

Jadi, yang perlu dilakukan adalah menganalisis data untuk dapat menemukan pola dari fitur-fitur yang ada, yang dapat membedakan satu customer dengan yang lainnya.

Selanjutnya, kita akan membangun suatu model ML regresi yang akan membantu perusahaan untuk dapat memprediksi CLV dari setiap customer, sehingga akan berguna untuk menentukan aspek apa saja yang berpengaruh dalam memberikan profit kepada perusahaan dan perusahaan bisa mengambil keputusan bisnis yang tepat dari nilai CLV yang diprediksi model.
1.5 Metric Evaluation

Evaluasi metrik yang akan digunakan yaitu:

    RMSE adalah nilai rataan akar kuadrat dari error
    MAE adalah rataan nilai absolut dari error
    MAPE adalah rataan nilai persentase error yang dihasilkan oleh model regresi

Semakin kecil nilai RMSE, MAE, dan MAPE yang dihasilkan, berarti model semakin akurat dalam memprediksi sesuai dengan limitasi fitur yang digunakan.
2. Data Understanding

Attributes Information
Attribute 	Data Type 	Description
Vehicle Class 	Object 	Tipe kendaraan
Coverage 	Object 	Jenis pertanggungan polis asuransi customer
Renew Offer Type 	Object 	Penawaran untuk pembaruan polis
EmploymentStatus 	Object 	Status pekerjaan cutomer
Marital Status 	Object 	Status pernikahan cutomer
Education 	Object 	Tingkat pendidikan customer
Number of Policies 	Float 	Jumlah polis yang dimiliki customer
Monthly Premium Auto 	Float 	Premi customer perbulan (USD)
Total Claim Amount 	Float 	Jumlah claim customer (USD)
Income 	Float 	Pendapatan cutomer (USD)
Customer Lifetime Value 	Float 	Customer Lifetime Value (Target)
