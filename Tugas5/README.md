1. Jelaskan manfaat dari setiap element selector dan kapan waktu yang tepat untuk menggunakannya.
    - Selektor ID adalah alat untuk memilih elemen HTML berdasarkan atribut ID yang harus unik, berguna saat ingin menerapkan gaya pada elemen tertentu.
    - Selektor Kelas berfungsi untuk memilih elemen HTML berdasarkan atribut kelas yang dimilikinya.
    - Selektor Universal digunakan untuk memilih semua elemen dalam HTML dengan menggunakan tanda "*". Selektor ini berguna saat ingin menerapkan gaya yang sama pada semua elemen.
    - Elemen Style berisi informasi gaya untuk dokumen atau sebagian dari dokumen, sering dibuat dalam file terpisah seperti CSS, yang kemudian digunakan untuk menerapkan gaya pada elemen-elemen HTML.

2. Jelaskan HTML5 Tag yang kamu ketahui.
    - <html> --> tag yang digunakan saat awal membuat dokumen html. semua elmen HTML ditaruh didalam tag <html> ini.
    - <body> --> tag yang digunakan untuk menampilkan semua konten yang akna muncul pada halaman web, seperti teks, gambar, tautan, dan lainnya
    - <head> --> tag yang digunakan untuk memberikan informasi seperti judul halaman, meta-informasi, dan lainnya. Isi dalam tag ini tidak ditampilkan di halaman web
    - <a> --> tag a merupakan singkatan dari anchor yang digunakan untukmembuat tautan dalam halaman web dengan menggunakan atribut href untuk menentukan url yang ditujusaat tautan dilink
    -<img> --> tag yang digunakan untuk menampilkan gambar dalam halaman web.

3. Jelaskan perbedaan antara margin dan padding.
    Margin dan padding adalah dua konsep penting dalam desain CSS yang digunakan untuk mengatur tata letak dan ruang di sekitar elemen HTML. perbedaan utama ynag terdapat pada margin dan padding adalah:

    Margin:
    - Margin adalah jarak antara batas luar (border) dari elemen dengan elemen-elemen di sekitarnya.
    - Margin tidak memiliki warna atau latar belakang, dan secara khusus memengaruhi tata letak elemen dalam hal jarak. Margin tidak mempengaruhi tampilan elemen itu sendiri, hanya mengatur ruang di sekitarnya.

    Padding:
    - padding adalah jarak antara batas dalam (border) dari elemen dengan kontennya sendiri.
    - padding, dapat memiliki warna dan latar belakang, sehingga dapat memengaruhi tampilan elemen tersebut.

4. Jelaskan perbedaan antara framework CSS Tailwind dan Bootstrap. Kapan sebaiknya kita menggunakan Bootstrap daripada Tailwind, dan sebaliknya?
    Tailwind CSS dan Bootstrap adalah dua framework CSS yang berbeda dalam pendekatan desainnya. Bootstrap menyediakan komponen UI yang telah dirancang dengan baik, siap pakai, dan mempromosikan penggunaan kelas-kelas CSS yang telah ditentukan. Sebaliknya, Tailwind memberi pengembang kendali tinggi dengan memungkinkan mereka membuat desain kustom dengan cara menggabungkan kelas-kelas kecil dalam HTML.

    Penggunaan Bootstrap lebih baik digunakan jika membutuhkan pengembangan yang cepat dan konsistensi dalam tampilan, Sedangkan Tailwind cocok untuk digunakan ketika menginginkan fleksibilitas dan kontrol yang tinggi terhadap tampilan elemen.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
    - pada langkah awal saya menambahkan Bootstrap CSS dan juga JS pada html di root folder sebagai base html.
    - membuat tampilan navigation bar (navbar) dalam web menggunakan atribut dan kelas dari Bootstrap.
    - setelah itu saya membuat fungsi edit product dan delete product pada views.py kemudian menghubungkan nya ke path urls untuk mengakses fungsi yang dibuat. Lalu membuat tampilan html untuk edit product.
    - kemudian membuat tombol edit dan delete product di main.html
    - setelah itu saya membuat kustomisasi pada halaman login, register, edit product, dan create product dengan menambahkan beberapa elemen CSS pada template html, sehingga laman login, register, dan lainnya terlihat lebih menarik dan berwarna.