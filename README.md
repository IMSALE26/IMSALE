<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>IMSALE - Keripik Pisang</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-yellow-50 font-sans">

  <!-- Header -->
  <header class="bg-orange-500 text-white p-4 text-center text-2xl font-bold">
    IMSALE 🍌
  </header>

  <!-- Hero -->
  <section class="text-center p-6">
    <h1 class="text-3xl font-bold">Keripik Pisang Kering</h1>
    <p class="mt-2 text-gray-700">Authentic Taste, No Compromise</p>
  </section>

  <!-- Product -->
  <section class="max-w-md mx-auto bg-white rounded-2xl shadow-lg p-4">
    <img src="https://via.placeholder.com/300" alt="Sale Pisang" class="rounded-xl mb-4">
    <h2 class="text-xl font-semibold">IMSALE 300g</h2>
    <p class="text-gray-600">Camilan manis alami khas Wonosobo</p>
    <p class="text-lg font-bold mt-2">Rp 15.000</p>

    <!-- Order Form -->
    <form class="mt-4">
      <input type="text" placeholder="Nama" class="w-full border p-2 rounded mb-2" required>
      <input type="text" placeholder="Alamat" class="w-full border p-2 rounded mb-2" required>
      <input type="number" placeholder="Jumlah" class="w-full border p-2 rounded mb-2" required>
      <button type="button" onclick="orderNow()" class="w-full bg-orange-500 text-white p-2 rounded-xl font-bold">Pesan Sekarang</button>
    </form>
  </section>

  <!-- Script -->
  <script>
    function orderNow() {
      const name = document.querySelectorAll('input')[0].value;
      const address = document.querySelectorAll('input')[1].value;
      const qty = document.querySelectorAll('input')[2].value;

      const message = `Halo, saya ingin pesan IMSALE 🍌\nNama: ${name}\nAlamat: ${address}\nJumlah: ${qty}`;
      const phone = '6281234567890'; // ganti dengan nomor kamu

      window.open(`https://wa.me/${phone}?text=${encodeURIComponent(message)}`);
    }
  </script>

</body>
</html>
