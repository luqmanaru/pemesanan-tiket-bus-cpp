#include <iostream>
#include <string>

using namespace std;

int main() {
    int jumlahTiket;
    long harga, ppn, totalHarga, totalBayar, uangPembayaran, uangKembali;
    string kodeBus, kodeTujuan, namaPenumpang, namaBus, namaTujuan;
    
    cout << "\n\t\tAGEN BUS SELALU SELAMAT TOUR\n";
    cout << "***********************************************************************\n";
    
    cout << "Masukkan Nama Penumpang : ";
    getline(cin, namaPenumpang);

    cout << "Masukkan Kode Bus [R/S/H] : ";
    cin >> kodeBus;

    // Menentukan nama bus berdasarkan kode
    if (kodeBus == "R" || kodeBus == "r")
        namaBus = "Rosalinda";
    else if (kodeBus == "S" || kodeBus == "s")
        namaBus = "Sinar Jaya";
    else if (kodeBus == "H" || kodeBus == "h")
        namaBus = "Hiba Utama";
    else {
        cout << "Kode Bus tidak valid.\n";
        return 1;
    }

    cout << "Masukkan Kode Tujuan [SBY/MLG/SLO/TGL/LMP/YGY] : ";
    cin >> kodeTujuan;

    // Menentukan tujuan & harga
    if (kodeTujuan == "SBY") {
        namaTujuan = "Surabaya";
        harga = 300000;
    } else if (kodeTujuan == "MLG") {
        namaTujuan = "Malang";
        harga = 400000;
    } else if (kodeTujuan == "SLO") {
        namaTujuan = "Solo";
        harga = 200000;
    } else if (kodeTujuan == "TGL") {
        namaTujuan = "Tegal";
        harga = 250000;
    } else if (kodeTujuan == "LMP") {
        namaTujuan = "Lampung";
        harga = 350000;
    } else {
        namaTujuan = "Yogyakarta";
        harga = 400000;
    }

    cout << "Jumlah Tiket : ";
    cin >> jumlahTiket;

    totalHarga = harga * jumlahTiket;
    ppn = totalHarga * 0.05;
    totalBayar = totalHarga + ppn;

    cout << "Total Harga : " << totalHarga << endl;
    cout << "PPN         : " << ppn << endl;
    cout << "Total Bayar : " << totalBayar << endl;

    cout << "Masukkan Pembayaran : ";
    cin >> uangPembayaran;
    uangKembali = uangPembayaran - totalBayar;

    cout << "\n===== STRUK PEMBELIAN =====\n";
    cout << "Nama Penumpang     : " << namaPenumpang << endl;
    cout << "Nama Bus           : " << namaBus << endl;
    cout << "Tujuan             : " << namaTujuan << endl;
    cout << "Harga per Tiket    : " << harga << endl;
    cout << "Jumlah Tiket       : " << jumlahTiket << endl;
    cout << "Total Bayar        : " << totalBayar << endl;
    cout << "Uang Kembali       : " << uangKembali << endl;

    if (jumlahTiket <= 3) {
        cout << "Bonus: Souvenir\n";
    } else {
        cout << "Bonus: Voucher Belanja Rp100.000\n";
    }

    cout << "\n*** Terima kasih telah menggunakan layanan kami ***\n";

    return 0;
}
