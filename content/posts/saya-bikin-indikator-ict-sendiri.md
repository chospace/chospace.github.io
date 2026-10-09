---
title: "Saya Ngerakit Indikator ICT Sendiri (dan Pelajarannya)"
date: 2026-10-09T22:05:00+07:00
tags: ["trading", "ict", "pine-script", "tradingview"]
author: "Cho"
summary: "Ceritanya saya pengen indikator ICT all-in-one. Jadinya ngerakit sendiri: gabungin konsep yang udah ada, tambahin engine buatan sendiri, dan belajar banyak di prosesnya."
showToc: true
TocOpen: false
draft: true
---

Udah lama saya pakai konsep ICT/SMC buat trading. Masalahnya, tiap mau analisa harus pasang indikator satu-satu: satu buat FVG, satu buat order block, satu buat liquidity. Chart jadi rame kayak pasar malam.

Kepikiran: kenapa nggak bikin satu indikator yang ngumpulin semuanya?

## Ngerakit, Bukan Nemuin

Jujur aja: saya nggak nemuin konsep baru. Konsep ICT-nya udah ada yang bikin bagus banget (LuxAlgo) — dan saya pakai logikanya dengan lisensi yang bener (CC BY-NC-SA, atribusi tetap dicantumkan).

Yang saya kerjain:

1. **Gabungin** modul-modul ICT (market structure, liquidity, order block, FVG, killzone, dll) jadi satu indikator dengan master toggle — 8 modul, bisa on/off satu-satu.
2. **Nambahin engine sendiri**: garis multi-timeframe high/low (PDH/PWH/PMH) — Previous Day/Week/Month High & Low yang auto-extend. Ini yang belum ada di versi aslinya dan paling sering saya pakai.
3. **Ngerapihin** biar enak dipakai harian.

Ditulis pakai Pine Script v5 di TradingView.

## Yang Saya Pelajari dari Kodenya

Ngerakit indikator ternyata cara belajar paling efektif. Beberapa hal yang baru bener-bener saya pahami setelah ngutak-atik kodenya:

- **Liquidity pool** itu bukan sekadar high/low terakhir. Kode yang bagus nyari *cluster* — 3 swing point atau lebih yang numpuk dalam margin ATR. Di situlah stop loss orang-orang ngumpul.
- **Order block yang jebol** nggak langsung hilang — dia berubah jadi *breaker*, alias zona flip support/resistance. Ini yang sering kelewat kalau cuma lihat chart manual.
- **FVG butuh filter displacement**. Tanpa filter, tiap gap kecil ke-detect dan chart jadi sampah. Syaratnya: body candle harus lebih gede dari rata-rata, wick-nya kecil. Simpel tapi ngaruh banget.
- **Killzone pakai jam New York** (Asia 20:00, London 02:00, dst). Standar ICT — dan bener, pergerakan paling "jujur" emang di jam-jam itu.

## Yang Paling Susah

Bagian tersulit bukan kodenya — tapi **nahan diri buat nggak overfitting**. Godaannya gede: "ah tambahin filter ini biar sinyalnya dikit tapi akurat."

Padahal indikator yang bagus itu yang jujur nunjukkin apa yang terjadi di chart, bukan yang sok akurat.

## Pelajaran Terbesar

Setelah ngerakit sendiri, saya jadi sadar: indikator itu cuma alat bantu visualisasi. Yang bikin profit bukan indikatornya, tapi **disiplin ngikutin plan dan ngelola risiko**.

Indikator secanggih apapun nggak bakal nolong trader yang entry tanpa stop loss.

---

*"Disiplin mengelola risiko, bukan mengejar profit."*

Indikatornya saya namain **AWSM ICT Concept**. Masih versi awal, bakal terus saya kembangin sambil dipakai trading harian.

Kalau kamu juga lagi belajar Pine Script atau ICT, tulis di komentar — kita belajar bareng.
