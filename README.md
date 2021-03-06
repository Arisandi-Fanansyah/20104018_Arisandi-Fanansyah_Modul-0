# 20104018_Arisandi-Fanansyah_Modul-0
# Modul 0 : Dasar Pemrograman Java

# Dasar Teori
A. DASAR TEORI
 
  Penamaan identifier harus diawali dengan karakter unicode, tanda $ (dollar) atau tanda _ (underscore). Penamaan identifier ini bersifat casesensitive dan tidak dibatasi panjang maksimum.
  
 1. Keyword dalam Java

  Kata kunci adalah identifier yang telah dipesan untuk didefinisikan sebelumnya oleh Java untuk tujuan tertentu. Anda tidak dapat menggunakan keyword sebagai nama variabel, class, method.
  
Berikut Ini Keyword Java :
 - abstract default if      private throws
 - boolean  do      import  public  Tr
 - break    double  int     return  void
 - byte     else    static  short   while
 - case     extends long    super   const
 - catch    final   native  switch  For
 - char     finally new     this    Continue
 - class    float   package throw   Transient
  
  Kata-kata kunci tersebut tidak bisa dipakai sebagai identifier. Selain kata kunci, Java juga mempunyai 3 kata literal, yaitu true, false dan true, yang juga tidak bisa dipakai untuk penamaan identifier.
  
- Tipe Dasar

  Java mempunyai 8 tipe dasar, yaitu boolean, char, byte, short, int, long, float, dan double. Spesifikasi panjang bit dan range untuk masingmasing tipe adalah sebagai berikut:
  
Tipe      Panjang Bit   Range
Boolean       16          -
Char          16       0 – 216-1
Byte           8      -27 – 27-1
Short         16     -215 – 215-1
Int           32     -231 – 231-1
Long          64     -263 – 263-1
Float         32          -
Double        64          -

  Nilai default untuk masing-masing tipe adalah sebagai berikut:
  
Tipe      Nilai Default
Boolean       False
Char         ‘\u0000’
Byte             0
Short            0
Int              0
Long             0L
Float           0.0F
Double          0.0

- Variabel

 Variabel adalah item yang digunakan data untuk menyimpan pernyataan objek. Variabel memiliki tipe data dan nama. Tipe data menandakan tipe nilai yang dapat dibentuk oleh variabel itu sendiri. Nama variabel harus mengikuti aturan untuk identifier.

 Berikut Aturan penamaan variable :
 
a. Diawali dengan : huruf/abjad atau karakter mata uang atau underscore ( _ ).
b. Terdiri dari huruf/abjad, angka dan underscore.
c. Tidak boleh mengandung karakter khusus atau spasi.
d. Tidak boleh diawali dengan angka.

- Casting dan Promotion

 Casting diperlukan untuk mengkonversi dari suatu tipe ke tipe data yang lebih kecil panjang bitnya. Sedangkan promotion terjadi pada saat mengkonversi dari suatu tipe data ke tipe data yang lebih panjang bitnya.

Contoh :
```java
int p = (int) 10L;
long i = 10;
```
# Praktikum
 Soal:
  1. Menganalisa batasan maksimum dari suatu tipe
  2. Anak Ayam
  3. A + B - C
 
 Jawaban :
 
  1. [Jawaban Soal 1](https://github.com/Arisandi-Fanansyah/20104018_Arisandi-Fanansyah_Modul-0/blob/main/latihan/BigInteger.java)
  
  ```java
  long p = 2147483648;
  ```
  
  Syntax diatas akan menampilkan error :
  
  ```java
  C:\Users\Arisandi_F\IdeaProjects\PraktikumPBO\src\main\java\com\Arisandi\pbo\modul2\latihan\BigInteger.java:5: error: integer number too large: 2147483648
  ```
  
  Alasan error itu terjadi padahal daya tampung pada tipe data long adalah 2^63-1 ?
  Karena java hanya membaca syntax tersebut dengan tipe data integer bukan tipe data long. jika ingin menggunakan tipe data long, maka syntax diatas harus menambahkan huruf yang biasa disebut suffix yaitu "L" pada akhir angka, agar data terseut dapat dibaca oleh java dengan tipe data long.
  
  Contoh :
  ```java
  long p = 2147483648L;
  ```
  
  2. [Jawaban Soal 2](https://github.com/Arisandi-Fanansyah/20104018_Arisandi-Fanansyah_Modul-0/blob/main/latihan/Anak_Ayam.java)
  
  Hasil run program
  
  ```java
  Masukkan jumlah anak ayam : 10
Tek kotek kotek kotek, anak ayam turun berkotek

Anak ayam turun 10, mati 1 tinggal 9.

Anak ayam turun 9, mati 1 tinggal 8.

Anak ayam turun 8, mati 1 tinggal 7.

Anak ayam turun 7, mati 1 tinggal 6.

Anak ayam turun 6, mati 1 tinggal 5.

Anak ayam turun 5, mati 1 tinggal 4.

Anak ayam turun 4, mati 1 tinggal 3.

Anak ayam turun 3, mati 1 tinggal 2.

Anak ayam turun 2, mati 1 tinggal 1.

Anak ayam turunlah 1, mati satu tinggal Induknya

Process finished with exit code 0

  ```
  
  3. [Jawaban Soal 3](https://github.com/Arisandi-Fanansyah/20104018_Arisandi-Fanansyah_Modul-0/blob/main/latihan/Sistem_Operasi.java)
  
  Hasil run program
  
  ```java
  Sistem Operasi
Hasil Case 1 : 1
Hasil Case 2 : 3

Process finished with exit code 0
  ```
  
# Kesimpulan
Kesimpulan yang saya dapatkan pada pembelajaran kali ini yaitu saya dapat mengetahui aturan penamaan identifier, mengenal kata-kata kunci yang terdapat pada Java, mengetahui tipe-tipe dasar yang ada pada Java, dan mengetahui penggunaan variable pada Java.
