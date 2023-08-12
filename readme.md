# Pendahuluan

Setelah Channel WPU menayangkan video tutorial reactJS Episode 4 dengan studi kasus membuat aplikasi catatan-belanja, saya merasa tertantang untuk mengconvert codingan react WPU catatan-belanja menjadi versi AlpineJS. Alasan saya merasa tertantang karena sebelumnya saya sudah menyelesaikan tutorial AlpineJS di youtube dengan durasi 4jam-an di channel [https://www.youtube.com/@TheCodeholic](https://www.youtube.com/watch?v=5ILDMMLgX0E&t=703s&pp=ygUSYWxwaW5lanMgY29kZWhvbGlj).
Karena projek ini hanya latihan, jadi saya instalasi tailwindCSS & AlpineJS hanya lewat CDN.

# Tantangan

1. Karena pak Dhika tidak menyediakan desain versi mobile (responsif), maka convert CSS juga menjadi tantangan tersendiri bagi saya. Proses convert CSS tidak menggunakan murni CSS seperti yang dilakukan pak Dhika, tapi saya menggunakan TailwindCSS agar sedikit keren, hehe.
1. Walaupun alpineJS dan ReactJS sama-sama menawarkan reactivity, namun keduanya memiliki konsep yang berbeda dalam memanipulasi data. Pada react, manipulasi data harus menggunakan method immutable, sedangkan AlpineJS tidak. Sehingga ada perbedaan codingan pada CRUD aplikasi.
1. x-if pada AlpineJS tidak fleksible. Saat saya punya kondisi lebih dari satu, maka x-if harus ditulis manual berualang kali dengan kondisinya, dalam artian tidak bisa menggunakan elseif.
1. Tantangan terbesar adalah saat coding sorting. Pada react, kondisi pada switch akan terus dijalankan ketika react re-render. Pada AlpineJS, Alpine tidak melakukan re-render, sehingga membuat saya kebingungan mengatasinya. Saya tahu ada x-effect dan $watch yang fungsinya relevan dengan permasalahan ini, tapi saya kurang paham penggunaannya dan bagaimana codingan baiknya. Tapi untungnya, setelah bereksperiment dengan banyak kesalahan, saya menemukan solusinya.

# Teknologi yang digunakan

1. AlpineJS
2. TailwindCSS

# Demo

Demo: [https://belanjaan.sampurasun.my.id/](https://belanjaan.sampurasun.my.id/)

# Terima Kasih
