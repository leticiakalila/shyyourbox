1. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial). 
    - tahap pertama saya membuat repositroy baru terlebih dahulu dan menghubungkannya dengan direktori lokal
    - tahap kedua saya menginstlasi django dengan membuat file requirements, dan mengaktifkan env
    - tahap ketiga saya menambahkan aplikasi main pada direktori yang telah saya buat sebelumnya dan menambahkan main dalam INSTALLED_APPS.
    - tahap keempat saya membuat berkas HTML sebagai struktur dan tampilan konten pada halaman web.
    - tahap kelima saya menambahkan file urls.py untuk mengatur rute URL spesifik untuk fitur-fitur dalam aplikasi tersebut
    - tahap keenam saya men - set up model di models.py
    - tahap ketujuh saya menambahkan fungsi show main untuk aplikasi main
    - setelah selesai saya melakukan git add, commit, push ke repositori github dan melakukan deployment ke adaptable


2. Buatlah bagan yang berisi request client ke web aplikasi berbasis Django beserta responnya dan jelaskan pada bagan tersebut kaitan antara urls.py, views.py, models.py, dan berkas html.
    - ada pada berkas jawaban nomor 2

3. Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?
    Dalam menggunakan lingkungan virtual membantu kita dalam menjaga isolasi antara proyek-proyek yang berbeda dan mencegah pencampuran dependensi yang digunakan oleh proyek tertentu dengan yang lain. Meskipun memungkinkan untuk membuat aplikasi web berbasis Django tanpa lingkungan virtual, melakukannya akan menimbulkan risiko karena kurangnya isolasi antara proyek-proyek tersebut. Selain menjaga isolasi antar proyek, virtual environment juga memudahkan pembaruan pada proyek dan lebih mudah diuji.

4. Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.
    - MVC, yang merupakan singkatan dari Model-View-Controller, adalah sebuah arsitektur yang membagi aplikasi menjadi tiga komponen utama: model, view, dan controller. Hal ini membantu memisahkan peran dan tanggung jawab masing-masing komponen, dan memungkinkan pengembang untuk bekerja secara terpisah pada bagian-bagian yang berbeda dari aplikasi tanpa perlu merusak fungsionalitas keseluruhan.
    - MVT, yang merupakan singkatan dari Model-View-Template, adalah konsep arsitektur yang digunakan dalam pengembangan web untuk memisahkan komponen-komponen utama dari sebuah aplikasi. Konsep ini memungkinkan pengembang web untuk mengorganisasi dan mengelola kode dengan lebih terstruktur.
    - MVVM, yang merupakan singkatan dari Model-View-ViewModel, adalah pemisahan yang jelas antara tampilan (View) dan logika (ViewModel). Ini memungkinkan pengembang untuk bekerja secara terpisah pada tampilan dan logika.