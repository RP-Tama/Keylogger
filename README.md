# Keylogger Menggunakan Python dengan Pynput

Skrip Python ini berfungsi sebagai keylogger sederhana yang menggunakan perpustakaan Pynput. Ini menangkap dan mencatat ketukan tombol ke dalam file teks untuk analisis lebih lanjut. Harap dicatat bahwa penggunaan keylogger tanpa izin tertulis adalah tidak etis dan dapat melanggar hukum. Pastikan Anda memiliki izin yang tepat sebelum menggunakan atau mendistribusikan alat seperti ini.

## Persyaratan

Sebelum menjalankan skrip, pastikan Anda telah menginstal dependensi yang diperlukan. Anda dapat menginstalnya menggunakan perintah berikut:

```bash
pip install pynput
```

## Instalasi

1. Klon repository:

    ```bash
    git clone https://github.com/nama-pengguna-anda/keylogger.git
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

## Penyangkalan

Skrip ini ditujukan untuk tujuan pendidikan dan informasi saja. Ketahui implikasi hukumnya dan selalu peroleh izin yang sesuai sebelum menggunakan atau mendistribusikan keylogger.

## Lisensi

Proyek ini dilisensikan di bawah Lisensi MIT - lihat file [LICENSE](LICENSE) untuk detailnya.

---
