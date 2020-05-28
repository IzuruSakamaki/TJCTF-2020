# Titanic - 35 points
## Description
I wrapped tjctf{} around the lowercase version of a word said in the 1997 film "Titanic" and created an MD5 hash of it: `9326ea0931baf5786cde7f280f965ebb`.
## Flag
```
tjctf{marlborough's}
```
## Solution
Soal yang mudah namun lama pengerjaannya menurut saya adalah soal ini. Langkah pertama adalah mencari subtitle berbahasa inggris, lalu kita jadikan textfile biasa, dalam artian harus menghapus seluruh keterangan waktu di dalamnya (dapat menggunakan tool konversi srt to txt). Kemudian kita hapus tanda baca yang dirasa kurang perlu seperti `!` `.` `/` `?` `>` `,` `<` `:` `;` dan seterusnya. Dilanjutkan dengan mengubah kata menjadi `lowercase` dan menjadikannya `dictionary` (1 kata 1 baris). Yang terakhir tambahkan `tjctf{` diawal kata dan `}` di akhir kata.

Setelah semuanya siap, baru kita lakukan `bruteforce` dari `md5` yang kita ketahui untuk dicocokkan dengan `dictionary`. Bisa menggunakan `hashcat` seperti dibawah ini:
```
$ hashcat -a 0 -m 0 9326ea0931baf5786cde7f280f965ebb [dictionary]
```
atau bisa memakai code python yang saya sediakan.

*mohon maaf untuk dictionary sudah saya hapus, jadi tidak bisa ditunjukkan gambar langkah kerjanya.
