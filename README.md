# Tugas4-CloudComputing

Tugas – Cloud Run

Manfaatkanlah cloud run untuk melakuakn deployment terhadap suatu aplikasi web (bebas ambil dari mana). Dengan ketentuan sebagai berikut:
  - Minimal membuat dua cloud run berbeda
  - Masing-masing dihubungkan ke cloud build untuk menginplementasikan continuous deployment
  - Setiap aplikasi yang dideploy di cloud run disimpan pada satu repository yang sama namun branch berbeda
  - Tidak ada error yang tampil
  - Cpu allocation: only allocated during request processing (mengganti ini akan mengakibatkan tagihan yang tidak diperlukan pada tugas ini)
  - Didokumentasikan dengan terperinci (tidak hanya gambar, namun diberi penjelasan)

Contoh proyek untuk memenuhi kebutuhan tugas:

Sebuah aplikasi sedang dikembangkan dengan gencar dan sudah memiliki pengguna aktif. Tim pengembang membagi source code menjadi tiga branch dengan nama ‘production’, ‘testing’, dan ‘deployment’ yang merepresentasikan state pada code saat itu. Alasan tim pengembang membaginya menjadi tiga branch yaitu karena pengembangan dilakukan pada aplikasi yang sedang berjalan. Sehingga perlu dibedakan antara satu environment dengan environment yang lain agar tidak mengganggu pengguna dan meminimalisir bug pada aplikasi yang sudah berjalan akibat perubahan terbaru. Aplikasi dihubungkan dengan cloud build dengan trigger yaitu push pada masing-masing branch. Setiap environment dideploy menggunakan cloud run. Sehingga ada 3 cloud run yang berjalan dan ketiganya memiliki state berbeda dan pengguna berbeda. Development untuk tim Dev, testing untuk tim Quality Control, dan production untuk end user.
