1.  perbedaan antara asynchronous programming dengan synchronous programming.
    Dalam pemrograman synchronous, tugas-tugas dijalankan secara berurutan satu per satu, yang berarti program menunggu setiap tugas saat ini selesai sebelum melanjutkan ke tugas berikutnya. Analoginya, seperti antrian di toko atau bank, di mana setiap orang harus menunggu giliran mereka selesai sebelum orang berikutnya dapat dilayani.
    Sementara dalam pemrograman asynchronous, program tidak menunggu operasi untuk selesai. Sebaliknya, program terus menjalankan eksekusi dan kemudian dapat memeriksa hasil operasi tersebut di kemudian hari. Ini memungkinkan program untuk menjalankan banyak operasi secara bersamaan tanpa harus menunggu satu operasi selesai sebelum operasi lainnya dimulai.

2. Dalam penerapan JavaScript dan AJAX, terdapat penerapan paradigma event-driven programming. Jelaskan maksud dari paradigma tersebut dan sebutkan salah satu contoh penerapannya pada tugas ini.
    
    Paradigma Event-Driven Programming adalah metode dalam pemrograman di mana jalannya program ditentukan oleh kejadian yang terjadi, bukan hanya oleh urutan instruksi dalam kode program. Dalam konteks JavaScript dan penggunaan AJAX (Asynchronous JavaScript and XML) dalam aplikasi web, paradigma ini memiliki relevansi yang signifikan.
    Sebagai contoh dalam paradigma pemrograman berbasis peristiwa dan penggunaan AJAX, kita dapat membuat sebuah formulir yang memungkinkan pengiriman data ke server tanpa memerlukan pengguliran ulang halaman web. Formulir ini menggunakan XMLHttpRequest untuk mengirim permintaan dan menerima respons dari server secara asinkron. Formulir ini juga dapat menambahkan pendengar peristiwa pada elemen input atau tombol untuk menanggapi tindakan seperti klik, tekan, atau perubahan. Selain itu, formulir ini mampu menampilkan hasil atau pesan dari server di elemen HTML tertentu.

3. Jelaskan penerapan asynchronous programming pada AJAX.
    Pemrograman asinkron dalam konteks AJAX adalah metode yang memungkinkan aplikasi web berkomunikasi dengan server tanpa harus menunggu respons. Pendekatan ini meningkatkan efisiensi dan responsivitas aplikasi web karena tidak perlu me-refresh halaman web setiap kali ada permintaan data. Dalam pemrograman asinkron di AJAX, JavaScript berfungsi sebagai bahasa pemrograman utama untuk mengirim dan menerima data dari server secara non-sinkron. Selain itu, JavaScript juga mampu mengubah tampilan pengguna sesuai dengan data yang diterima atau dikirim, menciptakan pengalaman pengguna yang lebih dinamis dan interaktif

4. Pada PBP kali ini, penerapan AJAX dilakukan dengan menggunakan Fetch API daripada library jQuery. Bandingkanlah kedua teknologi tersebut dan tuliskan pendapat kamu teknologi manakah yang lebih baik untuk digunakan.
    - Fetch API adalah fitur bawaan dari browser modern yang berarti Ini berarti Fetch API lebih ringan dan tidak bergantung pada library lain, Namun jQuery adalah library eksternal yang harus diunduh dan dimuat terlebih dahulu sehingga jQuery lebih kompatibel dengan browser lama yang belum mendukung Fetch API1.
    -  jQuery menawarkan antarmuka yang lebih sederhana untuk tugas seperti pengiriman data JSON, sementara Fetch API membutuhkan lebih banyak kode untuk tugas yang serupa, tetapi memberikan lebih banyak kontrol dan fleksibilitas dalam hal permintaan dan respons Ajax.
    - Fetch API menggunakan konsep Promise untuk mengatasi respon asinkron, yang dianggap lebih elegan dan mudah dibaca dalam penulisan kode asinkron, sementara jQuery menggunakan callback yang lebih fleksibel, meskipun dapat digunakan dalam kasus-kasus yang lebih kompleks.
    -  Fetch API menyediakan metode bawaan untuk mengubah respons menjadi berbagai tipe data, sedangkan jQuery memerlukan penentuan jenis data sebelumnya dengan opsi dataType.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
    - Langkah awal say membuat fungsi bernama "get_item_json" di dalam "views.py" untuk mengambil data dalam format JSON. Selanjutnya, saya perlu membuat sebuah fungsi baru yang akan menambahkan produk menggunakan AJAX. Dalam fungsi ini, saya harus mengimpor "csrf_exempt" dan menuliskan kode di atasnya, dengan nama fungsi "add_item_ajax."
    - kemudian pada halaman main_html saya membuat fungsi refreshProducts()', fungsi asinkron 'refreshCards', dan 'addProduct()' untuk memunculkan table dan cards menggunakan AJAX dan merefresh data dari item serta mengupdate informasi jumlah item yang tersimpan secara asynchronous.
    - Setelah itu saya menambahkan image_url = models.TextField() pada models, lalu menambahkan fields dengan "image_url", lalu saya melakukan migrations.