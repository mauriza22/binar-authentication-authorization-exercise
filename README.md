<!-- @format -->

# binar-authentication-authorization-exercise

### 1. Apa itu otentikasi?

Otentikasi adalah proses verifikasi identitas user, yang digunakan untuk verifikasi tersebut biasanya username/email atau password, atau keduanya.

### 2. Sebutkan tiga faktor otentikasi yang umum digunakan.

- PIN
- Token
- Biometric

### 3. Apa perbedaan antara otentikasi dua faktor dan otentikasi multifaktor?

_otentikasi dua faktor_ -> memerlukan dua faktor yang berbeda untuk mengautentikasi pengguna. misal: user diminta untuk memasukkan password kemudian user akan menerima token melalui sms.

_otentikasi multifaktor_ -> memerlukan lebih dari dua faktor untuk mengauntentikasi pengguna. misal : aplikasi mbaking yang memerlukan pengisian beberapa data untuk meningkatkan keamanan akses pengguna.

### 4. Apa itu Single Sign-On (SSO)?

Single Sign-On (SSO) adalah sebuah mekanisme otentikasi yang memungkinkan pengguna untuk mengakses beberapa aplikasi atau layanan dengan menggunakan satu set kredensial (seperti nama pengguna dan kata sandi) yang sama. Dengan kata lain,
setelah pengguna berhasil login ke satu aplikasi atau sistem, mereka secara otomatis diotentikasi untuk mengakses aplikasi atau sistem lainnya tanpa perlu memasukkan kembali kredensial mereka.

### 5. Mengapa password dianggap sebagai bentuk otentikasi yang lemah?

1. Rentan terhadap Pencurian atau Pemalsuan: Password dapat dengan mudah dicuri atau diretas.
2. Ketergantungan pada Kebiasaan Pengguna: Banyak pengguna cenderung menggunakan kata sandi yang lemah atau memilih kata sandi yang mudah ditebak karena kenyamanan atau ketidakpedulian. Hal ini meningkatkan risiko kebocoran keamanan.

### 6. Apa itu otentikasi biometrik dan berikan dua contoh.

Otentikasi biometrik adalah proses otentikasi yang menggunakan karakteristik fisik atau perilaku unik dari individu untuk mengonfirmasi identitas mereka. Contoh:

1. Finger Print
2. Face ID

### 7. Sebutkan satu kelemahan dari otentikasi berbasis biometrik.

Misalnya, jika data sidik jari seseorang dicuri dari database yang disimpan oleh suatu perusahaan, orang tersebut tidak dapat mengubah sidik jarinya seperti yang dapat dilakukan dengan kata sandi.

### 8. Apa fungsi dari token otentikasi?

Fungsi utama dari token otentikasi adalah untuk meningkatkan keamanan akses ke akun atau sistem dengan menyediakan lapisan keamanan tambahan di luar penggunaan kata sandi saja.

### 9. Apa itu OTP dan bagaimana cara kerjanya?

OTP adalah singkatan dari "One-Time Password" atau kata sandi satu kali pakai. Ini adalah kode otentikasi yang berlaku hanya untuk satu kali penggunaan dan biasanya berlaku untuk jangka waktu terbatas. OTP digunakan sebagai metode
otentikasi tambahan dalam proses otentikasi dua faktor (2FA) atau otentikasi multifaktor (MFA) untuk meningkatkan keamanan akses ke akun atau sistem.

1. Saat pengguna mencoba untuk login atau mengakses sistem yang memerlukan otentikasi tambahan, mereka diminta memasukkan kode OTP bersama dengan kredensial otentikasi lainnya, seperti nama pengguna dan kata sandi.
2. Pengguna memasukkan kode OTP yang mereka terima ke dalam kolom yang ditentukan pada halaman login atau proses otentikasi. Kode ini harus dimasukkan dengan benar dan dalam jangka waktu yang ditentukan.
3. Sistem otentikasi memverifikasi kode OTP yang dimasukkan oleh pengguna dengan kode yang diharapkan atau yang diharapkan berdasarkan algoritma yang sama yang digunakan untuk menghasilkan kode OTP. Jika kode yang dimasukkan cocok dengan
   yang diharapkan, otentikasi berhasil dan pengguna diberikan akses ke akun atau sistem yang diminta.

### 10. Bagaimana otentikasi dapat diperkuat dalam sistem online?

1. Mengimplementasikan Otentikasi Multifaktor (MFA)
2. Mewajibkan pengguna untuk menggunakan kata sandi yang kuat dengan panjang yang mencukupi, campuran huruf besar dan kecil, angka, dan karakter khusus
3. Menggunakan teknologi biometrik, seperti pemindaian sidik jari atau pemindaian wajah, sebagai faktor otentikasi tambahan dapat memperkuat keamanan sistem dengan mengandalkan karakteristik fisik unik dari individu.
