# LAPORAN ANALISIS DATA LALU LINTAS NHTSA

## Masalah

  National Highway Traffic Safety Administration (NHTSA) merupakan sebuah lembaga pemerintah Amerika Serikat yang memiliki misi yang sangat penting, yaitu melindungi masyarakat dengan menyelamatkan nyawa, mencegah cedera, dan mengurangi dampak ekonomi yang dihasilkan oleh kecelakaan lalu lintas. Untuk mencapai tujuan ini, NHTSA menggabungkan berbagai pendekatan yang komprehensif.

  Salah satu peran utama NHTSA adalah mengumpulkan, menganalisis, dan mempublikasikan data tentang kecelakaan lalu lintas yang terjadi dalam satu tahun tertentu. Data ini mencakup berbagai informasi penting seperti jenis kecelakaan, lokasi, faktor penyebab, dan dampaknya terhadap korban. Melalui analisis data yang mendalam ini, NHTSA dapat mengidentifikasi tren dan pola kecelakaan yang ada, memahami penyebabnya, dan merumuskan solusi yang lebih baik untuk mencegah kecelakaan di masa mendatang.

## Tujuan

  Analisis data tahun 2021 dilakukan untuk mengidentifikasi masalah keselamatan lalu lintas. Tujuannya adalah mengembangkan rekomendasi peraturan untuk meningkatkan keselamatan dan mengurangi risiko kecelakaan. Analisis mengungkapkan tren jenis kecelakaan dan faktor penyebab seperti kondisi cuaca dan perilaku pengemudi. Ini memungkinkan pengembangan peraturan yang lebih spesifik dan strategi pencegahan yang lebih efektif. Indikator utama telah diidentifikasi sebagai dasar untuk rekomendasi peraturan:

1. Berdasarkan kategori kecelakaan (jenis jalan, jenis persimpangan, kondisi penerangan, dan cuaca)

2. Berdasarkan wilayah tempat terjadinya kecelakaan (top 10 negara bagian, top 10 kota negara bagian, dan daerah pedesaan vs. perkotaan)

3. Berdasarkan waktu terjadinya kecelakaan (menurut bulan, hari, dan jam)

4. Berdasarkan kondisi pengemudi ketika kecelakaan terjadi (dalam keadaan mabuk atau tidak beserta waktu insiden)

  Namun, analisis ini tidak hanya terbatas pada data internal. Untuk memastikan bahwa rekomendasi peraturan yang dihasilkan memiliki dasar yang kuat, informasi eksternal yang relevan juga dipertimbangkan. Ini termasuk riset ilmiah terkini tentang keselamatan lalu lintas, praktik terbaik yang telah terbukti efektif di negara-negara lain, dan perkembangan teknologi terbaru yang dapat digunakan untuk meningkatkan keselamatan di jalan raya.

## Temuan

  Analisis data melibatkan proses terstruktur dengan penggunaan Google Spreadsheet, Microsoft Excel, dan SQL untuk membersihkan dan mengolah data. SQL digunakan untuk agregasi data, perhitungan persentase, dan query khusus. Selanjutnya, data diubah menjadi visualisasi yang informatif. Analisis data jenis kecelakaan adalah langkah awal penting untuk pemahaman keselamatan lalu lintas dan rekomendasi peraturan yang lebih efektif.

### 1. Berdasarkan kategori kecelakaan

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/crash%20type-all.jpg)

  Jenis kecelakaan paling umum adalah bukan tabrakan dengan kendaraan bermotor, sebanyak 21.768 kejadian. Selain itu, berbagai bentuk kecelakaan lainnya terjadi seperti angle (6.416), front-to-front (3.618), dan front-to-rear (2.424). Data ini mencerminkan keragaman situasi penyebab kecelakaan di jalan.
  Selanjutnya, analisis akan memeriksa beberapa faktor, yaitu jenis jalan, jenis persimpangan, kondisi penerangan, dan cuaca yang dapat memengaruhi kecelakaan. Korelasi antara jenis kecelakaan dengan faktor-faktor ini akan diidentifikasi. Selain itu, hasil temuan akan dipertimbangkan berdasarkan kondisi saat kecelakaan terjadi.


  - Jenis jalan dan jenis persimpangan

  ![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/not%20collision%20with%20motor%20vehicle/road%20type-not%20collision%20with%20motor%20vehicle.jpg)

  Kecelakaan tertinggi terjadi di jenis jalan *Principal Arterial - Other* (5.315 insiden) dalam kecelakaan tunggal. Ini juga berlaku untuk jenis kecelakaan *angle* (2.691), *front to front* (1.184), dan beberapa jenis lainnya. *Interstate* tertinggi pada jenis kecelakaan *front to rear* (853) dan *sideswipe: same direction* (208), sementara *Minor Arterial* tertinggi pada jenis *sideswipe: opposite direction* (131). Kecelakaan *rear to rear* yang lebih jarang terjadi (2 insiden) terdistribusi pada jenis jalan *Principal Arterial - Other* dan *Major Collector*. Ini menunjukkan bahwa kecelakaan sering terjadi di jalan panjang, dengan volume tinggi, dan kendaraan bermotor berkecepatan tinggi.

   ![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/not%20collision%20with%20motor%20vehicle/intersection%20type-not%20collision%20with%20motor%20vehicle.jpg)

  Kecelakaan tertinggi juga terjadi di jalan lurus (18.692 insiden) dalam kecelakaan tunggal. Ini adalah temuan penting dan jenis persimpangan ini juga sering menjadi lokasi insiden untuk jenis kecelakaan lain, kecuali angle (3.108) yang lebih sering terjadi di perempatan.
  
  - Kondisi penerangan dan cuaca

   ![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/not%20collision%20with%20motor%20vehicle/light%20condition-not%20collision%20with%20motor%20vehicle.jpg)

  Dalam analisis data ini, ditemukan bahwa kondisi penerangan yang memiliki jumlah kecelakaan tertinggi adalah kategori *daylight*, dengan total insiden mencapai 8.208 pada jenis kecelakaan tunggal. Temuan ini menunjukkan bahwa kecelakaan tunggal terjadi ketika kondisi penerangan cukup baik, yaitu saat siang hari. Namun, kategori ini juga menduduki peringkat teratas untuk jenis kecelakaan lainnya.

  ![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/not%20collision%20with%20motor%20vehicle/atmosphere%20condition-not%20collision%20with%20motor%20vehicle.jpg)

  Berkorelasi dengan hasil kondisi penerangan, cuaca yang paling banyak menyebabkan kecelakaan adalah yang disebut *clear*, dengan total insiden yang sangat tinggi, yaitu mencapai 15.203 pada jenis kecelakaan tunggal. Ini menunjukkan bahwa sebagian besar insiden tidak terjadi akibat perubahan cuaca seperti hujan, salju, kabut, atau sejenisnya. Temuan ini juga berlaku untuk jenis kecelakaan lainnya.

### 2. Berdasarkan wilayah tempat terjadinya kecelakaan

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/states-all.jpg)

  Analisis lanjutan dilakukan dengan mengamati di negara apa saja kecelakaan ini terjadi secara keseluruhan. Dari hasil tersebut, diambil sepuluh negara dengan angka kecelakaan paling tinggi. Kecelakaan paling banyak terjadi di Texas (3.513), California (3.484), dan Florida (3.091). Faktor-faktor demografis seperti populasi juga dipertimbangkan. California memiliki [populasi](https://datacommons.org/ranking/Count_Person/State/country/USA?h=geoId%2F48) tertinggi (sekitar 39 juta), diikuti oleh Texas (sekitar 29 juta), tetapi Texas memiliki angka kecelakaan lebih tinggi meskipun perbedaan populasi tidak terlalu besar. Analisis lebih mendalam kota-kota di setiap negara bisa memberikan wawasan lebih rinci tentang pola kecelakaan, meskipun ada beberapa anomali yang menarik.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/cities/texas.jpg)

  Saat kita melihat data kecelakaan di berbagai kota di masing-masing sepuluh negara, ditemukan bahwa ada kota-kota dengan jumlah kecelakaan yang tinggi, tetapi informasi khusus tentang lokasi kecelakaan ini tidak tersedia dalam data. Sebagai contoh, di negara bagian Texas, jumlah kecelakaan tertinggi tidak memiliki keterangan yang menyebutkan di kota mana kecelakaan tersebut terjadi. Selain itu, jumlah kecelakaan ini cukup besar jika dibandingkan dengan kecelakaan yang memiliki informasi lokasi kota yang jelas.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/cities/new%20york.jpg)

  Kita dapat melihat bahwa satu-satunya pengecualian adalah negara bagian New York. Ini menunjukkan bahwa dalam data kecelakaan di Texas, angka kecelakaan tertinggi tidak terkait dengan kota tertentu, sementara di New York, kota New York memiliki total 117 kecelakaan.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/urban%20vs%20rural-all.jpg)

  Selanjutnya, analisis dilakukan terhadap data yang berkaitan dengan jumlah kecelakaan yang terjadi di daerah pedesaan dan perkotaan. Hasil analisis ini memberikan gambaran tentang pola kecelakaan di berbagai tipe lingkungan. Ditemukan bahwa lebih dari setengah dari jumlah total kecelakaan untuk semua jenis kecelakaan tercatat di daerah perkotaan, yakni sekitar 57,5% dari total insiden (20.101). Sementara itu, jumlah kecelakaan di daerah pedesaan mencapai sekitar 42,5% (14.829).

### 3. Berdasarkan waktu terjadinya kecelakaan

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/month-all.jpg)

  Data yang berkaitan dengan jumlah kecelakaan yang terjadi pada setiap bulan kemudian diteliti. Analisis ini bertujuan untuk memahami pola kecelakaan selama berbagai musim di tahun 2021. Angka kecelakaan tertinggi terjadi pada bulan Oktober, dengan jumlah mencapai 3.517 insiden. Hal yang menarik adalah bahwa angka kecelakaan relatif stabil dari bulan Juni hingga Oktober. Di sisi lain, angka kecelakaan terendah tercatat pada bulan April, dengan jumlah kecelakaan mencapai 2.103 insiden.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/day-all.jpg)

  Hari dengan angka kecelakaan tertinggi adalah Minggu, dengan total 6.342 insiden. Ini merupakan temuan yang menarik karena Minggu sering kali dianggap sebagai hari libur dan mungkin ada faktor-faktor tertentu yang memengaruhi tingkat kecelakaan pada hari ini.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/all%20accident-avg%20per%20hour.jpg)

  Rata-rata jumlah kecelakaan tertinggi dalam satu hari tercatat pada pukul 12.00 siang, dengan rata-rata mencapai 5,9 insiden atau, jika dibulatkan, sekitar enam insiden. Temuan ini menunjukkan bahwa jam tengah hari adalah waktu di mana risiko kecelakaan rata-rata paling tinggi dalam satu hari. Tren ini kemudian tampak stabil hingga pukul 15.00 sore, artinya selama periode ini, angka kecelakaan cenderung tinggi dan konsisten.

### 4. Berdasarkan kondisi pengemudi ketika kecelakaan terjadi

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/drunk%20vs%20sober-all.jpg)

  Jumlah pengemudi yang tidak dalam keadaan mabuk lebih mendominasi, yaitu sekitar 74,2% dari total insiden kecelakaan (sebanyak 26.292 insiden). Sementara itu, pengemudi yang berada dalam keadaan mabuk saat mengalami kecelakaan hanya mencapai sekitar 25,8% (sebanyak 9.120 insiden). Temuan ini merupakan hal yang menarik karena mengindikasikan bahwa pengemudi yang tidak dalam keadaan mabuk mendominasi hampir tiga perempat dari keseluruhan jumlah kecelakaan yang tercatat.

![](https://github.com/jessie-kusumawardhani/jessie-kusumawardhani.github.io/blob/main/CHART%20screenshots/Total%20Crash%20by%20Hour%20(Sober%20vs.%20Drunk%20Driver).jpg)

  Jumlah kecelakaan tertinggi dalam satu hari terjadi pada pukul 12.00 siang untuk pengemudi yang tidak dalam keadaan mabuk dengan total 1.627 insiden. Di sisi lain, pengemudi yang berada dalam keadaan mabuk memiliki angka kecelakaan tertinggi pada pukul 17.00 sore dengan total 708 insiden.

## Kesimpulan

  Jenis kecelakaan umumnya tidak melibatkan kendaraan bermotor (21.768). Analisis masih tahap awal, mencari korelasi dengan jenis dan kondisi seperti jenis jalan, persimpangan, penerangan, dan cuaca. Kecelakaan paling banyak terjadi di jalan bervolume besar seperti Principal Arterial - Other, yang notabene dikategorikan sebagai jalan tanpa persimpangan. Insiden juga sebagian besar terjadi pada siang hari dan dalam keadaan cerah. Texas, California, dan Florida memiliki tingkat kecelakaan tertinggi. Sementara jumlah penduduk ketiga negara bagian juga tertinggi, terdapat anomali seperti banyak kota terjadinya kecelakaan tidak teridentifikasi. Lebih dari setengah kecelakaan terjadi di daerah perkotaan (57,5%). Kecelakaan mencapai puncaknya dari Juni hingga Oktober dan pada hari Minggu, terutama antara pukul 12.00 - 15.00, dengan sekitar enam kecelakaan pada pukul 12.00 siang oleh pengemudi yang tidak mabuk (74,2%).

## Rekomendasi

Di Amerika Serikat, siswa sekolah dapat [memperoleh](https://www.policygenius.com/auto-insurance/driving-age-by-state/#:~:text=In%20the%20U.S.%2C%20you%20can%20typically%20apply%20for%20your%20full%20driver%E2%80%99s%20license%20between%20the%20ages%20of%2016%20and%2018.) SIM pada usia 16-18 tahun, dengan beberapa negara bagian memberikan izin pada [usia](https://www.rhinocarhire.com/Drive-Smart-Blog/Minimum-Driving-Age-Country/Minimum-Driving-Age-State.aspx) 17 atau 18. Libur musim panas [berlangsung](https://moonpreneur.com/blog/usa-school-holiday-calendar/#:~:text=among%20all%20individuals.-,Summer%20Break%C2%A0,length%2C%20with%20some%20districts%20offering%20as%20many%20as%20three%20months%20off.,-Labor%20Day) dari Mei/Juni hingga Agustus/September. Ini mungkin menunjukkan kemungkinan pengendara muda yang melakukan perjalanan jauh selama liburan musim panas. Namun, diperlukan analisis lebih mendalam mengenai usia pengendara yang terlibat dalam kecelakaan untuk rekomendasi yang lebih tepat, seperti pelatihan atau izin khusus untuk pengendara muda yang melakukan perjalanan jauh. Selain itu, pembatasan volume pengendara pada siang hari juga dapat diterapkan, terutama pada hari Minggu antara 12.00-15.00, dan dara mengenai jenis kendaraan yang terlibat dalam kecelakaan (motor, mobil, bus, truk) perlu dipertimbangkan untuk meningkatkan keselamatan jalan raya dan mengurangi kecelakaan ke depannya.
