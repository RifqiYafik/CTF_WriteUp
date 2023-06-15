# Monkey

## About Challenge

![Monkey](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/7cbad361-0937-49e0-8bd8-009d31db7ab2)

Terdapat sebuah [Link](http://103.167.136.89:10002/) yang mengarahkan ke website dan menampilakan seperti gambar dibawah 
![4](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/e16df8cc-50cc-481b-b3e5-217f5d281b63)


## Solution
Terdapat Halaman login dengan inputan Username dan Password. Terdapat Hint yaitu "Do you know if it is possible to post an array in PHP? I use MongoDB btw".
Kemudian saya mencari beberapa referensi dari berbagai sumber dan menemukan cara untuk melakukan enumerasi dengan [skrip](nosqli-user-pass-enum.py) nosql atau yang disebut MongoDB. 
