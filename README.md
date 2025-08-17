# GymFitAnalytics
Analisis Pola Latihan Anggota Gym Menggunakan model IBM granite
# Analisis Pola Latihan dan Kinerja Anggota Gym

## Tinjauan Proyek (Project Overview)
Proyek ini bertujuan untuk menganalisis dataset latihan anggota gym untuk mengidentifikasi pola, tren, dan perbedaan kinerja antara anggota dengan tingkat pengalaman yang berbeda (pemula, menengah, dan ahli). Dengan memahami bagaimana preferensi latihan dan efisiensi pembakaran kalori berubah seiring dengan meningkatnya pengalaman, pengelola gym dapat memperoleh wawasan berharga untuk menciptakan program yang lebih personal, meningkatkan retensi anggota, dan mengembangkan strategi bisnis yang lebih efektif. Analisis ini dilakukan sepenuhnya menggunakan Python di Google Colab dan didukung oleh Large Language Model (LLM) untuk menghasilkan insight strategis.

## Link Dataset Mentah (Raw Dataset Link)
Dataset yang digunakan dalam analisis ini adalah "Gym Members Exercise Dataset" yang tersedia secara publik.
* **Sumber:** [Gym Members Exercise Dataset on Kaggle](https://www.kaggle.com/datasets/valakhorasani/gym-members-exercise-dataset?resource=download)

---

## Insight & Temuan (Insight & Findings)
Berdasarkan analisis data yang didukung oleh AI, ditemukan beberapa wawasan utama:

**Insight 1:** Menciptakan Produk Latihan Premium Berbasis Efisiensi Waktu.
**Penjelasan Logis:** Data dengan jelas menunjukkan bahwa anggota berpengalaman (ahli) mencapai hasil pembakaran kalori yang lebih superior dalam durasi waktu yang sama atau bahkan lebih singkat, terutama pada latihan HIIT. Ini adalah nilai jual yang sangat kuat untuk segmen pasar yang memiliki waktu terbatas tetapi rela membayar lebih untuk hasil maksimal, seperti para profesional atau eksekutif. Gym dapat merancang program khusus 45 menit yang berfokus pada teknik HIIT dan Strength tingkat lanjut.

**Insight 2:** Mengembangkan "Jalur Pengembangan Anggota" (Member Journey Path) untuk Meningkatkan Retensi.
**Penjelasan Logis:** Adanya pergeseran fokus dari "durasi" ke "intensitas" seiring bertambahnya pengalaman menunjukkan sebuah pola kematangan anggota. Gym dapat memetakan perjalanan ini dan secara proaktif membimbing anggota. Sebagai contoh, seorang anggota yang telah aktif selama 3-4 bulan dan mayoritas melakukan kardio dapat secara otomatis ditawari sesi percobaan gratis untuk kelas "Pengenalan HIIT". Pendekatan ini membantu anggota menghindari stagnasi dan mencapai hasil lebih baik, yang pada akhirnya meningkatkan loyalitas dan retensi.

---

## Penjelasan Dukungan AI (AI Support Explanation)
* **AI Tool:** IBM Granite (`ibm-granite/granite-3.3-8b-instruct`)
* **Platform:** Model AI di-download dan dijalankan secara lokal di dalam environment Google Colab menggunakan pustaka `transformers` dari Hugging Face.
* **Cara Penggunaan:** Peran utama AI dalam proyek ini adalah sebagai alat untuk **Generasi Insight (Insight Generation)**. Setelah analisis kuantitatif selesai (pembuatan metrik dan visualisasi), temuan-temuan kunci dari analisis tersebut dirangkum menjadi sebuah *prompt* teks. Prompt ini kemudian diberikan kepada model AI yang sudah dimuat. LLM bertugas untuk melakukan **summarization** dan **reasoning**, yaitu mengubah rangkuman fakta statistik menjadi insight bisnis yang strategis dan naratif, lengkap dengan penjelasan logis di baliknya.
