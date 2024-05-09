<!-- @format -->

# binar-authentication-authorization-exercise

## Slide 8

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

## Slide 9

### 1. Apa itu otorisasi?

Authorization adalah proses yang terjadi setelah identifikasi user tersebut berhasil dan hak atau akses apa saja yang bisa didapat oleh user tersebut.

### 2. Apa perbedaan utama antara otentikasi dan otorisasi?

Yang membedakannya adalah authentication itu proses untuk mendapatkan identitas sedangkan authorization itu adalah proses pemberian izin identitas tersebut.

### 3. Sebutkan dua metode otorisasi yang sering digunakan dalam sistem komputer.

1. Hak Akses Berbasis Peran (Role-Based Access Control/RBAC): Ini adalah metode di mana pengguna diberikan hak akses berdasarkan peran atau tanggung jawab mereka dalam organisasi. Sebagai contoh, seorang pegawai administrasi dapat memiliki
   akses untuk mengelola dokumen, sedangkan seorang manajer dapat memiliki akses untuk menyetujui atau menolak permintaan.
2. Pengendalian Akses Berbasis Kebijakan (Policy-Based Access Control/PBAC): Ini adalah metode di mana pengguna diberikan hak akses berdasarkan aturan atau kebijakan yang ditetapkan oleh administrator. Misalnya, sebuah perusahaan dapat
   menetapkan kebijakan bahwa hanya karyawan dengan level akses tertentu yang dapat mengakses data keuangan atau rahasia perusahaan.

### 4. Apa itu Role-based Access Control?

Role-based Access Control (RBAC) adalah sebuah model kontrol akses yang mengatur akses ke sistem komputer berdasarkan peran (role) dari pengguna dalam organisasi atau sistem.

### 5. Apa itu Policy-based Access Control?

Policy-based Access Control (PBAC) adalah cara untuk mengontrol siapa yang memiliki akses ke apa dalam sebuah sistem komputer berdasarkan pada aturan atau kebijakan yang telah ditetapkan sebelumnya. Dalam PBAC, kebijakan akses bisa
berdasarkan pada banyak hal, seperti jabatan seseorang, waktu akses, lokasi, atau tipe data yang diakses. Tujuannya adalah untuk memastikan bahwa orang hanya mendapatkan akses ke apa yang mereka butuhkan dan memiliki izin untuk menggunakan,
dan tidak lebih dari itu.

### 6. Apa keuntungan menggunakan ABAC dibandingkan dengan RBAC?

Keuntungan menggunakan ABAC dibandingkan dengan RBAC meliputi:

- Fleksibilitas yang Lebih Besar: ABAC memberikan fleksibilitas yang lebih besar dalam menentukan hak akses karena penggunaan atribut memungkinkan untuk menyesuaikan akses dengan lebih detail sesuai dengan kebutuhan bisnis atau keamanan.
- Konteks yang Lebih Kaya: Dengan ABAC, hak akses dapat dipertimbangkan dalam konteks yang lebih kaya, seperti lokasi, waktu, dan atribut lainnya, yang dapat meningkatkan keamanan dan efisiensi akses.
- Manajemen yang Lebih Efisien: ABAC dapat memudahkan manajemen hak akses karena aturan-aturan dapat dikelola secara terpusat dan diterapkan dengan lebih fleksibel sesuai dengan kebijakan organisasi.

### 7. Apa itu JSON Web Token (JWT) dan bagaimana hubungannya dengan otorisasi?

### 8. Apa yang dimaksud dengan "least privilege" dalam konteks otorisasi?

### 9. Mengapa penting untuk sering memeriksa dan memperbarui kebijakan otorisasi?

### 10. Apa itu Access Control List (ACL)?

Access Control List (ACL) adalah daftar yang menentukan izin atau hak akses yang dimiliki oleh pengguna atau grup pengguna terhadap sumber daya tertentu dalam sebuah sistem komputer. ACL biasanya diterapkan pada file, folder, atau objek
lainnya dalam sistem operasi atau jaringan komputer. ACL mendefinisikan siapa yang dapat mengakses suatu sumber daya dan apa jenis akses yang mereka izinkan, seperti membaca, menulis, atau menjalankan.

## Slide 10

### 1. Bagaimana otentikasi dan otorisasi bekerja bersama dalam keamanan sistem informasi?

### 2. Sebutkan contoh aplikasi yang menggunakan otentikasi dan otorisasi.

### 3. Apa yang terjadi jika proses otentikasi gagal?

### 4. Mengapa penting untuk log aktivitas otentikasi dan otorisasi?

### 5. Bagaimana cara sistem menangani perubahan kebijakan otorisasi tanpa mengganggu pengguna?

### 6. Apa pengaruh kegagalan sistem otentikasi terhadap proses otorisasi?

### 7. Bagaimana implementasi kebijakan "zero trust" mempengaruhi otentikasi dan otorisasi?

### 8. Apa dampak dari serangan keamanan pada sistem otentikasi dan otorisasi?

### 9. Bagaimana teknologi blockchain dapat mempengaruhi otentikasi dan otorisasi?

### 10. Apa peran administrator sistem dalam pengelolaan otentikasi dan otorisasi?
