1. Apa itu Django UserCreationForm, dan jelaskan apa kelebihan dan kekurangannya?
    Django UserCreationForm adalah Formulir bawaan Django untuk membuat atau mendaftarkan pengguna baru di situs web yang dibangun oleh django.
    Kelebihan:
    - UserCreationForm telah dirancang sedemikian rupa hingga mudah untuk digunakan
    - Formulir ini sudah terintegrasi dengan baik dengan sistem otentikasi Django.
    - Validasi yang otomatis untuk memeriksa apakah data yang dimasukkan sudah sesuai dengan persyaratan (misal: panjang karakter password dan password hanya boleh terdiri dari angka dan huruf)
    
    kekurangan:
    - tidak dapat digunakan untuk semua kasus, misal sebuha aplikasi membutuhkan lebih banyak informasi pelanggan atau autentikasi yang berbeda. Dalam hal ini kita diperlukan untuk membuat kustom sendiri
    - memliki ketergantungan terhadap django 
    - tidak dapat mengelola emmail konfirmasi secara otomatis.

2. Apa perbedaan antara autentikasi dan otorisasi dalam konteks Django, dan mengapa keduanya penting?
    - Autentikasi merupakan proses identitas pengguna, memastikan jika pengguna adalah pengguna yang sah. 
    - Otorisasi adalah penentuan izin atau hak akses yang dimiliki pengguna setelah di autentikasi, seperti mengatur apa yang boleh diakses pengguna dalam aplikasi.

    Autentikasi dan otorisasi merupakan konsep penting dalam pengembangan aplikasi web, meskipun kefuanya terikat dengan erat namun keduanya memiliki perbedaan seperti yang sudah saya sebutkan diatas. Dengan menerapkan konsep Autentikasi dan Otorisasi, kita dapat membangun aplikasi web yang aman, sesuai dengan kebutuhan bisnis dan pengguna aplikasi web, cdan mematuhi hukum dan etika.

3. Apa itu cookies dalam konteks aplikasi web, dan bagaimana Django menggunakan cookies untuk mengelola data sesi pengguna?
    Cookies dalam konteks web adalah data kecil yang disimpan oleh server web pada setiap perangkat pengguna. Cookies digunakan utnuk melacak informasi sesi pengguna. Django menggunakan cookies untuk menyimpan informasiyang diperlukan untuk mengidentifikasi dan memelihara sesi pengguna.

    penggunaan Django terhadap cookies:
    - pada tahap awal ketika pengguna registrasi pada situs Django, Django akan memebuat cookie dengaan id unik untuk pengguna tersebut,
    - kemudian pengembang web dapat menyimpan data dalam sesi pengguna, kemudian data tersebut kana dienkripsi dam disimpan dalam cookie,
    - pada saat pengguna login, Django akan mengambil id unik cookie pengguna untuk mengambil data sesi dari pengguna,
    - selain itu kita juga dapat menghapus atau memperbaharui data sesi pengguna sesuai dengan kebutuhan.

4. Apakah penggunaan cookies aman secara default dalam pengembangan web, atau apakah ada risiko potensial yang harus diwaspadai?
    penggunaan cookies dalam pengembangan web tidak sepenuhnya aman masih ada risiko potensial yang harus diwaspadai, berikut contoh risiko yang harus diwaspadai dalam penggunaan cookie:
    - Cross-Site (XSS)
    - Session Fixation
    - Session Hijacking
    - eavesdropping (penyadapan)
    - Cookie Theft
    namun dengan praktik keamanan yang tepat penggunaan cookie dapat dibilang relatif aman.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
    Berikut merupakan langkah langkah yang saya implementasikan untuk mengerjakan checklist diatas:
    - pertama saya membuat Form registrasi, login, logout dengan cara mengimpor beberapa fungsi termasuk UserCreationForm, membuat fungsi registasi, login, logout yang disimpan di bagian views agar data pengguna akan secara otomatis terdaftar ketika di submit form, membuat Halaman registrasi dan login pada bagian template, dan membuat path untuk registrasi, login, logout agar fungsi dapat di akses.
    - Selanjutnya, membuat dua akun pada web dan memasukkan 3 dummy data, agar 3 dummy data dalam kedua akun tersebut tidak tercampur, maka kita harus menghubungkan model Item dengan user dengan menggunakan Foreignkey untuk menghubungkan satu data dengan satu pengguna saaja atau pengguna tertentu. kemudian mengubah fungsi create produk dengan menambahkan perintah request.user untuk menandakan bahwa objek tersebut milik pengguna yang login. pada bagian show_main product juga di ubah agar terfilter menggunakan filter(user = request.user). tidak lupa untuk melakukan migrasi setiap melakukan perubahan atau penambahan pada model.
    - checklist selanjutnya dalah penggunaan cookie untuk data sesi pengguna yaitu lastlogin, langkah awal import datetime terlebih dahulu kemudian pada bagian fungsi login_user yang sudah dibuat tambahkan set.cookie lastlogin dan import fungsi datetime, lalu menambhakan potongan kode request cookie pada fungsi show_main agar menmabhakna informasi last login dalam halaman web.kemudian mendelete cookie pada fungsi logout user, kemudian data last login akan ditampilkan dengan terlebih dahulu menmabahkan perintah last login pada main html 
