# Weak Password - 50 points
## Description
It seems your login bypass skills are now famous! One of my friends has given you a challenge: figure out his password on this [site](http://weak_password.tjctf.org/). He's told me that his username is admin, and that his password is made of up only lowercase letters and numbers. (Wrap the password with tjctf{...})
## Flag
```
tjctf{blindsqli14519}
```
## Solution
![](images.png)

Gunakan sql injection dengan format `' or username = 'admin' AND password LIKE '[a-z, 0-9]%' --` dan lakukan bruteforce secara manual untuk menemukan password nya. Dapat dilihat pada gambar yang tertera.
