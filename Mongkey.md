# Monkey

## About Challenge

![Monkey](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/7cbad361-0937-49e0-8bd8-009d31db7ab2)

Terdapat sebuah [Link](http://103.167.136.89:10002/) yang mengarahkan ke website dan menampilakan seperti gambar dibawah 
![4](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/e16df8cc-50cc-481b-b3e5-217f5d281b63)


## Solution
Terdapat Halaman login dengan inputan Username dan Password. Terdapat Hint yaitu "*Do you know if it is possible to post an array in PHP? I use MongoDB btw*".
Kemudian saya mencari beberapa referensi dari berbagai sumber dan menemukan cara untuk melakukan enumerasi dengan [skrip](nosqli-user-pass-enum.py) nosql atau yang disebut MongoDB. 
Langsung saja saya coba jalankan pada vim di linux dengan comand seperti dibawah ini untuk melakukan enumerasi pada username.
```shell
python3 nosqli -u http://103.167.136.89:10002/ -up user -pp pass -ep user -op login:login -m POST
```
Setelah enumerasi selesai didapatkan 2 username pada website ini yaitu admin dan guest.

![11](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/0854bca7-ecb5-4ba9-8544-128e4b6ba80d)


Username sudah ditemukan, saya mencoba sekali lagi melakukan enumerasi pada pasword dengan comand dibawah ini
```shell
python3 nosqli -u http://103.167.136.89:10002/ -up user -pp pass -ep pass -op login:login -m POST
```
Tidak disangka Flag yang kita cari didapatkan pada saat melakukan enumerasi pada passwordnya.

![12](https://github.com/RifqiYafik/CTF_WriteUp/assets/136687984/81673266-6a79-46b0-b8be-fca08649006d)

## Flag
**ForestyHC{reject_humanity_return_to_monke_5543d8}**
