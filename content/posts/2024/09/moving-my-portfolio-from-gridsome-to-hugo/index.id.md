---
title: "Migrasi Portofolio dari Gridsome ke Hugo: Solusi yang Lebih Cepat dan Sederhana"
type: "posts"
summary: "Dalam artikel ini, saya berbagi pengalaman memindahkan portofolio dari Gridsome ke Hugo. Saya akan membahas kenapa Hugo lebih cepat, lebih mudah digunakan, dan bagaimana proses migrasinya berjalan lebih lancar."
date: 2024-09-13
draft: false
description: "In this article, I share my experience migrating my portfolio from Gridsome to Hugo. I'll explain why Hugo is faster, easier to use, and how the migration process went more smoothly."
categories: ["Career"]
tags: ["Websites", "Hugo", "Blowfish"]
heroStyle: background
showWordCount: true
showZenMode: true
showReadingTime : true

---

Halo 👋🏻, saya Utrodus Said Al Baqi, Seorang **Software Engineer** yang menguasai **Flutter** untuk pengembangan aplikasi lintas platform. 

Jika Anda pernah mengunjungi [utrodus.com](https://utrodus.com), mungkin Anda telah melihat beberapa perubahan besar. Baru-baru ini, saya memigrasikan situs portfolio saya dari **[Gridsome](https://gridsome.org/)** ke **[Hugo](https://gohugo.io/)**, sebuah keputusan yang didorong oleh kebutuhan praktis dan teknis.

Awalnya, situs saya dibangun menggunakan **Gridsome**, sebuah static site generator yang menggunakan Vue.js. Gridsome cukup membantu dalam menampilkan proyek-proyek saya, tetapi seiring bertambahnya portfolio dan keinginan saya untuk menambahkan fitur blog, semakin sulit untuk memelihara proyek ini. 

Di sini, saya akan menjelaskan mengapa saya memilih **Hugo**, bagaimana saya mengelola proses migrasi, dan mengapa Hugo menjadi solusi yang lebih baik bagi pengembang yang mencari performa, kesederhanaan, dan skalabilitas.

### Kenapa Berpindah dari Gridsome?

Gridsome adalah tools yang luar biasa untuk membangun situs statis, terutama jika Anda sudah familiar dengan ekosistem `Vue.js`. Namun, ketika saya memperluas situs portfolio saya untuk menambahkan blog, beberapa keterbatasan mulai muncul:

1. **Kompleksitas**: Pengelolaan konten menjadi semakin menantang, terutama ketika saya ingin membuat postingan blog. Arsitektur berbasis Vue membuat bahkan perubahan konten kecil sering kali membutuhkan modifikasi kode, yang seharusnya merupakan tugas sederhana.

2. **Performa**: Meskipun Gridsome cukup cepat, seiring dengan berkembangnya proyek, waktu build juga semakin lama. Saya membutuhkan static site generator yang dapat menangani skala konten yang lebih besar dengan kecepatan dan efisiensi yang lebih baik.

3. **Pemeliharaan**: Mengelola dependensi dan struktur Gridsome membutuhkan lebih banyak perhatian daripada yang saya bayangkan. Ini membuat saya mencari solusi yang lebih mudah untuk dikelola.

### Kenapa Hugo?

Setelah mengeksplorasi berbagai static site generator seperti **Jekyll**, **Gatsby**, dan **Hugo**, saya menemukan bahwa **Hugo** adalah pilihan terbaik untuk kebutuhan saya. Berikut alasannya:

1. **Kecepatan yang Tak Tertandingi**: **[Hugo](https://gohugo.io/)** dibangun dengan Go, yang membuatnya menjadi salah satu static site generator tercepat. Waktu build, bahkan dengan banyak halaman dan postingan blog, hampir instan.

2. **Pengelolaan Konten yang Sederhana**: Hugo menangani konten melalui file **Markdown** yang sederhana. Saya tidak perlu lagi berurusan dengan komponen Vue.js yang kompleks atau query GraphQL hanya untuk menulis sebuah postingan blog.

3. **Kemudahan Pemeliharaan**: Dengan Hugo, pemeliharaan jauh lebih mudah. Hugo tidak memiliki banyak dependensi, sehingga lebih mudah dikelola dalam jangka panjang.

4. **Tema Blowfish**: Saya menemukan tema **[Blowfish](https://blowfish.page/)** oleh [Nuno Coração](https://n9o.xyz/), yang sangat sesuai dengan kebutuhan saya. Desain minimalis dan fitur yang ramah pengembang membuatnya ideal untuk menampilkan portfolio dan mengelola konten blog.

### Proses Migrasi: Dari Gridsome ke Hugo

Migrasi portfolio saya dari Gridsome ke Hugo melibatkan beberapa langkah penting:

#### 1. **Migrasi Konten**:
   Hugo menggunakan organisasi konten berbasis folder. Ini berarti saya harus mengonversi konten yang sudah ada ke dalam file Markdown dan menambahkan **front matter** yang sesuai. Proses ini cukup sederhana dibandingkan dengan logika pengambilan data yang lebih kompleks di Gridsome.

#### 2. **Template dan Layout**:
   Sistem templating Hugo dibangun di atas **Go templates**, yang sederhana namun solid. Berbeda dengan komponen Vue di Gridsome, Hugo memungkinkan Anda untuk mengelola layout melalui file HTML biasa, menawarkan fleksibilitas lebih besar tanpa perlu mengelola dependensi JavaScript yang berat.

#### 3. **Deployment**:
   Saya menggunakan [**Netlify**](https://www.netlify.com/) untuk hosting, proses build dan deployment otomatis sangat mudah. Setiap kali saya push perubahan ke cabang utama, Hugo akan membangun situs dan Netlify menangani hostingnya.



### Kenapa Blowfish?

Tema **[Blowfish](https://blowfish.page/)** adalah faktor kunci dalam keputusan saya beralih ke Hugo. Tema ini menawarkan estetika yang bersih dan minimalis, yang menempatkan fokus pada konten tanpa gangguan yang tidak perlu. Inilah alasan mengapa Blowfish menonjol:

- **Kemudahan Kustomisasi**: Blowfish dirancang sangat ramah pengembang. Mudah dimodifikasi dan dikembangkan, memungkinkan saya menyesuaikan layout agar sesuai dengan kebutuhan portfolio saya.
- **Desain Responsif**: Tema ini sepenuhnya responsif, memastikan bahwa situs saya terlihat bagus di semua perangkat.
- **Pengelolaan Konten**: Dengan Hugo dan Blowfish, mengelola postingan blog semudah menulis file Markdown dan menempatkannya di direktori yang benar. Tidak perlu lagi repot dengan komponen Vue atau query GraphQL seperti di Gridsome.

Untuk instruksi lebih lanjut tentang cara menginstal dan mengonfigurasi tema Blowfish, Anda dapat melihat dokumentasi resminya di sini:  **[Panduan Instalasi Blowfish](https://blowfish.page/docs/installation/)**.

### Kesimpulan

Berpindah dari **[Gridsome](https://gridsome.org/)** ke **[Hugo](https://gohugo.io/)** benar-benar mengubah cara saya mengelola portfolio. Hugo lebih cepat, lebih mudah dikelola, dan menawarkan sistem manajemen konten yang sesuai dengan alur kerja saya.

Tema **[Blowfish](https://blowfish.page/)**, khususnya, membuat pembuatan portfolio dan blog yang bergaya dan profesional menjadi sangat mudah. Jika Anda mencari cara untuk menyederhanakan situs Anda, saya sangat merekomendasikan untuk mencoba Hugo dan Blowfish.

Saya sangat bersemangat untuk terus memperluas portfolio saya dan berbagi lebih banyak konten tanpa terbebani menjaga konfigurasi yang kompleks. Anda akan selalu dapat pembaruan terbaru di situs saya di [utrodus.com](https://utrodus.com).

Jika ingin melihat kode sumber portfolio saya:

***Built with Gridsome:***

{{< github repo="utrodus/utrodus.com-old" >}}

***Built with Hugo & Blowfish Theme:***

{{< github repo="utrodus/utrodus.com" >}}

---
