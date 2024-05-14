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

- Fleksibilitas: ABAC memberikan fleksibilitas yang lebih besar dalam menentukan hak akses karena penggunaan atribut memungkinkan untuk menyesuaikan akses dengan lebih detail sesuai dengan kebutuhan bisnis atau keamanan.
- Konteks yang Lebih kompleks: Dengan ABAC, hak akses dapat dipertimbangkan dalam konteks yang lebih kompleks, seperti lokasi, waktu, dan atribut lainnya, yang dapat meningkatkan keamanan dan efisiensi akses.
- Manajemen yang Lebih Efisien: ABAC dapat memudahkan manajemen hak akses karena aturan-aturan dapat dikelola secara terpusat dan diterapkan dengan lebih fleksibel sesuai dengan kebijakan organisasi.

### 7. Apa itu JSON Web Token (JWT) dan bagaimana hubungannya dengan otorisasi?

JSON Web Token (JWT) adalah format yang digunakan untuk mentransfer informasi terstruktur secara aman antara dua pihak. JWT biasanya digunakan untuk mengotentikasi dan mengotorisasi pengguna dalam sistem yang terdistribusi atau terhubung
secara jaringan.

JWT memiliki tiga bagian utama: header, payload, dan signature. Header mengidentifikasi jenis token dan algoritma yang digunakan untuk mengenkripsi data. Payload berisi informasi yang ingin disampaikan, seperti ID pengguna atau izin akses.
Signature adalah hasil dari penggabungan header dan payload dengan sebuah kunci rahasia, yang digunakan untuk memastikan bahwa token tidak diubah atau dipalsukan.

Hubungannya dengan otorisasi -> JWT sering digunakan sebagai cara untuk memberikan izin akses kepada pengguna dalam sistem. Setelah pengguna berhasil melakukan otentikasi dan diberikan JWT, token tersebut dapat digunakan untuk mengakses
sumber daya atau layanan yang dilindungi oleh sistem. Informasi dalam payload JWT seringkali berisi izin-izin yang diberikan kepada pengguna, seperti apa yang mereka bisa lakukan dan apa yang tidak mereka bisa lakukan.

### 8. Apa yang dimaksud dengan "least privilege" dalam konteks otorisasi?

"Least privilege" dalam konteks otorisasi berarti memberikan pengguna atau sistem hanya hak akses yang diperlukan untuk menjalankan tugas atau fungsi tertentu, dan tidak memberikan hak akses yang lebih banyak dari yang dibutuhkan.

Dengan menerapkan prinsip "least privilege", sistem komputer atau organisasi hanya memberikan akses yang tepat kepada pengguna atau sistem untuk melakukan tugas atau fungsi yang diperlukan. Hal ini membantu mengurangi risiko keamanan karena
mengurangi jumlah akses yang tidak perlu dan meminimalkan dampak jika ada kebocoran keamanan atau pelanggaran yang terjadi.

### 9. Mengapa penting untuk sering memeriksa dan memperbarui kebijakan otorisasi?

1. **Mengurangi Risiko Keamanan**: Ketika kebijakan otorisasi diperiksa secara teratur, maka kita dapat mengidentifikasi dan memperbaiki celah keamanan atau kelemahan yang mungkin ada dalam sistem. Ini membantu mengurangi risiko akses tidak
   sah atau penyalahgunaan oleh pihak yang tidak berwenang.

2. **Menyesuaikan dengan Perubahan**: Dengan memeriksa dan memperbarui kebijakan otorisasi secara berkala, kita dapat memastikan bahwa kebijakan tersebut tetap relevan dan sesuai dengan kebutuhan bisnis dan regulasi yang berlaku saat ini.

3. **Mengikuti Prinsip Least Privilege**: Dengan memeriksa kebijakan otorisasi, kita dapat memastikan bahwa setiap pengguna atau sistem hanya memiliki akses sesuai dengan yang dibutuhkan untuk melakukan tugas-tugas mereka (prinsip least
   privilege). Hal ini membantu mencegah akses yang tidak perlu dan mengurangi risiko penyalahgunaan.

### 10. Apa itu Access Control List (ACL)?

Access Control List (ACL) adalah daftar yang menentukan izin atau hak akses yang dimiliki oleh pengguna atau grup pengguna terhadap sumber daya tertentu dalam sebuah sistem komputer. ACL biasanya diterapkan pada file, folder, atau objek
lainnya dalam sistem operasi atau jaringan komputer. ACL mendefinisikan siapa yang dapat mengakses suatu sumber daya dan apa jenis akses yang mereka izinkan, seperti membaca, menulis, atau menjalankan.

## Slide 10

### 1. Bagaimana otentikasi dan otorisasi bekerja bersama dalam keamanan sistem informasi?

memastikan bahwa hanya pengguna yang sah yang mendapatkan akses yang sesuai

### 2. Sebutkan contoh aplikasi yang menggunakan otentikasi dan otorisasi.

Aplikasi Mbanking:

Otentikasi: Pengguna harus memasukkan username dan kata sandi mereka. Dan juga menggunakan otentikasi dua faktor (2FA) seperti kode OTP yang dikirim ke ponsel pengguna saat pertama kali mendaftar.

Otorisasi: Setelah masuk, pengguna memiliki akses untuk melihat saldo, melihat riwayat transaksi, melakukan transfer uang, atau membayar tagihan berdasarkan izin yang diberikan oleh bank.

### 3. Apa yang terjadi jika proses otentikasi gagal?

Pengguna tidak akan diberikan akses ke sistem atau aplikasi. Hal ini dilakukan untuk memastikan bahwa hanya pengguna yang sah dan terverifikasi yang dapat mengakses sumber daya yang dilindungi.

### 4. Mengapa penting untuk log aktivitas otentikasi dan otorisasi?

Log aktivitas otentikasi dan otorisasi memungkinkan organisasi untuk mendeteksi upaya akses yang tidak sah atau aktivitas mencurigakan. Jika ada pola login yang mencurigakan, seperti upaya login yang gagal berturut-turut atau akses dari
lokasi geografis yang tidak biasa, tim keamanan dapat mengambil tindakan cepat untuk mencegah potensi serangan.

### 5. Bagaimana cara sistem menangani perubahan kebijakan otorisasi tanpa mengganggu pengguna?

Sebelum menerapkan perubahan kebijakan otorisasi, lakukan perencanaan dan pengujian di sebelum production. Ini membantu memastikan bahwa perubahan tidak akan menyebabkan gangguan yang tidak diinginkan.

Test akses dengan berbagai peran pengguna untuk memastikan bahwa kebijakan baru bekerja sesuai yang diharapkan.

### 6. Apa pengaruh kegagalan sistem otentikasi terhadap proses otorisasi?

Jika otentikasi gagal, pengguna tidak akan dapat membuktikan identitas mereka. Tanpa identitas yang terverifikasi, sistem tidak dapat melanjutkan ke langkah berikutnya, yaitu otorisasi. Akibatnya, pengguna tidak akan mendapatkan akses ke
feature atau informasi yang mereka butuhkan atau minta.

### 7. Bagaimana implementasi kebijakan "zero trust" mempengaruhi otentikasi dan otorisasi?

Prinsip "zero trust" berarti bahwa tidak ada pengguna atau perangkat yang dipercaya secara otomatis, bahkan jika mereka berada di dalam jaringan organisasi. Sehingga

- Dalam kebijakan "zero trust", setiap permintaan akses harus diautentikasi, tidak peduli dari mana asalnya. Ini berarti bahwa setiap kali pengguna atau perangkat mencoba mengakses aplikasi, mereka harus membuktikan identitas mereka melalui
  proses otentikasi yang ketat.

- Kebijakan "zero trust" biasanya mendorong penggunaan otentikasi multifaktor (MFA), yang mengharuskan pengguna untuk memverifikasi identitas mereka menggunakan lebih dari satu metode (misalnya, kata sandi ditambah kode OTP dari ponsel).

### 8. Apa dampak dari serangan keamanan pada sistem otentikasi dan otorisasi?

- Data Sensitif Terancam: Jika penyerang berhasil melewati otentikasi, mereka dapat mengakses data sensitif, termasuk informasi pribadi, keuangan, atau rahasia perusahaan.

- Manipulasi Sistem: Penyerang dapat mengubah atau menghapus data, atau bahkan menanamkan malware yang dapat menyebabkan kerusakan lebih lanjut.

### 9. Bagaimana teknologi blockchain dapat mempengaruhi otentikasi dan otorisasi?

Data yang disimpan di blockchain tidak dapat diubah atau dihapus. Ini memberikan audit trail yang aman dan transparan untuk semua aktivitas otentikasi dan otorisasi. Dengan menggunakan kriptografi yang kuat, blockchain memastikan bahwa data
yang disimpan terlindungi dari modifikasi yang tidak sah.

### 10. Apa peran administrator sistem dalam pengelolaan otentikasi dan otorisasi?

- Mereka memastikan bahwa pengguna memiliki akses yang sesuai dengan kebutuhan pekerjaan mereka, tetapi juga menerapkan prinsip least privilege untuk membatasi akses hanya pada apa yang benar-benar diperlukan.

- Mereka harus merespons dengan cepat terhadap indikasi serangan keamanan atau kegiatan yang mencurigakan, dan mengambil tindakan pencegahan atau pemulihan yang sesuai.

- Mereka harus memastikan kebijakan tersebut diterapkan secara konsisten di seluruh organisasi dan disesuaikan dengan peraturan perundang-undangan dan standar keamanan yang berlaku.
