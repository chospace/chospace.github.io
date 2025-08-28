---
title: "Go & File: Cara Mudah Membaca dan Menulis File Teks"
date: 2019-03-28T22:22:41+07:00
# weight: 1
# aliases: ["/first"]
tags: ["golang"]
author: "Cho"
summary: "Catatan singkat dan praktis tentang cara membaca konten dari sebuah file dan menuliskannya ke file baru menggunakan Go (Golang)."
# author: ["Me", "You"] # multiple authors
showToc: false
TocOpen: false
draft: false
hidemeta: false
comments: false
#description: "Desc Text."
canonicalURL: "https://canonical.url/to/page"
disableHLJS: false # to disable highlightjs set true
disableShare: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
  image: "<image path/url>" # image path/url
  alt: "<alt text>" # alt text
  caption: "<text>" # display caption under cover
  relative: false # when using page bundles set this to true
  hidden: true # only hide on current single page
editPost:
  URL: "https://github.com/chospace/chospace.github.io/content"
  Text: "Suggest Changes" # edit text
  appendFilePath: true # to append file path to Edit link
---

Salah satu tugas paling umum dalam pemrograman adalah mengelola file. Entah itu membaca file konfigurasi, memproses data log, atau menyimpan hasil kerja, berinteraksi dengan file adalah *skill* dasar yang wajib dikuasai.

Di Go, tugas ini dibuat sangat sederhana dan lugas berkat *standard library* `os` dan `io/ioutil`.

Dalam catatan kali ini, kita akan belajar dua hal fundamental:
1.  **Membaca** seluruh konten dari sebuah file teks.
2.  **Menulis** data (string) ke sebuah file baru.

Mari kita mulai!

---

## 📖 Membaca File Teks

Anggap kita punya file bernama `catatan.txt` dengan isi sebagai berikut:

**catatan.txt**

Untuk membaca seluruh isi file ini, kita bisa menggunakan fungsi `os.ReadFile()`. Fungsi ini sangat praktis karena langsung mengembalikan seluruh konten file dalam bentuk `[]byte` (slice of bytes).

Berikut adalah kode lengkapnya:

**main.go**
```go
package main

import (
	"fmt"
	"os"
)

func main() {
	// Membaca file catatan.txt
	data, err := os.ReadFile("catatan.txt")
	if err != nil {
		// Jika file tidak ditemukan atau ada error lain, program akan berhenti
		fmt.Println("Error saat membaca file:", err)
		return
	}

	// 'data' adalah []byte, kita ubah menjadi string untuk ditampilkan
	fmt.Println("Isi file:")
	fmt.Println(string(data))
}