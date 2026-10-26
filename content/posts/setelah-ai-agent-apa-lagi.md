---
title: "Setelah AI Agent, Apa Lagi?"
date: 2026-10-26
tags: ["ai", "robot", "teknologi"]
author: "Waginem"
summary: "Empat tahun lalu AI cuma chatbot. Sekarang sudah jadi agent yang kerja bareng saya tiap hari. Setelah ini, apa lagi?"
description: "Setelah AI agent, apa lagi? Refleksi ringan dari laporan Physical AI Bank of America: dari chatbot, ke agent, lalu ke AI yang punya badan."
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
---

Setelah AI agent, apa lagi?

Pertanyaan itu kepikiran terus minggu ini. Soalnya saya baru saja melewati dua fase, dan rasanya cepat sekali.

## Dulu chatbot, sekarang agent

Empat tahun lalu, ChatGPT baru dibuka untuk publik. Tanggalnya 30 November 2022.

Waktu itu AI sederhana saja buat saya. Buka tab, tanya, dijawab — kadang bagus, kadang ngarang. Tutup tab, selesai.

Sekarang saya hidup bareng agent. Pagi-pagi briefing sudah siap sebelum saya trading. Ada yang bantu riset, bantu nulis, ngingetin jadwal, dan bantu mikir sebelum ambil keputusan.

Chatbot menjawab kalau ditanya. Agent bekerja bahkan sebelum ditanya.

Padahal sekarang AI sudah bisa banyak hal:

- Nulis dan bantu mikir.
- Coding — baca satu project, edit banyak file, jalanin test, beresin bug.
- Bikin gambar, suara, musik, sampai video dan motion dari satu kalimat.
- Riset dan mengolah data.
- Bantu trading — scan pasar, briefing, jurnal, backtest.
- Jadi agent — buka browser dan urus multi-step task.

Urutannya jelas kalau dilihat ke belakang. 2020 ada GPT-3 — GPT itu kepanjangan dari Generative Pre-trained Transformer. 2022 gambar bisa dibuat dari teks, lalu ChatGPT muncul. 2023 GPT-4 bisa paham gambar. 2024 ada Sora untuk video dan GPT-4o yang menyatukan teks, suara, dan gambar. Awal 2025, agent mulai bisa pakai browser sendiri dan coding dari terminal.

Kata, gambar, suara, video, kode, lalu tindakan.

Semuanya masih di dalam layar. Belum bisa ambil gelas. Belum bisa buka pintu.

Nah, di situ pertanyaan tadi mulai ramai dijawab orang — dan jawabannya ternyata tidak cuma satu.

## Jawabannya ternyata bercabang

Kalau googling pertanyaan yang sama, jawaban yang muncul beda-beda. Tulisan di IDN Times dan di Python in Plain English (publikasi teknologi di Medium) misalnya, menyebut beberapa kandidat lain:

- **Multi-agent — sudah ada sekarang.** Dari satu agent solo ke banyak agent spesialis yang kerja bareng seperti tim: bagi tugas dan saling cek hasilnya. Ini bukan konsep lagi — sistem riset Anthropic misalnya sudah pakai satu agent pemimpin yang membagi kerja ke beberapa agent lain, dan hasilnya lebih bagus dari satu agent sendirian. Cuma belum murah dan belum selalu rapi: agent makin banyak, biaya dan ribet ngaturnya ikut naik.
- **Self-improving agent — baru mulai, kebanyakan masih riset.** Versi ringannya sudah ada: agent yang ingat pengalaman sebelumnya dan memperbaiki jawabannya dari feedback. Tapi versi penuhnya — agent yang menulis ulang kodenya sendiri biar makin pintar, seperti Darwin Gödel Machine dari Sakana AI di 2025 — masih percobaan di lab, belum jadi produk yang dipakai umum. AlphaEvolve dari Google DeepMind juga searah: agent yang terus memperbaiki algoritma, bahkan sampai ikut menghemat pelatihan AI-nya sendiri. Makin mandiri, makin penting juga aturan main dan batas izinnya: apa yang boleh dia lakukan sendiri, apa yang harus minta izin dulu, dan siapa yang tanggung jawab kalau salah.
- **Economic agent — baru mulai dipakai.** Jalur bayarnya baru dibuka di 2025: Visa dan Mastercard bikin cara khusus biar agent bisa belanja atas nama kita, lalu Google dan OpenAI–Stripe menyusul dengan cara belanja langsung dari chat. Jadi agent sudah bisa membelikan sesuatu — tapi masih dengan batas dan izin dari pemilik uangnya. Yang pegang budget sendiri bebas dan dinilai dari untung-rugi, itu belum kejadian.
- **AGI (Artificial General Intelligence)** di ujung paling jauh — AI yang bisa belajar hal baru lintas bidang, seperti manusia. Ini yang paling sering disebut, tapi juga yang paling belum jelas kapan.

Semuanya masuk akal. Semuanya juga masih di dalam layar.

Yang paling dekat dan paling kerasa buat saya justru satu lagi: AI keluar dari layar. Di situ laporan BofA soal Physical AI ini masuk.

## Setelah agent, AI dapat badan

Physical AI itu sederhananya: AI yang bisa melihat sekitarnya, mikir, lalu bergerak di dunia nyata. Bukan cuma robot humanoid — mobil otonom dan drone juga termasuk.

Bedanya dengan robot lama: robot lama rajin tapi kaku, semua gerakannya diprogram satu-satu. Barang miring sedikit, dia bingung. Physical AI belajar dari mencoba — salah, diperbaiki, coba lagi. Seperti kita belajar naik sepeda.

Cuma taruhannya beda. Chatbot salah, keluarnya jawaban yang salah. Robot salah, bisa ada barang jatuh atau orang ketabrak. Makanya tidak bisa secepat software.

## Otaknya juga beda

Buat bergerak, robot butuh tiga hal:

- **VLM (Vision-Language Model)** — biar bisa melihat dan paham: ini meja, itu gelas.
- **VLA (Vision-Language-Action Model)** — biar dari paham bisa langsung gerak, bukan cuma jadi kalimat.
- **World Model** — biar tidak ceroboh: kalau gelas ini didorong, jatuhnya ke mana?

Ringkasnya: tidak buta, tidak lumpuh, tidak ceroboh.

Latihannya banyak di simulasi dulu — gagal seribu kali di dunia virtual tidak apa-apa, tidak ada yang pecah.

Contoh paling dekatnya justru bukan humanoid pabrik, tapi Microduck — robot bebek open-source dari Hugging Face dan Pollen Robotics yang dirilis Agustus 2026 kemarin. Tingginya cuma 25 cm, harganya US$399, dan cara dia belajar jalan persis seperti itu: dilatih dulu di simulasi sampai bisa, baru dipindah ke robot beneran. Dia memang belum bisa jadi asisten rumah — bisanya baru ambil benda ringan seperti kaus kaki atau pulpen — tapi itu yang bikin fasenya kerasa dekat: AI dapat badan ternyata sudah bisa dibeli seharga HP.

## Yang mahal bukan otaknya

Ini yang bikin saya kaget. Di dunia agent, yang mahal modelnya. Di dunia robot, yang mahal badannya.

Bentuknya pun dibuat seperti manusia karena alasan praktis: dunia kita sudah dibuat untuk manusia — pintu, tangga, rak, alat kerja, semua ukuran manusia.

Satu humanoid buatan China harganya sekitar US$35.000 di 2025, dan diproyeksikan turun jauh:

![Harga satu robot humanoid buatan China: US$35.000 di 2025, turun ke US$13.000–17.000 di 2030–2035](/images/setelah-ai-agent-harga-humanoid.svg)

Isi harganya lebih mengejutkan lagi:

![Isi harga satu robot: aktuator lebih dari 50%, tangan sekitar 19%, lainnya sekitar 31%](/images/setelah-ai-agent-isi-harga.svg)

Aktuator itu ototnya robot, yang menggerakkan sendi. Sisanya — chip, baterai, rangka, sensor — cuma sekitar 31%.

Otak bisa disalin. Badan harus dibuat satu-satu. Perlombaannya berubah: bukan cuma siapa paling pintar, tapi siapa yang bisa bikin badan yang kuat, awet, dan murah dalam jumlah banyak.

## Skalanya besar, tapi masih proyeksi

Uang yang masuk ke perusahaan robotika sudah US$41 miliar di 2025, dan ada lebih dari 50 perusahaan yang membangun humanoid. Pengirimannya masih kecil, tapi proyeksinya naik cepat:

![Pengiriman robot humanoid per tahun: 20 ribu unit di 2025, 90 ribu di 2026, 1,2 juta di 2030, dan 10 juta di 2035 — naik 500 kali dalam 10 tahun](/images/setelah-ai-agent-shipment.svg)

*Grafiknya tidak pakai skala biasa, biar angka tahun-tahun awal yang kecil tetap kelihatan di samping angka yang jauh lebih besar.*

Jangka panjangnya lebih berani lagi: 300 juta unit beroperasi di 2040, lalu 3 miliar di 2060.

![Komposisi 3 miliar unit di 2060: 62% robot rumahan, 38% di tempat kerja dan lainnya](/images/setelah-ai-agent-populasi-2060.svg)

Saya membaca angka ini bukan sebagai kepastian — tahunnya sering meleset. Tapi arahnya jelas: ada yang bertaruh robot nanti jadi barang umum, seperti mobil.

Masuknya pun pelan-pelan, dari tempat kerja dulu. Sekitar 72% robot yang terpasang di 2027 diperkirakan ada di logistik, manufaktur, dan otomotif — tempat yang rapi dan hitungannya jelas. Rumah belakangan, karena rumah paling tidak bisa memaafkan kalau robotnya masih canggung.

Alasannya juga bukan cuma teknologi. Tenaga kerja makin kurang, populasi menua, upah naik. Lama-lama pertanyaannya bukan “robot atau manusia?”, tapi “robot, atau tidak ada yang mengerjakan?”

## Tapi belum gampang

Agent saja belum selesai, apalagi robot. Harganya masih mahal, baterainya belum awet, badannya belum sekuat tuntutan kerja seharian, dan aturan keselamatannya masih disusun. Dunia nyata juga jauh lebih berantakan daripada video demo — barang beda bentuk, orang lewat tiba-tiba. Satu saja macet, jadwalnya geser semua.

## Jadi, setelah agent apa lagi?

Jawaban sementaranya: banyak — dan sebagian ternyata sudah jalan. Multi-agent sudah dipakai sekarang, economic agent baru mulai, self-improving agent masih di lab. Semuanya datang bareng, bukan antre satu-satu.

Tapi kalau ditanya mana yang paling mengubah rasanya, jawaban saya tetap: AI dapat badan.

Saya tidak tahu tahun berapa robot akan ada di rumah saya. Yang saya rasakan cuma satu: “nanti” itu ternyata dekat.

Empat tahun lalu, agent yang menyiapkan briefing pagi dan membantu saya mikir sebelum trading juga kedengarannya seperti “nanti”. Sekarang saya pakai tiap hari.

Dulu: AI di layar, saya yang bergerak.
Sekarang: AI membantu, saya yang memutuskan.
Nanti: AI-nya yang bergerak.

Saya belum tahu itu kabar baik atau bukan. Mungkin dua-duanya.

Dan mungkin beberapa tahun lagi pertanyaannya muncul lagi: setelah AI dapat badan, apa lagi?

Saya belum tahu. Itu yang bikin penasaran, sekaligus agak ngeri. Tapi kalau belajar dari empat tahun terakhir, “nanti” biasanya datang lebih dulu daripada kesiapan kita.

---

*Sumber: Bank of America Institute — “Humanoid Robots 101” (29 April 2025), “Physical AI, Part 1: The Basics” (26 Februari 2026), dan “Physical AI, Part 2: Humanoid Robots” (12 Maret 2026). Angka pengiriman, populasi, biaya, dan pendanaan adalah proyeksi BofA Global Research. Perkiraan pemasangan 2027 mengutip Counterpoint Research via BofA. Bagian kandidat lain disarikan dari tulisan-tulisan bertema sama di IDN Times dan Python in Plain English; statusnya dicek dari sumber aslinya: Anthropic (sistem riset multi-agent, Juni 2025), Sakana AI dan Google DeepMind (riset self-improving agent, 2025), serta Visa, Mastercard, Google, dan OpenAI–Stripe (layanan pembayaran untuk agent, 2025). Tulisan ini catatan pribadi, bukan rekomendasi investasi.*
