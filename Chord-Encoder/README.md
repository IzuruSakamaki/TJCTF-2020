# Chord Encoder - 40 points
## Description
I tried creating my own [chords](https://static.tjctf.org/67be5bd036a4be8323314d1da6ad2e673963f76634a62ec47d53fb07a04a3722_chords.txt), but my [encoded sheet music](https://static.tjctf.org/c29857b8d4d1b2dfe502b5053d73844a08358ae681b2af8de6829b765dc2c28e_notes.txt) is a little hard to read. Please play me my song!

[chord_encoder.py](https://static.tjctf.org/da36df431da358250884ff9765e8c0c5f054b845aff31b85e37229159176bb9f_chord_encoder.py)

## Flag
```
flag{zats_wot_1_call_a_meloD}
```
## Solution
Setelah mengunduh beberapa textfile dan kode python yang terlampir dalam soal, maka dapat langsung kita buka `chords.txt` dan `notes.txt`. Ubah semua data yang ada pada `notes.txt` sesuai dengan yang ada pada `chords.txt`. Lalu buka kode pythonnya.

![](img.png)

Saya tidak tahu apakah kode ini bekerja atau tidak, namun saya melihat sedikit logika berpikir dalam kode ini. Dapat dilihat pada gambar bahwa kita harus merubah seluruh huruf besar menjadi angka yang telah ditentukan pada kode python ini. Setelah huruf besar diubah menjadi sebuah angka, maka akan kita dapatkan hasil berupa hexadecimal. Ubahlah menjadi text dan kita akan menemukan flag nya.
