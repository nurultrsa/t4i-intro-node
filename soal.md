SOAL 1
1. Mohon jelaskan apa itu Node.js? Apa perbedannya dengan JavaScript?
2. Mohon jelaskan arsitektur dari Node.js?
3. Apa perbedaan antara Built-in Module, External Module, dan Custom Module pada Node.js?
4. Sebutkan salah satu contoh dari Built-in Module, External Module, dan Custom Module pada Node.js?

JAWABAN
1. Node.js adalah open source, cross-platform runtime environment dan library yang digunakan untuk menjalankan aplikasi web di luar browser klien. Node digunakan untuk pemrograman di sisi server, terutama digunakan untuk non-blocking, event-driven, seperti situs web tradisional dan layanan API back-end. Setiap browser memiliki versi mesin JS-nya sendiri, dan node.js dibuat pada Javascript V8E Google Chrome. Dengan node situs dapat dijalankan menggunakan ‘stack’ tersusun, yang membuat pengembangan dan pemeliharaan menjadi cepat dan mudah, memungkinkan developer untuk fokus memenuhi tujuan proyek. Perbedaannya dengan javascript adalah bentuknya lalu dari fleksibilitas, kegunaan, perbedaan framework, dan kapabilitas tambahan. Javascript adalah bahasa pemrograman yang digunakan untuk membuat script website, yang berarti tujuannya dalam front-end, kebalikan dengan node yang digunakan untuk sisi back-end (server) dan bisa digunakan di luar browser. 
2. Node.js node mengikuti model Single Threaded Event Loop. Model pemrosesannya didasarkan pada model berbasis event Javascript dengan mekanisme callback. Karena node.js mengikuti arsitektur ini, node dapat menangani banyak permintaan klien secara bersamaan dengan mudah. Dimulai dari klien mengirimkan permintaan ke web server, kemudian semua permintaan diterima secara Single Thread dan node secara internal mengatur eksekusi proses ke dalam queue secara berulang (fase Event Loop terjadi): permintaan 1 klien 1, permintaan 2 klien 2, dst. Jika tidak ada permintaan node akan terus menunggu. 
3. Built-in module adalah modul yang sudah terpasang dan selalu tersedia sehingga tidak perlu dilakukan secara terpisah. Karena merupakan bagian dari inti node.js, modul selalu dimantain dan developer tidak perlu khawatir dengan update terbarunya. External module yang merupakan NPM Packages memiliki dependensi terpisah, dilacak di dalam package.json, dan kodenya tidak diperiksa ke dalam version control. Yang terakhir, custom module atau bisa disebut juga local module, yaitu modul yang ditulis sendiri, merupakan bagian dari codebase dan perlu diperiksa ke dalam version control. Inti dari custom modul adalah menggunakan ulang kode di dalam proyek. Contohnya membuat file/utility, code bisa diekspor dari file tersebut  dan digunakan di bagian berbeda dari aplikasi.
4. Contoh dari built in module = http, stream, fs, querystring, dll. Contoh dari external module = moment, nodemon. Contoh dari costume module = fungsi sendiri, seperti :
exports.skilvul = function () {
return "Hello Nurul!";
};
export kemudian import ke main file.
