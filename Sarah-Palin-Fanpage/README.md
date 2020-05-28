# Sarah Palin Fanpage - 35 points
## Description
Are you a true fan of Alaska's most famous governor? Visit the [Sarah Palin fanpage](http://sarah_palin_fanpage.tjctf.org/).
## Flag
```
tjctf{wkDd2Pi4rxiRaM5lOcLo979rru8MFqVHKdTqPBm4k3iQd8n0sWbBkOfuq9vDTGN9suZgYlH3jq6QTp3tG3EYapzsTHL7ycqRTP5Qf6rQSB33DcQaaqwQhpbuqPBm4k3iQd8n0sWbBkOf}
```
## Solution
![](cookies.png)

Dalam situs ini terdapat suatu `cookie` yang bernama `data` dengan value yang sedikit membuat saya tertarik. Saya putuskan untuk mencoba menerjemahkannya ke dalam text biasa (base64 to text) dan ternyata menghasilkan suatu susunan kata petunjuk untuk menemukan flag.
```
{"1":false,"2":false,"3":false,"4":false,"5":false,"6":false,"7":false,"8":false,"9":false,"10":false}
```
Ubah menjadi
```
{"1":true,"2":true,"3":true,"4":true,"5":true,"6":true,"7":true,"8":true,"9":true,"10":true}
```
Kembalikan ke bentuk base64 dan ubah cookienya.

![](sarah.png)

Buka VIP area dan kita temukan flag nya.
