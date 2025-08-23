---
date: '2021-02-23T14:59:54+07:00'
draft: false
title: 'Cara web ini di buat!'
summary: "Kenapa bikin web ini? Gimana caranya? (Pstingan kedua ✌️)"
tags: ["tutorial", "hugo", "github"]
weight: 2
---

## Kenapa Bikin Web Ini?
Sebenarnya sih... **nggak ada alasan yang terlalu keren**. 😉
Cuma pengen punya tempat buat nulis sambat, random, dan kadang-kadang sok produktif.

---

## Stack yang Dipakai

- **[Hugo](https://gohugo.io/)** → Mesin roket buat bikin web statis. Super cepat!
- **[PaperMod](https://github.com/adityatelange/hugo-PaperMod)** → Baju minimalis buat web-nya. Clean dan gampang dioprek.
- **[Git](https://git-scm.com/)** → Mesin waktu buat ngelacak semua perubahan kode.
- **[GitHub Pages](https://pages.github.com/)** → Lahan gratis buat nerbitin web kita. Mantap!
- **PowerShell / Terminal** → Tongkat sihir buat ngasih perintah ke komputer.
- **VS Code** → Bengkel buat ngedit dan ngerakit semua filenya.

---

## Kenapa Hugo?
- **Ngebut parah!** Build situs cuma kedipan mata (detik, bukan menit).
- **Nulisnya santai.** Cuma pakai Markdown, kayak ngetik di Notepad.
- **Banyak "baju" gratis.** Temanya bejibun dan bisa dimodif sesuka hati.
- **Sekalian belajar ngoding ringan.** Punya web keren sambil ngasah skill? Kenapa enggak!

---

## Gimana Cara Bikinnya? (Versi Kilat ⚡)

Tertarik bikin juga? Tenang, nggak sesusah itu kok. Anggap aja lagi ngerakit Tamiya.

### **Persiapan Awal (Modal Wajib)**

1.  **Install Hugo:** Kunjungi [situs resminya](https://gohugo.io/installation/) dan ikuti petunjuk buat OS kamu.
2.  **Install Git:** Ini juga wajib. Ambil dari [website Git](https://git-scm.com/downloads/).
3.  **Punya Akun GitHub:** Kalau belum punya, daftar dulu. Gratis!

### **Langkah-langkah Ajaib**

1.  **Bikin "Kerangka" Situs:** Buka terminal, terus jalanin perintah ini:
    ```bash
    hugo new site nama-web-keren-kamu
    cd nama-web-keren-kamu
    ```

2.  **Pasang Tema (Biar Cakep):** Kita pakai PaperMod kayak web ini ya. Caranya gampang, tinggal "kloning" tema ke dalam folder web kamu.
    ```bash
    git init
    git submodule add [https://github.com/adityatelange/hugo-PaperMod.git](https://github.com/adityatelange/hugo-PaperMod.git) themes/PaperMod
    ```

3.  **Aktifin Temanya:** Buka file `hugo.toml` (atau `config.toml`) terus tambahin baris ini di paling bawah:
    ```toml
    theme = "PaperMod"
    ```
    Jangan lupa atur juga `baseURL` di file yang sama jadi alamat GitHub Pages kamu nanti (contoh: `"https://username.github.io/"`).

4.  **Bikin Postingan Pertama:** Waktunya nulis!
    ```bash
    hugo new content posts/postingan-pertamaku.md
    ```
    Sekarang buka file `.md` yang baru dibuat di folder `content/posts/` dan mulai tulis sesukamu. Jangan lupa ubah `draft: true` jadi `draft: false` kalau sudah siap tayang.

5.  **Terbangin ke GitHub! 🚀**
    * Buat repository baru di GitHub. Kasih nama `username.github.io` (ganti `username` dengan username GitHub kamu).
    * Kembali ke terminal, di dalam folder web kamu, jalanin perintah ini satu per satu:
    ```bash
    # Perintah buat ngerakit semua file jadi web statis
    hugo

    # Masuk ke folder public (hasil rakitan)
    cd public

    # Upload ke GitHub
    git init
    git add .
    git commit -m "Yeah! Website pertama gue live!"
    git branch -M main
    git remote add origin [https://github.com/username/username.github.io.git](https://github.com/username/username.github.io.git)
    git push -u origin main
    ```

**Voila!** Tunggu beberapa menit, dan coba akses `https://username.github.io`. Kalau semua lancar, website kamu udah mejeng di internet!

---

## Rencana ke Depan
- Nulis lebih rajin (semoga).