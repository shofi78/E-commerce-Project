# BI Model for E-Commerce - Dashboard

## Latar Belakang
Sebagai early stage startup yang bergerak di bidang retail, Pacmano d’e-comercio memiliki visi menjadi one-stop shopping marketplace terbesar di Amerika Selatan, dan untuk mewujudkan visi tersebut, perusahaan memiliki misi tumbuh bersama dengan mitra, mengedepankan tingkat pelayanan yang konsisten dan terpercaya bagi semua pelanggan, dan menjual semua barang kebutuhan sehari-hari dengan harga yang paling terjangkau dan kualitas nomor satu. 

Namun, sejak awal berdirinya Pacmano di 2015, perusahaan baru memiliki sistem ERP di tahun 2016, sehingga semua data terkait penjualan, pelanggan dan mitra baru terekam di pertengahan tahun 2016. Saat ini, tim management perlu mempersiapkan langkah apa saja yang harus dilakukan untuk meningkatkan akuisisi mitra & pelanggan, dan juga memaksimalkan penjualan. Untuk itu, tim management dan semua departemen terkait membutuhkan suatu metrik yang dapat memberikan insight dan penggambaran terkait kondisi dan perkembangan di tiap departemen dalam kaitannya dengan performance/ key result perusahaan Pacmano d’e-comercio. 

Perkembangan pesat yang terjadi pada perusahaan Pacmano d’e-comercio menyebabkan aliran informasi berupa data-data krusial menjadi sulit diinterpretasikan oleh tim manajemen dan lintas departemen secara cepat dan mudah. Untuk itu, diperlukan suatu dashboard untuk dijadikan sebagai SSOT yang akan membantu tim manajemen dan departemen terkait untuk mendapatkan insight dari metrik-metrik bisnis, yang berguna untuk menentukan kebijakan dan arah perusahaan.

## Objectives
Project ini ditujukan untuk menentukan metrik-metrik bisnis yang dibutuhkan oleh C-Level, Departemen Sales & Operations, Departemen Pemasaran dan Departemen Business Development, dan menampilkan metrik-metrik tersebut ke dalam sebuah dashboard SSOT. 

Pada Dashboard Executive Summary, project ini bertujuan untuk menampilkan informasi berupa overview aspek bisnis perusahaan, yang ditujukan khususnya untuk C-Level Management.

Pada Dashboard Sales & Operations, project ini bertujuan untuk menampilkan informasi terkait performa penjualan terhadap target, dan tingkat pelayanan perusahaan.

Pada Dashboard Marketing, project ini bertujuan untuk menampilkan data harian pemasaran berupa informasi yang berguna untuk melihat efektivitas promosi, segmentasi pelanggan dan retensi/ loyalitas pelanggan.

Pada Dashboard Business Development, project ini bertujuan untuk menampilkan data pengembangan bisnis berupa fitur yang mendukung keberlangsungan bisnis, seperti conversion rate berdasarkan A/B Testing.

## Process Overview
a. Penyusunan PRD
Pada awal project, dilakukan penyusunan PRD untuk menentukan tujuan, scope, fitur, timeline, perkiraan user flow dan HiFi Dashboard Mockup. Dokumen lengkap PRD dapat diakses di [**link**](https://docs.google.com/document/d/10blzS2O8wq901DAAHNKbEMb3MM3TlxmRgJRpjE0wuPc/edit?usp=sharing) tersebut. Pada PRD, dirancang perkiraan user flow pada produk yang akan dibuat

<img width="5776" alt="User Flow PLBI 2 - Ecomercio - Grup N" src="https://user-images.githubusercontent.com/102605912/193493518-69dd2b9e-1b56-42c1-bb63-c7af78d10d31.png">

Dan juga dibuat Hi Fi Dashboard Mockup sebagai acuan dan gambaran umum tampilan dashboard yang akan di launch
HiFi Dashboard dapat dilihat pada [**link**](https://www.figma.com/file/rbwWu1Go9EJdB63WL2Emwm/Pacmano-d'Ecomercio-Hi-Fi-Prototype---PLBI-2---Group-N?node-id=0%3A1) ini.

b. Penentuan Business Metrics
Project ini diawali dengan menentukan Business Metrics yang dapat memberikan gambaran terkait kondisi perusahaan secara keseluruhan, dan kondisi pada tiap departemen, yaitu departemen Sales & Operations, departemen Marketing dan departemen Business Development.
Untuk dapat menentukan Business Metrics yang tepat sasaran, perlu dilakukan analisis terlebih dahulu terkait ketersediaan data pada sistem enterprise perusahaan. Dari proses ini diketahui bahwa data yang tersedia dari sistem ERP dan Web Service Analytics adalah sebagai berikut;
  - Data Sales Performance
    
    Pada data ini terdapat data krusial seperti order id, lead id, seller id, purchase time, seller & customer locations, dengan hubungan data seperti yang ditampilkan     pada gambar berikut.
    ![Dasa set sales](https://user-images.githubusercontent.com/102605912/193494102-b68a5dda-fd10-4282-9655-fa3a31966719.PNG)
  - Data Marketing Performance 
  
    Pada data ini terdapat informasi terkait pelanggan, yang dapat digunakan untuk melakukan analisis segmentasi pelanggan, seperti usia, status, penghasilan, jumlah       pengeluaran pada kategori produk, dll.
  - Data A/B Testing
  
    Pada dataset ini terdapat informasi yang penting untuk departemen business development dalam pengambilan keputusan terkait landing page yang akan digunakan.
    
Dari ketiga dataset tersebut, maka diputuskan akan dibuat sebuah Dashboard SSOT, dimana di dalamnya terdapat beberapa dashboard dengan metrik sebagai berikut;
  - Executive Summary Dashboard
  
    Menampilkan Business Metrics Berupa Total Revenue, Total Customer, Total Seller, Total Order, Total Product yang dijual, Campaign Rate, dan pertumbuhan Revenue         tiap kuarter. Metrik-metrik tersebut dipilih karena merupakan penggambaran umum dari kondisi bisnis terkini.
  - Sales & Operations Dashboard
  
    Menampilkan Business Metrics sebagai berikut
    - Sales Performance
    
      Menampilkan total sales per bulan, persentase pertumbuhan sales per bulan & target per bulan, sebesar 1.5% pertumbuhan terhadap aktual sales di bulan sebelumnya.       Metrik ini bertujuan untuk analisis dalam merencanakan target, dan melakukan evaluasi atas histori penjualan
    - Customer Review
    
      Menampilkan jumlah rata-rata skor review dari pelanggan berdasarkan waktu, dan persentase tiap skor (skala 1-5)  yang diberikan terhadap jumlah total review.
      Metrik ini diharap dapat memberi informasi terkait review pelanggan tiap bulan dan dapat dilakukan analisis dengan korelasinya terhadap jumlah sales, dan tingkat       pelayanan/SLA
    - Top Product
    
    Menampilkan produk yang paling banyak menyumbang pendapatan dari sales, diurutkan dari yang terbesar hingga terkecil. 
    Metrik ini diharapkan dapat memberikan insight terkait produk kategori apa saja yang banyak digemari dan dibeli pelanggan, dan produk mana yang tidak, sehingga   dapat dilakukan penjualan di produk-produk yang paling laku, dan menjadi peluang untuk mengakuisisi produk-produk yang masih kurang populer
    - Customer, Sellers & Sales Distribution
    
      Metrik ini menampilkan total sales berdasarkan wilayah, dan menampilkan perbandingan jumlah customer dan seller di tiap wilayah tersebut
      Metrik ini dapat memberikan insight terkait wilayah mana yang paling banyak terdapat customer dan paling menyumbang besar terhadap revenue, dan dengan  perbandingan jumlah customer dengan seller, dapat membantu untuk menentukan arah & strategi akuisisi & penjualan

    - Lead Time/ Cycle
    
    Metrik ini menampilkan lead time dari setiap stage/ tahap flow operasional, tujuannya untuk mempertahankan tingkat pelayanan yang konsisten terhadap pelanggan.
    
  - Marketing Dashboard
  
    Menampilkan Business Metrics sebagai berikut
    - Monthly Active User
    
      Metrik ini menunjukan jumlah customer yang aktif rata-rata setiap bulan berdasarkan customer yang melakukan visit website.
    - Recommendation product by segmentation
Menampilkan produk yang menjadi rekomendasi produk berdasarkan segmentasi customer.
Most ordered product by quarterly/seasonal
Menampilkan jumlah produk yang paling banyak dibeli dalam waktu setiap kuartal.
Average conversion rate per campaign
Metrik ini menunjukan rata-rata konversi setiap campaign yang dijalankan secara terpisah.
Most purchased product by segmentation
Menampilkan produk yang paling banyak dibeli berdasarkan segmentasi customer.
RFM Indicator
Metrik untuk mengetahui rata-rata RFM score berdasarkan segmentasi customer.
RFM Segmentation
Metrik untuk mengetahui segmentasi dari masing-masing customer menggunakan RFM Segmentation.
A/B Testing Dashboard
Menampilkan Business Metrics sebagai berikut:
Ringkasan Hasil Uji
Ditampilkan ringkasan apakah uji hipotesis ini gagal tolak atau ditolak. Diberikan juga alasan dari hasil uji tersebut dengan data p-value dan power. Tidak lupa memberikan rekomendasi bisnis untuk AB Testing team.
Total Converted, Conversion Rate dan Visit
Metrics ini digunakan untuk mengetahui jumlah conversi, conversion rate dan jumlah visit pada masing - masing landing page
Daily p-value dan power
Menampilkan insight dari nila p-value dan power yang diperoleh per hari untuk dijadikan pedoman akan keberlangsungan dari eksperimen. Selain itu ditampilkan pada MDE berapa power minimal dapat dicapai pada eksperimen.







