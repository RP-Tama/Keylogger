# Keylogger Menggunakan Python dengan Pynput
Github ini dibuat sebagai pemenuhan tugas kelas Keamanan Jaringan Komputer (ET234302) 2023, Departemen Teknologi Informasi, Institut Teknologi Sepuluh Nopember

## Anggota kelompok Keamanan jaringan komputer
Muhammad Dzakwan 5027201065
Fransiskus Benyamin S 5027211021
Muhamad Ilham Yumna 5027211024
Raditya Pratama 5027211047
Wisnu Adjie Saka 5027211051

Skrip Python ini berfungsi sebagai keylogger sederhana yang menggunakan perpustakaan Pynput. Ini menangkap dan mencatat ketukan tombol ke dalam file teks untuk analisis lebih lanjut. 

Sebagai introduksi, keylogger adalah alat yang dapat digunakan dalam penerapan keamanan jaringan komputer. Keylogger memiliki beberapa fungsi sebagai berikut:

1. Investigasi Insiden Keamanan: Keylogger dapat digunakan sebagai alat forensik untuk menyelidiki insiden keamanan. Dengan merekam aktivitas keyboard, peneliti keamanan dapat mencari tahu cara serangan terjadi, memahami alur serangan, dan mengidentifikasi sumber masalah.

2. Pendeteksian Ancaman: Keylogger dapat membantu dalam mendeteksi ancaman keamanan dengan merekam aktivitas yang mencurigakan, seperti upaya login yang gagal, penggunaan kata sandi yang tidak valid, atau aktivitas lain yang dapat mengindikasikan serangan.

3. Pengujian Keamanan: Ahli keamanan sering menggunakan keylogger sebagai alat uji penetrasi untuk mengevaluasi kekuatan dan kelemahan sistem keamanan. Dengan merekam aktivitas keyboard, mereka dapat menilai sejauh mana sistem dapat menahan serangan atau apakah ada celah keamanan yang perlu diperbaiki.
Peringatan Dini Terhadap Ancaman Keamanan: Keylogger dapat membantu dalam mendeteksi dan memberikan peringatan dini terhadap ancaman keamanan, seperti serangan malware atau upaya phishing, yang mungkin mencoba mencuri informasi pribadi atau kredensial login.

4. Penelitian Keamanan: Keylogger dapat digunakan oleh para peneliti keamanan untuk mengumpulkan data tentang ancaman baru dan teknik serangan yang muncul, sehingga mereka dapat mengembangkan solusi keamanan yang lebih efektif.
## Persyaratan

Sebelum menjalankan skrip, pastikan Anda telah menginstal dependensi yang diperlukan. Anda dapat menginstalnya menggunakan perintah berikut:

```bash
pip install pynput
```

## Instalasi

1. Klon repository:

    ```bash
    git clone https://github.com/RP-Tama/Keylogger.git
    ```

2. Pindah ke direktori proyek:

    ```bash
    cd keylogger
    ```

3. Instal paket Python yang diperlukan:

    ```bash
    pip install -r requirements.txt
    ```

## Penggunaan

1. Buka skrip dalam editor teks.

2. Sesuaikan variabel `log_dir` untuk menentukan direktori di mana Anda ingin menyimpan keylog. Contoh:

    ```python
    log_dir = "/path/to/your/logs/"
    ```

3. Jalankan skrip:

    ```bash
    python keylogger.py
    ```

4. Keylogger akan mulai berjalan, menangkap, dan mencatat ketukan tombol secara real-time.

5. Untuk menghentikan keylogger, tekan `Ctrl + C` di terminal tempat skrip berjalan.

## Konfigurasi

Anda dapat memodifikasi skrip ini sesuai kebutuhan Anda. Beberapa penyesuaian yang mungkin termasuk:

- **Tingkat Logging**: Ubah tingkat logging untuk mengontrol sejauh mana detail log. Misalnya, Anda dapat mengaturnya ke `logging.INFO` untuk log yang kurang terperinci.

- **Format Log**: Sesuaikan format log untuk menyertakan informasi tambahan atau sesuaikan format timestamp.

```python
logging.basicConfig(filename=(log_dir + "keylogs.txt"), \
    level=logging.DEBUG, format='%(asctime)s: %(message)s')
```
