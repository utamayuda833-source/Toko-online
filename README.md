toko-online/
├── index.html   <- isi produk
├── style.css    <- bunga sakura
└── script.js    <- 0895348749026
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Toko NamaKamu</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header>
    <h1>🛍️ Toko sakura</h1>
    <p>Barang berkualitas, harga bersahabat</p>
  </header>

  <section class="produk">
    <div class="card">
      <img src="https://via.placeholder.com/300" alt="Produk 1">
      <h3>Kaos Polos Premium</h3>
      <p>Rp 89.000</p>
      <button onclick="pesanWA('Kaos Polos Premium', 89000)">Pesan via WA</button>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/300" alt="Produk 2">
      <h3>Hoodie Oversize</h3>
      <p>Rp 199.000</p>
      <button onclick="pesanWA('Hoodie Oversize', 199000)">Pesan via WA</button>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/300" alt="Produk 3">
      <h3>Topi Baseball</h3>
      <p>Rp 65.000</p>
      <button onclick="pesanWA('Topi Baseball', 65000)">Pesan via WA</button>
    </div>
  </section>

  <footer>
    <p>© 2026 Toko sakura | Jakarta</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body { font-family: Arial; margin: 0; background: #f5f5f5; }
header { background: #ff6b6b; color: white; text-align: center; padding: 30px; }
.produk { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; padding: 20px; }
.card { background: white; padding: 15px; border-radius: 12px; text-align: center; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
.card img { width: 100%; border-radius: 8px; }
.card button { background: #25D366; color: white; border: none; padding: 10px 20px; border-radius: 8px; cursor: pointer; font-size: 16px; }
.card button:hover { background: #128C7E; }
footer { text-align: center; padding: 20px; color: #777; }
function pesanWA(namaProduk, harga) {
  const nomor = "62895348749026"; // GANTI INI
  const pesan = `Halo, saya mau pesan:\n${KAOS POLOS}\nHarga: Rp ${harga.toLocaleString('id-ID')}`;
  const url = `https://wa.me/${62895348749026
  }?text=${encodeURIComponent(pesan)}`;
  window.open(url, '_blank');
}
