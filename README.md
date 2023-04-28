# SPARK-SQL-BIG-DATA
NAMA : Welson Mario Naibaho

KELAS : TI 3C

NIM : 2041720253

MATAKULIAH : BIG DATA

# TUGAS 1

PERTANYAAN

Jelaskan masing-masing dari code berikut sesuai nomor code.

Kode 1 : myList, myschema

Kode 2 : spark.createDataFrame

Kode 3 : parallelize, toDF

Kode 4 : hadoop, fs, put

Kode 5 : pyspark.sql, SQLContext, createOrReplaceTempView, show

Kode 6 : textFile, map, lamda, strip, StructField, Stringtype

Kode 7 : spark.read.format, jdbc, options, load

Kode 8 : show

Kode 9 : collect, rdd, take

Kode 10 : makeRDD, Seq, createDataset

Kode 11 : filter

Kode 12 : as, toDF, first

Kode 13 : listDatabase, listTables, listFunction, isCached, select

Kode 14 : Read, text

Kode 15 : load, json, format, printSchema

Kode 16 : write, save

Kode 17 : parquet

Kode 18 : Options, inferSchema, csv, header, codec

## KODE 1
    1. mylist = digunakan sebagai tipe data untuk menyimpan data yang akan diproses dalam RDD atau DataFrame. List bisa diubah menjadi RDD dengan menggunakan fungsi parallelize dan toDF untuk diubah menjadi DataFrame.

    2. myschema = digunakan untuk mendefinisikan struktur dari sebuah DataFrame.

## KODE 2
    1. spark.createDataframe = digunakan untuk membuat sebuah DataFrame dari suatu RDD atau Dataset.

## KODE 3
    1. parallelize = digunakan untuk membuat sebuah RDD (Resilient Distributed Dataset) dari suatu koleksi data yang ada di dalam memori.
    
    2. toDF = digunakan untuk mengubah sebuah RDD (Resilient Distributed Dataset) menjadi sebuah DataFrame. toDF menerima parameter berupa nama-nama kolom untuk DataFrame yang dihasilkan, atau bisa juga tidak memiliki parameter untuk menghasilkan DataFrame dengan kolom-kolom default ("_1", "_2", dst).

## KODE 4
    1. hadoop = adalah sebuah framework open-source untuk menyimpan dan memproses data besar secara terdistribusi. Apache Spark, di sisi lain, adalah sebuah framework open-source untuk komputasi data yang cepat dan umumnya digunakan untuk mengolah data dalam jumlah besar secara terdistribusi.

    2. fs = digunakan untuk mengakses file system secara terdistribusi. Package fs pada Spark mendukung beberapa jenis file system, termasuk Hadoop Distributed File System (HDFS), Local file system, Amazon S3, dan Google Cloud Storage.

    3. put = adalah salah satu perintah pada command line interface (CLI) dari Apache Hadoop HDFS yang digunakan untuk meng-upload file dari local file system ke HDFS.

## KODE 5
    1. pyspark.sql = adalah package pada Apache Spark yang digunakan untuk mengakses data terstruktur menggunakan SQL dan DataFrame API pada lingkungan pemrograman Python. Package ini memungkinkan kita untuk melakukan query terhadap data terstruktur yang disimpan dalam format seperti CSV, JSON, Parquet, dan lainnya.

    2. SQLContext = digunakan untuk mengakses data terstruktur menggunakan SQL pada lingkungan pemrograman Scala, Java, dan Python. Class ini digunakan sebelum Spark 2.0, sekarang sudah digantikan dengan SparkSession. Namun, SQLContext masih dapat digunakan pada Spark versi lama.

    3. createOrReplaceTempView = digunakan untuk membuat atau mengganti tampilan sementara (temporary view) pada suatu DataFrame.

    4. Show = adalah salah satu metode yang tersedia di Apache Spark yang digunakan untuk menampilkan data dari DataFrame. Dalam Spark, DataFrame adalah struktur data yang terdiri dari kolom dan baris, mirip dengan tabel dalam database relasional. show digunakan untuk menampilkan data DataFrame dalam format tabular yang mudah dibaca. Secara default, metode show akan menampilkan 20 baris pertama dari DataFrame. 

## KODE 6
    1. textFile = digunakan untuk membaca file teks dari sistem file Hadoop, S3, atau sistem file lainnya dan mengembalikan RDD yang berisi baris-baris dari file tersebut.

    2. map = digunakan untuk mengaplikasikan suatu fungsi pada setiap elemen RDD dan mengembalikan RDD baru yang terdiri dari hasil fungsi tersebut.

    3. lambda =  adalah sebuah konsep dasar pada bahasa pemrograman Python yang digunakan untuk membuat fungsi anonim atau tidak diberi nama.

    4. strip = digunakan untuk membersihkan atau menghilangkan karakter whitespace pada data yang dibaca dari file atau sumber data lainnya.

    5. StructField = digunakan untuk merepresentasikan sebuah kolom dalam sebuah schema tabel. Setiap StructField mendefinisikan sebuah nama kolom, tipe data kolom, dan apakah kolom tersebut dapat memiliki nilai null atau tidak.

    6. StringType = digunakan untuk merepresentasikan kolom dengan tipe data string atau teks. Tipe data ini dapat digunakan pada definisi schema tabel atau pada konversi tipe data pada DataFrame.

## KODE 7
    1. spark.read.format = adalah salah satu metode yang digunakan di Apache Spark untuk membaca data dari berbagai sumber data seperti file CSV, JSON, Parquet, Avro, dan lain-lain. Dalam Spark, metode ini memungkinkan pengguna untuk menentukan format data yang akan dibaca.

    2. jdbc = adalah salah satu modul yang tersedia di Apache Spark yang digunakan untuk membaca dan menulis data dari database menggunakan JDBC (Java Database Connectivity). Dengan menggunakan modul ini, pengguna dapat mengakses data yang disimpan di database, seperti MySQL, Oracle, SQL Server, dan lain-lain, dari lingkungan Spark.

    3. options = adalah salah satu parameter yang tersedia di Apache Spark yang digunakan untuk menentukan opsi konfigurasi saat membaca atau menulis data dari atau ke sumber eksternal. Opsi-opsi ini berbeda-beda tergantung pada jenis sumber data yang digunakan.

    4. load = digunakan untuk memuat data ke dalam DataFrame dengan format tertentu, seperti CSV, JSON, parquet, atau ORC. Pengguna dapat menentukan format file dengan menggunakan argumen pada metode

## KODE 8
    1. show = adalah salah satu metode yang tersedia di Apache Spark yang digunakan untuk menampilkan data dari DataFrame. Dalam Spark, DataFrame adalah struktur data yang terdiri dari kolom dan baris, mirip dengan tabel dalam database relasional. show digunakan untuk menampilkan data DataFrame dalam format tabular yang mudah dibaca. Secara default, metode show akan menampilkan 20 baris pertama dari DataFrame.

## KODE 9
    1. collect = digunakan untuk mengambil seluruh data dari DataFrame ke dalam bentuk Python list. Metode ini akan mengumpulkan semua data pada executor dan mengirimkannya kembali ke driver node, sehingga dapat mengakibatkan overhead yang besar terutama jika jumlah data yang diolah sangat besar.

    2. rdd = RDD adalah kumpulan data yang terdistribusi di seluruh node dalam sebuah cluster, yang dapat diproses secara terpisah dan paralel. Pengguna dapat melakukan operasi map, filter, join, dan sebagainya pada RDD, dan Spark akan secara otomatis membagi pekerjaan tersebut di antara node dalam cluster.

    3. take = digunakan untuk mengambil sejumlah baris dari sebuah RDD atau DataFrame dan mengembalikan hasilnya ke driver node dalam bentuk Python list.

## KODE 10
    1. makeRDD = digunakan untuk membuat RDD baru dari data yang sudah ada di dalam memori. Metode ini digunakan untuk membuat RDD dari data yang disediakan secara eksplisit oleh pengguna, seperti list, tuple, atau array.

    2. Seq = adalah tipe data di Scala yang merepresentasikan sebuah urutan dari elemen-elemen yang dapat diakses secara berurutan. Pada Spark, Seq biasanya digunakan sebagai parameter input untuk metode yang memerlukan sebuah kumpulan data atau sekumpulan nilai.
    
    3. createDataset = digunakan untuk membuat sebuah Dataset, yaitu sebuah struktur data yang mirip dengan DataFrame, tetapi memiliki tipe data yang terjaga (strongly-typed) dan mendukung pemrograman fungsional. createDataset menerima sebuah Seq (sequence) atau List dari objek-objek yang ingin dibuatkan Dataset-nya.

    

## KODE 11
    1. filter = digunakan untuk melakukan filtering (penyaringan) pada sebuah Dataset atau DataFrame dengan kriteria tertentu. filter menerima sebuah ekspresi boolean sebagai parameter, dan mengembalikan sebuah Dataset atau DataFrame yang hanya berisi baris-baris yang memenuhi kriteria tersebut.

## KODE 12
    1. as = digunakan untuk memberikan alias (nama lain) pada sebuah kolom dalam sebuah DataFrame atau Dataset. Alias ini bisa berguna untuk memberikan nama yang lebih deskriptif dan mudah dipahami pada kolom-kolom yang dihasilkan dari operasi-operasi transformasi pada DataFrame.

    2. toDF = digunakan untuk mengubah sebuah RDD (Resilient Distributed Dataset) menjadi sebuah DataFrame. toDF menerima parameter berupa nama-nama kolom untuk DataFrame yang dihasilkan, atau bisa juga tidak memiliki parameter untuk menghasilkan DataFrame dengan kolom-kolom default ("_1", "_2", dst).

    3. first = digunakan untuk mengembalikan elemen pertama dari RDD. Metode ini mengambil satu elemen pertama dari RDD dan mengembalikannya ke driver program. Metode first sangat berguna ketika pengguna ingin melihat elemen pertama dari RDD, seperti ketika ingin memeriksa struktur dari data yang sedang diolah.

## KODE 13
    1. listDatabase = digunakan untuk mengembalikan daftar database yang tersedia di semua sesi.

    2. listTables = digunakan untuk mengembalikan daftar tabel/tampilan dalam database yang ditentukan.

    3. listFunctions = digunakan untuk mengembalikan daftar fungsi yang terdaftar di database yang ditentukan.

    4. isCached = digunakan untuk mengembalikan nilai true jika tabel saat ini di-cache dalam memori.

    5. select = digunakan untuk memproyeksikan sekumpulan ekspresi dan mengembalikan DataFrame baru.

## KODE 14
    1. Read = digunakan untuk menyesuaikan cara data dibaca dari source data.

    2. text = digunakan untuk membaca file teks ke dalam DataFrame.

## KODE 15
    1. load = digunakan untuk memuat data dari source data dan mengembalikannya sebagai DataFrame.

    2. json = digunakan untuk membaca file JSON ke dalam Spark DataFrame

    3. format = digunakan untuk load sebuah file atau memformat hasil file dengan tipe data tertentu

    4. printSchema = digunakan untuk mencetak skema dataframe dalam format tree.

## KODE 16
    1. write = digunakan untuk menulis data dari sebuah DataFrame ke berbagai format file atau sink data seperti parquet, CSV, JSON, dan JDBC.

    2. save = digunakan untuk menyimpan data dari sebuah DataFrame ke berbagai format file atau sink data seperti parquet, CSV, JSON, dan JDBC.

## KODE 17
    1. parquet = digunakan untuk menyimpan data secara kolomar dalam bentuk kompresi, yang terdiri dari beberapa baris dan kolom. Parquet dirancang untuk mengoptimalkan proses analisis data, terutama pada Big Data, dengan mengurangi waktu pembacaan dan memori yang dibutuhkan untuk mengakses data.

## KODE 18
    1. Options = digunakan untuk mengatur berbagai opsi konfigurasi seperti delimiter, header, inferSchema dll

    2. inferSchema = adalah opsi konfigurasi saat membaca data dari format file seperti CSV, TSV, dan lain-lain. Saat inferSchema diaktifkan, Spark akan mencoba mengidentifikasi tipe data dari setiap kolom secara otomatis berdasarkan pada nilai yang ada pada baris pertama atau beberapa baris awal data.

    3. csv = digunakan untuk memuat file CSV dan mengembalikan hasilnya sebagai DataFrame.

    4. header = Saat header diaktifkan, Spark akan menganggap bahwa baris pertama dari file tersebut berisi header atau nama kolom.

    5. codec = digunakan untuk menentukan codec kompresi yang akan digunakan saat pada output. contoh codec yang disupport adalah gzip, snappy, dan bzip2.


