# UTS_Algoritma
# NAMA: JULIUS HUTABARAT
# NIM: 312410429
# Kelas: TI.24.A3

# Codingan Program Kasir

```
class Barang:
    def __init__(self, nama, harga, jumlah):
        self.nama = nama
        self.harga = harga
        self.jumlah = jumlah

    def total_harga(self):
        return self.harga * self.jumlah


class Keranjang:
    def __init__(self):
        self.barang_list = []

    def tambah_barang(self, barang):
        self.barang_list.append(barang)

    def tampilkan_daftar_barang(self):
        print("Daftar Barang dalam Keranjang:")
        for i, barang in enumerate(self.barang_list, start=1):
            print(f"{i}. {barang.nama} - Harga: {barang.harga} x Jumlah: {barang.jumlah} = Total: {barang.total_harga()}")

    def hitung_total_harga(self):
        total = sum(barang.total_harga() for barang in self.barang_list)
        return total

    def cetak_struk(self):
        print("\n--- Struk Pembelian ---")
        self.tampilkan_daftar_barang()
        total = self.hitung_total_harga()
        print(f"\nTotal Harga: {total}")
        print("-----------------------")


# Contoh penggunaan
if __name__ == "__main__":
    keranjang = Keranjang()

    # Menambah barang ke dalam keranjang
    barang1 = Barang("Baju", 100.000, 1)
    barang2 = Barang("Celana", 200.000, 1)
    barang3 = Barang("Sepatu", 450.000, 1)

    keranjang.tambah_barang(barang1)
    keranjang.tambah_barang(barang2)
    keranjang.tambah_barang(barang3)

    # Menampilkan daftar barang
    keranjang.tampilkan_daftar_barang()

    # Menghitung total harga
    total_harga = keranjang.hitung_total_harga()
    print(f"\nTotal Harga Keseluruhan: {total_harga}")

    # Mencetak struk
    keranjang.cetak_struk()
```
# Hasil Codingan Program Kasir
![Screenshot 2024-11-08 102757](https://github.com/user-attachments/assets/009744fd-adf6-44b7-a91b-cb95544cb319)

# Algorima dari codingan program kasir

Algoritma Program Kasir
Definisi Kelas Barang:

Buat kelas Barang dengan atribut:
nama: Nama barang.
harga: Harga per unit barang.
jumlah: Jumlah barang yang dibeli.
Tambahkan metode total_harga():
Hitung total harga untuk barang tersebut dengan mengalikan harga dan jumlah.
Definisi Kelas Keranjang:

Buat kelas Keranjang dengan atribut:
barang_list: Sebuah list yang akan menyimpan objek-objek Barang.
Tambahkan metode tambah_barang(barang):
Tambahkan objek Barang ke dalam barang_list.
Tambahkan metode tampilkan_daftar_barang():
Tampilkan daftar semua barang dalam keranjang dengan format yang jelas, termasuk harga dan jumlah.
Tambahkan metode hitung_total_harga():
Hitung total harga dari semua barang dalam barang_list dengan menjumlahkan hasil dari metode total_harga() untuk setiap barang.
Tambahkan metode cetak_struk():
Tampilkan struk pembelian yang mencakup daftar barang dan total harga keseluruhan.
Contoh Penggunaan:

Buat objek Keranjang baru.
Buat beberapa objek Barang dengan nama, harga, dan jumlah yang berbeda.
Tambahkan objek Barang tersebut ke dalam keranjang menggunakan metode tambah_barang().
Tampilkan daftar barang dalam keranjang dengan memanggil metode tampilkan_daftar_barang().
Hitung dan tampilkan total harga keseluruhan dengan memanggil metode hitung_total_harga().
Cetak struk pembelian lengkap dengan memanggil metode cetak_struk().
Rangkaian Langkah-langkah dalam Algoritma
Inisialisasi:

Buat instance dari Keranjang.
Menambah Barang:

Buat beberapa instance dari Barang dengan detail yang diinginkan.
Tambahkan setiap instance Barang ke dalam keranjang menggunakan tambah_barang().
Menampilkan Daftar Barang:

Panggil tampilkan_daftar_barang() untuk melihat semua barang yang ada di keranjang.
Menghitung Total Harga:

Panggil hitung_total_harga() untuk menghitung total harga semua barang di keranjang dan tampilkan hasilnya.
Mencetak Struk:

Panggil cetak_struk() untuk mencetak daftar barang dan total harga dalam format struk.
Contoh Alur Kerja Program
Pengguna menjalankan program.
Program membuat objek keranjang baru.
Program menambahkan barang ke dalam keranjang.
Program menampilkan daftar barang yang ada di keranjang.
Program menghitung total harga dari barang-barang yang ada di keranjang.
Program mencetak struk pembelian yang mencakup daftar barang dan total harga.
