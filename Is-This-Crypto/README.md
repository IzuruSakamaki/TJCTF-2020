# Is This Crypto? - 50 points
## Description
[Is this crypto?](https://static.tjctf.org/e141851decd4f7afab034c7055db229bd54011d2860ebd622302088fd4e062ae_file.txt)
## Flag
```
tjctf{ch0p1n_fl4gs}
```
## Solution
![](img.png)

Setelah mengunduh gambar, dapat dilihat gambar tersebut adalah meme dengan not balok Chopins Third Ballade. Dari soal dapat diketahui yang dicari adalah pembuat dari meme tersebut. Untuk mendapatkan data tersebut dapat menggunakan `exiftool` dan grep pada `terminal`. 
```
$ exiftool [imagename].png | grep Artist
```
