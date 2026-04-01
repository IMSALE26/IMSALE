<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>IMSALE - Keripik Pisang</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-yellow-50 font-sans">



  <!-- Produk -->
  <section class="max-w-md mx-auto bg-white rounded-2xl shadow-lg p-4 mt-6">
    <img src="https://via.placeholder.com/300" alt="Sale Pisang" class="rounded-xl mb-4">
    <h2 class="text-xl font-semibold">Keripik Pisang Kering 300g</h2>
    <p class="text-gray-600">Camilan manis alami khas Wonosobo</p>
    <p class="text-lg font-bold mt-2">Rp 15.000</p>
  </section>

  <!-- Komposisi -->
  <section class="max-w-md mx-auto bg-white rounded-2xl shadow-lg p-4 mt-4">
    <h3 class="text-lg font-bold mb-2">Komposisi</h3>
    <p class="text-gray-700">Pisang, Minyak, Garam</p>
  </section>

  <!-- Pembelian & Sosial Media -->
  <section class="max-w-md mx-auto bg-white rounded-2xl shadow-lg p-4 mt-4 mb-6 text-center">
    <h3 class="text-lg font-bold mb-3">Pesan Sekarang</h3>

    <button onclick="orderNow()" class="w-full bg-green-500 text-white p-2 rounded-xl font-bold mb-2">
      WhatsApp
    </button>

    <a href="https://instagram.com/imsale" target="_blank" class="block w-full bg-pink-500 text-white p-2 rounded-xl font-bold">
      Instagram
    </a>
  </section>

  <!-- Script -->
  <script>
    function orderNow() {
      const message = `Halo, saya ingin pesan IMSALE 🍌`;
      const phone = '6281234567890'; // ganti nomor kamu
      window.open(`https://wa.me/${phone}?text=${encodeURIComponent(message)}`);
    }
  </script>

</body>
</html>
