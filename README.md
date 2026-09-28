# Pertemuan 1 Dasar Dart
```dart
void main() {
  String namaPelanggan = 'Azkia Alfin Zulfikar';
  int jumlahPesan = 31;
  double hargaSatuan = 10;
  bool isMember = true;
  
  String? catatanDiskon;
  String infoDiskon = catatanDiskon ?? 'Tidak ada diskon khusus';
  
  print('Pelanggan: $namaPelanggan (Member: $isMember)');
  print('Total Belanja: ${jumlahPesan * hargaSatuan}');
  print('Catatan: $infoDiskon');

  final String idTransaksi = 'TRANSAKSI-${DateTime.now().millisecondsSinceEpoch}';
  const double pajakPpn = 0.12;
  
  print('ID Transaksi: $idTransaksi');
  print('Tarif PPN: ${pajakPpn * 100}%');

  late String statusPengiriman;
  statusPengiriman = 'Sedang dikirim oleh kurir';
  print('Status: $statusPengiriman');

  List<String> menuFavorit = ['Kopi Susu', 'Roti Bakar', 'Kopi Susu'];
  print('Menu Favorit (List): $menuFavorit');

  Set<String> kategoriUnik = {'Minuman', 'Makanan', 'Minuman'};
  print('Kategori Unik (Set): $kategoriUnik');

  Map<String, dynamic> dataPesanan = {
    'id': 101,
    'menu': 'Kopi Hitam',
    'tersedia': true,
  };
  print('Detail Pesanan (Map): Nama Menu = ${dataPesanan['menu']}');
}
