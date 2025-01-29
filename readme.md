# Instagram Unfollow Checker

Tools sederhana ini membantu kamu melihat siapa saja yang tidak mem-follow balik akun Instagram kamu. Script ini bekerja dengan membandingkan data dari daftar "Following" (akun yang kamu ikuti) dan "Followers" (akun yang mengikuti kamu) menggunakan file JSON yang diunduh dari Instagram.

---

## Fitur
- Menganalisis daftar "following" dan "followers".
- Menampilkan daftar akun yang tidak mem-follow balik kamu dalam format URL yang dapat diakses langsung.

---

## Cara Kerja
1. **Ekspor Data Instagram:**
   - Masuk ke akun Instagram kamu.
   - Pergi ke "Pengaturan" > "Pusat Akun" > "Informasi Dan izin Anda".
   - Lalu "Unduh Informasi Anda" > "Mengunduh atau Mentrasnfer Informasi" > "Beberapa Informasi Anda" 
   - Setelah itu cari Koneksi dan pilih "Pengikut dan Mengikuti"
   - Lanjut "Unduh Ke Perangkat"
   - Untuk Rentang Tanggal disesuaikan saja dengan selera masing masing, kalau saya disini pilih "Sepanjang Waktu"
   - Terus untuk Pemberitahuan itu email nya default , Terus ubah Format nya yang tadinya HTML menjadi JSON
   - Kualitas media cukup di sedang saja, lalu pencet/tekan buat file
   - Minta salinan data akun kamu. File ini biasanya akan dikirim melalui email atau bisa download lewat instagram.
   - Setelah menerima data, ekstrak file ZIP dan cari folder `connections/followers_and_following`.

2. **Simpan File:**
   - Letakkan file JSON berikut di dalam folder yang sama dengan script ini:
     - `followers_1.json`
     - `following.json`

3. **Jalankan Script:**
   - Pastikan Python sudah terinstall di perangkat kamu.
   - Buka terminal atau command prompt, navigasikan ke folder tempat script ini berada, lalu jalankan perintah berikut:
     ```bash
     python main.py
     ```

4. **Hasil:**
   - Script akan mencetak daftar URL akun Instagram yang kamu ikuti tetapi tidak mengikuti kamu kembali.

---

## Prasyarat
- Python 3.x
- File JSON hasil ekspor data Instagram:
  - `followers_1.json`
  - `following.json`

---

## Struktur File
```
|-- main.py
|-- followers_1.json
|-- following.json
|-- blocked_profiles.json
|-- close_friends.json
|-- follow_requests_you've_received.json
|-- hide_story_from.json
|-- pending_follow_requests.json
|-- recently_unfollowed_profiles.json
|-- recent_follow_requests.json
|-- removed_suggestions.json
```

---

## Contoh Output
Setelah menjalankan script, output akan berupa daftar URL akun yang tidak mem-follow balik kamu. Contoh:
```
https://www.instagram.com/alpnp_
https://www.instagram.com/storemeta4sec
https://www.instagram.com/jalanbarengintrovert
https://www.instagram.com/thecyberkarta
https://www.instagram.com/luxyife
https://www.instagram.com/exabytes_id
https://www.instagram.com/trimarthatobaccos
https://www.instagram.com/meta4sec
https://www.instagram.com/bayashi_tv
https://www.instagram.com/ismaelcocinillas
https://www.instagram.com/vixtrade.id
https://www.instagram.com/redlimit.id/
https://www.instagram.com/timothyronaldd
https://www.instagram.com/gdgoc.ug/
https://www.instagram.com/technofair
https://www.instagram.com/cybercom.ug
https://www.instagram.com/ncsc_id

atau bisa dilihat seperti ini

![Output Following](<Output_Following.png>)
```

---

**Selamat menggunakan!**

### Dikembangkan oleh: **[zfernm](https://www.linkedin.com/in/samuel-hamonangan-s-099604255/)**
