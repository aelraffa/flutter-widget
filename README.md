# flutter_widget

Proyek ini adalah aplikasi Flutter sederhana untuk latihan penggunaan widget dasar.

## Getting Started

Repositori ini bisa dijadikan titik awal untuk belajar pengembangan aplikasi Flutter.

Jika baru mulai belajar Flutter, beberapa referensi berikut bisa membantu:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

Dokumentasi resmi Flutter juga menyediakan tutorial, contoh implementasi, panduan mobile development, dan referensi API lengkap:
[online documentation](https://docs.flutter.dev/)

## Widget yang saya temukan

### 1. Root Widget (MyApp)

Aplikasi dijalankan melalui fungsi berikut:

runApp(const MyApp());

MyApp ini berperan sebagai root widget dari aplikasi.

Di dalam MyApp ada beberapa komponen utama:

- MaterialApp
- home: RowColumnPage() sebagai halaman pertama saat aplikasi dibuka

### 2. Halaman Utama: RowColumnPage (Scaffold)

Pada halaman ini digunakan Scaffold sebagai kerangka utama tampilan. Isinya terdiri dari:

1. AppBar
   - Text('My First App')
2. Body
   - Column

### 3. Isi Body (Column)

#### A. Container (Gambar)

Bagian ini menampilkan gambar dari web picsum.photos.

Widget AspectRatio dipakai agar area gambar tetap proporsional, lalu diposisikan di tengah menggunakan Center.

#### B. Container (Teks)

Bagian ini menampilkan teks di bawah gambar.

Teks Text('What image is that') diletakkan di dalam Container, lalu diberi margin, padding, dan warna latar.

#### C. Container (Kategori Ikon)

Bagian ini menampilkan tiga kategori dengan kombinasi Row dan Column.

Row digunakan untuk menyusun item secara horizontal. Setiap item berisi Column kecil yang terdiri dari Icon dan Text, yaitu Food, Scenery, dan People.

#### D. Counter (StatefulWidget)

Bagian ini menunjukkan penggunaan StatefulWidget untuk membuat fitur counter sederhana.

CounterCard menampilkan nilai counter melalui Text, kemudian menyediakan IconButton(Icons.add) untuk menambah nilai. Saat tombol ditekan, setState dipanggil agar tampilan langsung diperbarui.

Nilai counter akan bertambah setiap kali tombol + ditekan.