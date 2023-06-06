# Bowo-Ajaah



<!DOCTYPE html>
<html>
<head>
  <title>Formulir Kirim ke WhatsApp</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
    }

    .container {
      max-width: 400px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      color: #333;
    }

    input[type="text"], textarea {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
      resize: vertical;
    }

    .btn-submit {
      display: block;
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      background-color: #4CAF50;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }

    .btn-submit:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Formulir Kirim ke WhatsApp</h2>
    <form action="https://api.whatsapp.com/send" method="GET">
      <input type="hidden" name="phone" value="nomor_telepon_pengguna_whatsapp">
      <input type="hidden" name="text" value="Nama: {{nama}}%0AEmail: {{email}}%0AKomentar: {{komentar}}">
      <label for="nama">Nama:</label>
      <input type="text" id="nama" name="nama" placeholder="Masukkan nama Anda" required>
      <label for="email">Alamat Email:</label>
      <input type="text" id="email" name="email" placeholder="Masukkan alamat email Anda" required>
      <label for="komentar">Komentar:</label>
      <textarea id="komentar" name="komentar" placeholder="Tulis komentar Anda" required></textarea>
      <input type="submit" value="Kirim via WhatsApp" class="btn-submit">
    </form>
  </div>
</body>
</html>
