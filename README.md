# Analisis-Kepribadian-Pelanggan-dan-Pemasaran-Segmentasi-Pasar-Menggunakan-K-Means-Clustering

**Analisis Kepribadian Pelanggan dan Kampanye Pemasaran: Segmentasi Pasar Menggunakan K-Means Clustering**

Memahami perilaku dan kebiasaan belanja pelanggan adalah kunci utama bagi perusahaan untuk merancang kampanye pemasaran yang efisien dan tepat sasaran. Namun, data pelanggan riil seringkali masih mentah, memiliki nilai yang kosong (*missing values*), dan variabel yang terlalu kompleks untuk langsung dianalisis. Oleh karena itu, diperlukan prapemrosesan data dan *feature engineering* yang komprehensif untuk mengubah 2.240 baris data operasional perusahaan grosir menjadi basis segmentasi pasar yang *actionable*.

Sebagai Data Analyst, saya melakukan ekstraksi, pembersihan, eksplorasi data, hingga persiapan pemodelan *clustering* untuk mengelompokkan pelanggan berdasarkan daya beli, loyalitas, dan profil demografis. Proses ini bertujuan untuk memberikan wawasan berbasis data (*data-driven insight*) kepada tim *Marketing* dalam menyusun strategi promosi yang lebih personal dan meningkatkan ROI perusahaan.

# **Tech Stack Analitik**
Pembersihan, transformasi, dan pemodelan pada proyek ini dibangun menggunakan *environment* analitik berikut:

* **Python (Pandas, NumPy):** Digunakan untuk manipulasi *dataframe*, konversi tipe data (seperti *datetime*), serta *feature engineering* tingkat lanjut.
* **Scikit-Learn (K-Means, PCA):** Digunakan untuk prapemrosesan data numerik (*StandardScaler*) dan penerapan algoritma *machine learning* untuk *clustering* pelanggan.
* **Matplotlib & Seaborn:** Digunakan untuk Visualisasi Data Eksploratif (EDA) guna mendeteksi pola hubungan antar fitur dan memetakan distribusi data pelanggan.

# **Pengumpulan Data**
Dataset sekunder bersumber dari Kaggle (*Customer Personality Analysis*), memuat catatan historis perilaku belanja dari sebuah perusahaan grosir. Data ini mencakup 29 dimensi informasi mulai dari tingkat pendapatan, pendidikan, durasi langganan, umur, hingga pola pembelian berbagai kategori produk pemasaran (daging, ikan, anggur, dll).

# **Preprocessing & Feature Engineering**
Pendekatan transformasi data dilakukan secara terstruktur agar algoritma *machine learning* dapat membaca informasi secara optimal:

* **Data Translation & Formatting:** Menerjemahkan dan menyeragamkan 29 nama kolom ke dalam bahasa Indonesia agar lebih deskriptif dan mempercepat pemahaman konteks bisnis. Konversi tipe data *datetime* juga diterapkan pada tanggal pendaftaran pelanggan.
* **Data Cleansing:** Melakukan pembersihan data yang memiliki *missing values* secara sistematis (menggunakan `dropna`) untuk mencegah bias informasi, sehingga menghasilkan 2.216 baris data bersih dan valid.
* **Feature Engineering:** Menciptakan metrik analitik baru untuk menangkap profil pelanggan dengan lebih akurat. Ini termasuk perhitungan 'Umur' aktual, agregasi metrik 'Pengeluaran' total dari seluruh produk, perhitungan metrik loyalitas 'Lama Terdaftar' (dalam hitungan hari), serta pembuatan *flagging* kepemilikan 'Jumlah Anak'.
* **Data Standardization & Reduction:** Menyederhanakan kategori status pernikahan (Sendiri, Menikah, Cerai, dll) dan tingkat pendidikan (Undergraduate, Graduate, Postgraduate). Kolom redundan dan data privat (ID Pelanggan) dieksklusi untuk meningkatkan performa model *clustering*.

# **Visualisasi Data Eksploratif (EDA)**
Tahap ini mencakup peringkasan statistik deskriptif dari seluruh variabel pembentuk daya beli pelanggan. Visualisasi hubungan korelasi (*pairplot*) digunakan untuk mengamati perbedaan signifikan pola belanja dan kunjungan web berdasarkan variabel demografis utama, seperti status kepemilikan anak.

Tertarik dengan proses ekstraksi fitur tingkat lanjut dan kode pemodelan *clustering* di balik layar?
Silakan telusuri tahapan lengkapnya melalui Jupyter Notebook di repositori GitHub ini. Jika Anda memiliki *feedback*, masukan, atau ingin berdiskusi mengenai peluang kolaborasi dan karir di bidang data, mari terhubung melalui LinkedIn saya atau jangkau saya melalui email di deswitanaf.work@gmail.com.
