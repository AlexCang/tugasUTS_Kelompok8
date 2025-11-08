# AI AGE PREDICTION
### DESKRIPSI SINGKAT

Aplikasi ini merupakan sebuah sistem prediksi usia berbasis kecerdasan buatan (AI) yang memungkinkan pengguna mengupload gambar wajah, lalu aplikasi akan menganalisis dan memperkirakan umur orang pada foto tersebut secara otomatis. Aplikasi ini berfungsi sebagai contoh implementasi AI di bidang Computer Vision, khususnya dalam penentuan usia berdasarkan citra wajah.

Aplikasi ini tersusun dari dua komponen utama :
1. Model AI / Machine Learning

Model dilatih menggunakan dataset UTKFace, sebuah kumpulan data yang berisi foto wajah manusia beserta label usia. Arsitektur yang digunakan adalah MobileNetV2 melalui transfer learning, sehingga model tetap ringan dan efisien untuk dijalankan pada perangkat mobile. Model menghasilkan output berupa angka usia (regresi), bukan klasifikasi kategori umur. Proses training dilakukan melalui dua tahap: feature extraction dan fine-tuning. Model memiliki tingkat error yang relatif rendah, berkisar 4–6 tahun dari umur asli.

2. Aplikasi Mobile Flutter

Pengguna dapat melakukan capture foto dari kamera atau memilih dari galeri. Gambar dikirim untuk diprediksi oleh model AI, lalu hasilnya ditampilkan langsung pada layar.
Hasil prediksi terdiri dari: Gambar input; Usia estimasi dalam satuan tahun; Tombol untuk menyimpan hasil prediksi ke Firebase; Tampilan aplikasi menggunakan tema dark futuristik dengan aksen neon biru.
Aplikasi terdiri dari beberapa halaman utama: Halaman input foto;  Halaman hasil prediksi;  Halaman riwayat prediksi yang tersimpan (History).

ANGGOTA 1 : ALEXANDER CANGNAKA - 221110796

ANGGOTA 2 : PATRICK SANUSI     - 221110348

ANGGOTA 3 : MUHAMMAD LUTHFI ANANDA LUBIS - 221113040

URL APLIKASI LIVE : https://mikroskilacid-my.sharepoint.com/:f:/g/personal/221110796_students_mikroskil_ac_id/EpmlkIM5SvZBlOkTkAcGha8BUmvehK6D3leL-B4SZZAszA?e=qcF5Sx

URL ONE DRIVE     : https://mikroskilacid-my.sharepoint.com/:f:/g/personal/221110796_students_mikroskil_ac_id/ElOWeDHZ5sNMgSe19Ft4d5IBTsk-sZ5EfUNRk3mJzpOe_g?e=jJOZG7

### PETUNJUK PENGGUNAAN APLIKASI :

1. Pada layar Home Page, terdapat beberapa tombol yaitu tombol Take Photo, Upload From Gallery, dan View History. Tombol Take Photo akan langsung mengambil foto dari kamera pada Smartphone, namun sebelum itu, pengguna wajib memberikan akses terlebih dahulu. Tombol Upload From Gallery berfungsi untuk mengakses gallery pada Smartphone dan mengambil foto yang hendak diprediksi umurnya. Tombol View History merupakan tombol untuk melihat riwayat dari foto-foto yang sudah diprediksi sebelumnya.

2. Selanjutnya adalah layar Result, yang merupakan layar yang menampilkan hasil dari prediksi umur pada foto yang sudah diambil pengguna ataupun diupload pengguna dari layar Home Page. Pada layar ini, akan menampilak prediksi umur dari foto, lalu terdapat tombol Save Result untuk menyimpan data hasil prediksi tersebut ke dalam aplikasi dan Firebase Database dan Firebase Storage. Dibawah tombol Save Result terdapat tombol View History yang akan membawa pengguna menuju ke layar riwayat prediksi umur pada aplikasi. Apabila tombol Save Result ditekan, maka hasil prediksi umur tersebut berupa gambar, umur, dan kapan data tersebut diambil ,akan segera diupload ke dalam Firebase Database dan Firebase Storage.

3. Setelah penyimpanan berhasil, maka pengguna dapat melihat riwayat prediksi umur pada layar History. Pada layar ini, pengguna dapat menghapus riwayat prediksi umur dan riwayat tersebut akan langsung terhapus dari Firebase Database dan Firebase Storage. Apabila pengguna ingin melihat riwayat secara detil, maka pengguna bisa menekan riwayat yang diinginkan.

4. Pada layar Detail History, maka pengguna dapat melihat lebih jelas gambar yang sudah di-upload, umur prediksi, dan timestamp dari gambar yang diambil tersebut.

### PETUNJUK INSTALASI BAGI PENGGUNA :

1. Pengguna meng-install terlebih dahulu link URL aplikasi yang sudah disediakan di GitHubRepository.

2. Setelah pengguna meng-install aplikasi, maka pengguna akan langsung menuju ke layar Home Page untuk meng-upload foto atau gambar yang ingin diprediksi umurnya.

### PETUNJUK INSTALASI BAGI DEVELOPER :

1. Developer hanya perlu mengunduh file ZIP yang sudah disediakan pada GitHubRepository.

2. Kemudian developer melakukan perintah flutter pub get pada terminal Visual Studio Code.

3. Developer bisa mengubah kode apapun yang terdapat pada file ZIP tersebut dan bisa mengubah kode program aplikasi tersebut menjadi lebih advance.

4. Developer juga bisa mengkoneksikan flutter App tersebut ke Firebase Database dan Storage sendiri dengan cara membuat terlebih dahulu projek Firebase dan mengunduh file google-services.json. Kemudian developer bisa mengikuti arahan dari Firebase itu sendiri untuk menyempurnakan koneksi antara flutter App dengan Firebase.
