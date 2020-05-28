# Zipped Up - 70 points
## Description
My friend changed the password of his Minecraft account that I was using so that I would stop being so addicted. Now he wants me to work for the password and sent me this [zip file](https://static.tjctf.org/663d7cda5bde67bd38a8de1f07fb9fab9dd8dd0b75607bb459c899acb0ace980_0.zip). I tried unzipping the folder, but it just led to another zipped file. Can you find me the password so I can play Minecraft again?
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
