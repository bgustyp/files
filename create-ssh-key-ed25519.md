### Cara Membuat SSH Key ed25519 untuk Windows
1. Masuk cmd/powershell 
2. Lalu ketikan ssh-keygen -t ed25519 -C "user@mail.com"

```console
user@pc:~$ ssh-keygen -t ed25519 -C "user@mail.com"
Generating public/private ed25519 key pair.
Enter file in which to save the key (.ssh/id_ed25519):
```
3. Jika muncul seperti di atas lalu enter, lalu akan muncul pembuatan password untuk SSH Key yang akan di buat. (Jika tidak ingin menggunakan password tekan enter saja)
```console
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
```
4. Setelah itu akan muncul seperti di bawah
```console
Your identification has been saved in id_ed25519
Your public key has been saved in id_ed25519.pub.
The key fingerprint is:
SHA256:aXwULd8ZL+fbGidV/4pGH9fplAbZCabAUAT8fy4bYH8 user@mail.com
The key's randomart image is:
+--[ED25519 256]--+
|      .o*o..     |
|       . o...o.  |
|        . ooo.++o|
|       . + ..o+o=|
|        Soo   .+*|
|       ...o....*=|
|           +oE*o=|
|           .+o.B.|
|           o+ o. |
+----[SHA256]-----+
```
5. Selesai, hasil akan tersimpan di folder %USER% .ssh/
6. Setelah itu copy isi dari hasil file id_ed25519.pub bisa menggunakan notepad untuk membukanya.

NOTE: Jika ada masalah tidak bisa login dengan SSH Key coba cek file id_ed25519.pub lalu cek properti pastikan akses everyone tidak termasuk.
