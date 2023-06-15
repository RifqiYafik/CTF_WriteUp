# Fortune Cookies
## About The Challenge

Pada challenge ini sudah terbaca bahwa flag terdapat pada cookies dari web yang diberikan

![Fortune Cookies](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/db546296-3ba3-48a5-8d19-ef0090b6b56a)

## Solution
Terdpat [link](http://103.167.136.89:10088/) yang ketika di klik maka akan menampilkan tampilan seperti dibawah ini
![1](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/0004867f-aaf0-4a82-a1e9-4b8f923125eb)

Ketika kita klik 'Get Your Fortune' terdapat respon dari web yang berubah ubah setiap kita menekannya
![2](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/cc52b2df-73a3-472d-a158-ec8537c069aa)

Disini saya langsung mencoba melihat coookiesnya dengan cookie editor dan mengganti valuenya menjadi 1 kemudian save dan refresh halaman webnya dan benar saja terdapat respon yang merupakan flagnya.
![3](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/cb5b41ea-9473-4e69-b078-3657fd110931)

## Flag
**ForestyHC{here_is_your_fortun3_cookie_4a0a47}**
