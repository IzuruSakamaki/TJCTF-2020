# Login - 30 points
## Description
Could you login into this [very secure site](http://login.tjctf.org/)? Best of luck!
## Flag
```
tjctf{inevitable890898}
```
## Solution
![](idx.png)

Ketika kita buka `inspect element` pada halaman utama situs ini, kita akan mendapatkan suatu value yang disinyalir merupakan hasil hash dari md5. Kita coba buktikan dengan melakukan dekripsi menggunakan tool [MD5Online](https://www.md5online.org/md5-decrypt.html). Ternyata tebakan kita benar!

![](hashmd5.png)

Setelah mendapatkan hasil dekripsi, selanjutnya tinggal melakukan login dengan `admin` sebagai username dan `inevitable` sebagai password.

![](furagu.png)
 
 Akhirnya kita temukan flag nya.
