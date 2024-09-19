1.	Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file baru.
![1](https://github.com/user-attachments/assets/e36244fe-826e-4cc7-be5f-4d892be6098d)

Penjelasan: Perintah ls -la digunakan untuk menampilkan daftar file secara lengkap di direktori aktif (dengan format long listing). Output dari perintah ini dialihkan (redirect) ke file baru bernama file_baru.txt menggunakan >.

2.	Lihat daftar secara lengkap pada direktori /etc/passwd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.
![2](https://github.com/user-attachments/assets/dbaa0ce3-c257-42e9-847a-d7069aa2a92b)

Penjelasan: Perintah ini menampilkan daftar file di /etc/passwd dan mengalihkan outputnya ke file_baru.txt, tetapi menggunakan >> agar tidak menimpa file yang ada, melainkan menambahkannya (append).

3.	Urutkan file baru dengan cara membelokkan standard input.
![3](https://github.com/user-attachments/assets/403c3f65-80ff-4a6e-b3f6-457730267c46)

Penjelasan: Perintah sort < file_baru.txt mengambil isi file file_baru.txt sebagai input (<) dan menampilkannya dalam urutan yang diurutkan ke layar (stdout).

4.	Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.
![4](https://github.com/user-attachments/assets/1ddd7724-9fdc-4764-9ae9-03bf3a2fe5c8)

Penjelasan: Isi file file_baru.txt diurutkan dan outputnya dialihkan ke file baru bernama file_baru.urut.

5. Buatlah direktori latihan6 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.
![5](https://github.com/user-attachments/assets/7c0481de-58d8-4e4a-a9b0-e0cc4423c212)

Penjelasan: mkdir latihan6 mencoba membuat direktori bernama latihan6. Perintah pertama mengalihkan pesan error (jika terjadi) ke rmdirerror.txt. Perintah kedua mencoba lagi membuat direktori yang sama dan menambahkan pesan error (jika ada) ke file yang sama tanpa menimpanya (2>>).

6. Urutkan kalimat dengan menggunakan notasi here document (<<@@@ …@@@).
![6](https://github.com/user-attachments/assets/5bb090ca-2420-4a88-9609-eb04e325f35c)

Penjelasan: Menggunakan here document (<<@@@), beberapa baris teks diinput ke perintah sort untuk diurutkan secara langsung.

7. Hitung jumlah baris, kata, dan karakter dari file file_baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file_baru.txt.
![7](https://github.com/user-attachments/assets/4b079c79-b8e2-49b7-9487-0811bf8db520)

Penjelasan: Perintah wc menghitung jumlah baris, kata, dan karakter dari file file_baru.urut, lalu menambahkan hasilnya ke file_baru.txt menggunakan >>.

8.  Gunakan perintah di bawah ini dan perhatikan hasilnya.
![8](https://github.com/user-attachments/assets/60c3bb04-ae18-4f83-91ea-35361295f14d)

Penjelasan:
•	cat /etc/passwd | sort | pr -n | grep tty03: Menampilkan isi file /etc/passwd, mengurutkan, menambahkan nomor halaman (pr -n), dan mencari baris yang mengandung tty03.
•	find /etc -print | head: Mencari semua file di direktori /etc dan menampilkan 10 file pertama.
•	head /etc/passwd | tail -5 | sort: Menampilkan 5 baris terakhir dari 10 baris pertama file /etc/passwd, kemudian mengurutkannya.
9. unakan perintah berikut dan perhatikan hasilnya.
![9](https://github.com/user-attachments/assets/83150510-e374-4043-a0e4-ea28f9fc0323)

Penjelasan: Perintah ini menggunakan beberapa filter (cat, sort, pr, head, tail). who menampilkan siapa yang sedang login. Output dari who dialirkan ke cat dua kali (tanpa efek) kemudian diurutkan (sort), diformat (pr), diambil bagian atasnya (head), dan kemudian bagian akhirnya diambil (tail).



