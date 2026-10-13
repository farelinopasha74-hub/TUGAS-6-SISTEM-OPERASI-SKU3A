# TUGAS-6-SISTEM-OPERASI-SKU3A
**TUGAS-6-SISTEM-OPERASI-SKU3A**

**Nama:** Pasha Farelino

**NIM:** 09011282530111

**KELAS:** SKU3A

1. Eksekusi seluruh profile yang ada :
a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
echo “Profile dari /etc/profile”
<img width="772" height="552" alt="Screenshot From 2026-10-13 09-22-16" src="https://github.com/user-attachments/assets/2696b679-69b3-44b8-b0f5-b23805664d65" />
<img width="774" height="537" alt="Screenshot From 2026-10-13 08-47-31" src="https://github.com/user-attachments/assets/90cf6778-f1bb-43b4-a838-1efb29ee195d" />
<img width="606" height="59" alt="Screenshot From 2026-10-13 08-47-18" src="https://github.com/user-attachments/assets/156b03ea-8d5f-49e3-9570-126fef3070cc" />


b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
/home/stD02001/.bash_profile
<img width="843" height="152" alt="Screenshot From 2026-10-13 09-00-35" src="https://github.com/user-attachments/assets/b8163480-bbb0-41d8-8c7f-31dc3d1dbb72" />
<img width="802" height="33" alt="Screenshot From 2026-10-13 09-02-33" src="https://github.com/user-attachments/assets/cf31387d-3f43-4d5a-b306-48c5561f460b" />


/home/. stD02001/.bash_login
<img width="845" height="65" alt="Screenshot From 2026-10-13 09-03-36" src="https://github.com/user-attachments/assets/1a0bf23b-1b4b-42c2-aca3-c807fe61ffef" />
<img width="845" height="65" alt="Screenshot From 2026-10-13 09-02-59" src="https://github.com/user-attachments/assets/a9160af8-3c53-4177-9bfa-e521599decea" />


/home/mahasiswa/.profile
<img width="645" height="564" alt="Screenshot From 2026-10-13 09-33-20" src="https://github.com/user-attachments/assets/96ef87f4-cedd-4f55-9424-4b271b4f16fa" />
<img width="830" height="830" alt="Screenshot From 2026-10-13 09-30-36" src="https://github.com/user-attachments/assets/99877b52-faa7-4976-b538-e07e71b0c7a3" />


/home/mahasiswa/.bashrc
<img width="845" height="65" alt="Screenshot From 2026-10-13 09-03-36" src="https://github.com/user-attachments/assets/3a366706-0949-44d3-beaa-552b450d90bf" />
<img width="993" height="809" alt="Screenshot From 2026-10-13 09-07-49" src="https://github.com/user-attachments/assets/d2a1d052-247b-4cc1-a76b-2f6e4b57cd85" />
<img width="1152" height="898" alt="Screenshot From 2026-10-13 09-06-41" src="https://github.com/user-attachments/assets/7e178774-40b4-402e-b070-b1c62545fc54" />
<img width="1347" height="961" alt="Screenshot From 2026-10-13 09-10-29" src="https://github.com/user-attachments/assets/f0551bcf-2242-4dbb-b21f-2f78b3030db7" />
<img width="1468" height="887" alt="Screenshot From 2026-10-13 09-08-25" src="https://github.com/user-attachments/assets/1fe60fef-e041-4946-86c0-631b58ef86df" />



Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
file
tersebut,
cantumkan
instruksi
echo,
misalnya
pada
/home/
mahasiswa/.bash_profile :
echo “Profile dari .bash_profile”
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file
yang bersangkutan.

<img width="463" height="172" alt="Screenshot From 2026-10-13 09-53-41" src="https://github.com/user-attachments/assets/10b95455-fcdb-446e-9f3a-481919b4b1cf" />

<img width="818" height="86" alt="Screenshot From 2026-10-13 09-01-27" src="https://github.com/user-attachments/assets/5aa2c2e4-ffc4-424a-9f40-e380bc3c0466" />


c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai
berikut:
$ su mahasiswa
$ exit
<img width="445" height="94" alt="Screenshot From 2026-10-13 10-16-25" src="https://github.com/user-attachments/assets/4ccdc515-1965-4653-bfcc-72ea8c2242cf" />

kemudian gunakan opsi – sebagai berikut :
$ su – mahasiswa
$ exit
Jelaskan perbedaan kedua utilitas tersebut.
<img width="460" height="154" alt="Screenshot From 2026-10-13 10-16-59" src="https://github.com/user-attachments/assets/e04f19f2-18e2-4396-a895-dcfc3b8a13d2" />

su mahasiswa (Substitute User biasa): Berpindah user tanpa mengubah lingkungan shell (environment variables) atau direktori kerja saat itu. Anda akan tetap berada di direktori sebelumnya dan variabel PATH atau profil login user baru tidak dimuat sepenuhnya.

su - mahasiswa (Login Shell): Berpindah user dengan menginisialisasi ulang seluruh lingkungan shell seolah-olah user tersebut baru saja melakukan login dari awal. Direktori kerja otomatis berpindah ke direktori $HOME user tersebut, dan seluruh file profil (.bash_profile, .profile, dll.) akan dieksekusi.


2. Prompt String (PS)
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan
dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal
oleh semua shell
PS1=’> ‘
export PS1
<img width="576" height="88" alt="Screenshot From 2026-10-13 10-19-28" src="https://github.com/user-attachments/assets/acece0fb-35dc-4827-a0ca-d716ab7b94e4" />


b. Eksperimen hasil PS1 :
$ PS1=“\! > “
69 > PS1=”\d > “
Mon Sep 23 > PS1=”\t > “
10:10:20 > PS1=”Saya=\u > “
Saya=mahasiswa > PS1=”\w >”
~ > PS1=\h >”

3. Logout
Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi
logout
Echo “Terima kasih atas sesi yang diberikan”
Sleep 5
clear
<img width="842" height="263" alt="Screenshot From 2026-10-13 10-27-37" src="https://github.com/user-attachments/assets/08129855-4f25-45c4-9e3d-e572e4a06949" />
<img width="754" height="234" alt="Screenshot From 2026-10-13 10-37-00" src="https://github.com/user-attachments/assets/4688ef55-2abd-4db2-9dfb-d1eb479eba75" />


4. Bash script
a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
p1.sh
#! /bin/bash
echo “Program p1” ls –l
p2.sh
#! /bin/bash
echo “Program p2” who
p3.sh
#! /bin/bash
echo “Program p3” ps x
b. Jalankan script tersebut sebagai berikut :
$ ./p1.sh ; ./p3.sh ; ./p2.sh
$ ./p1.sh &
$ ./p1.sh $ ./p2.sh & ./p3.sh &
$ ./p1.sh ; ./p3.sh ) &
<img width="759" height="168" alt="Screenshot From 2026-10-13 10-44-29" src="https://github.com/user-attachments/assets/f57a981a-1cff-4628-a1ce-eed8d02be46f" />


5. Jobs
a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik,
kemudian menyimpan tanggal dan jam pada file hasil.
#!/bin/bash
while [ true ]
do
date >> hasil
sleep 10
done
<img width="823" height="262" alt="Screenshot From 2026-10-13 10-57-36" src="https://github.com/user-attachments/assets/7a2a1f08-199c-46cb-aa50-78e6297d5d03" />


b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di
background sebagai berikut :
$ jobs
$ find / -print > files 2>/dev/null &
$ jobs
<img width="823" height="262" alt="Screenshot From 2026-10-13 10-58-58" src="https://github.com/user-attachments/assets/1618a694-c907-4d58-8355-87b33af8f330" />


c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program
tersebut ke background
$ fg %1
$ bg

<img width="879" height="961" alt="Screenshot From 2026-10-13 10-56-14" src="https://github.com/user-attachments/assets/aba58df2-aad5-452a-b9f6-f2cb61ee3f16" />

d. Stop program background dengan utilitas kill
$ ps x
<img width="851" height="824" alt="Screenshot From 2026-10-13 11-02-01" src="https://github.com/user-attachments/assets/176d4b0f-07ab-438d-9752-361f3a88a157" />

$ kill [Nomor PID]
<img width="587" height="54" alt="Screenshot From 2026-10-13 11-03-18" src="https://github.com/user-attachments/assets/afc436d6-38f0-419e-bfdd-b98fb33e07c6" />

6. History
a. Ganti nilai HISTSIZE dari 1000 menjadi 20
$ HISTSIZE=20
$ h
b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang
terakhir dilakukan
$ !-5
c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada
history bufer
$ !!

d. Ulangi instruksi pada history bufer nomor 150
$ !150
e. Ulangi instruksi dengan prefix “ls”
<img width="675" height="812" alt="image" src="https://github.com/user-attachments/assets/27047938-dc80-4a8d-abe4-3a34976201dd" />

