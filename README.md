# Background
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clingy Pepes ($CLINGYP)</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #fef6e4;
      color: #333;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
      animation: fadeIn 2s ease-in;
    }
    header {
      background-color: #f582ae;
      color: white;
      padding: 2rem;
      text-align: center;
      animation: slideDown 1s ease-out;
    }
    section {
      padding: 2rem;
      max-width: 900px;
      margin: auto;
      animation: fadeInUp 1.5s ease;
    }
    h2 {
      color: #ff8fab;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background-color: #fcd5ce;
      color: #555;
      animation: fadeIn 2s ease-in 1s;
    }

    .floating-token {
      position: absolute;
      top: 20%;
      left: -100px;
      width: 80px;
      animation: floatAcross 20s linear infinite;
      z-index: 0;
    }

    .background-stars {
      background: repeating-linear-gradient(0deg, #fff1 0 1px, transparent 1px 3px);
      animation: starsMove 60s linear infinite;
      position: fixed;
      width: 100%;
      height: 100%;
      z-index: -1;
    }

    .buy-button, .countdown, .tracker-link {
      text-align: center;
      margin-top: 2rem;
    }
    .buy-button a {
      background: #f582ae;
      color: white;
      padding: 0.8rem 2rem;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }
    .buy-button a:hover {
      background: #ffb3c6;
    }
    .countdown span {
      font-size: 1.5rem;
      color: #ff5d8f;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes slideDown {
      from { transform: translateY(-100%); }
      to { transform: translateY(0); }
    }
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes floatAcross {
      0% { transform: translateX(0) rotate(0deg); }
      100% { transform: translateX(110vw) rotate(360deg); }
    }
    @keyframes starsMove {
      from { background-position: 0 0; }
      to { background-position: 0 1000px; }
    }
  </style>
</head>
<body>
  <div class="background-stars"></div>
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/99/Token_icon_coin.png" alt="token" class="floating-token">
  <header>
    <h1>Clingy Pepes ($CLINGYP)</h1>
    <p>Koin Meme Paling Bucin di Blockchain Solana</p>
  </header>

  <section>
    <h2>Pendahuluan</h2>
    <p>
      Di era kripto yang penuh dengan proyek ambisius, Clingy Pepes hadir sebagai simbol loyalitas berlebihan dan cinta tak berbalas.
      Terinspirasi dari meme katak yang memeluk kaki manusia, $CLINGYP adalah token cinta absurd yang berjalan di atas blockchain Solana.
    </p>

    <h2>Misi & Visi</h2>
    <p><strong>Misi:</strong> Menyebarkan tawa, cinta, dan ketergantungan digital lewat meme dan komunitas clingy.</p>
    <p><strong>Visi:</strong> Menjadi koin meme nomor satu di Solana dengan komunitas yang bucin maksimal.</p>

    <h2>Tokenomik</h2>
    <ul>
      <li>Total Pasokan: 69.000.000.000</li>
      <li>Pajak: 0%</li>
      <li>Distribusi: 50% Airdrop, 20% Likuiditas, 15% Tim, 10% Ekosistem, 5% Pemasaran</li>
    </ul>

    <h2>Fungsi</h2>
    <ul>
      <li>Marketplace NFT Meme</li>
      <li>Staking "Cuddle Points"</li>
      <li>DAO Komunitas</li>
    </ul>

    <h2>Roadmap</h2>
    <p><strong>Q2 2025:</strong> Peluncuran Token, Airdrop, Listing DEX</p>
    <p><strong>Q3 2025:</strong> Peluncuran NFT, Staking, Kolaborasi Influencer</p>
    <p><strong>Q4 2025:</strong> Aktivasi DAO, Merchandise, Event Komunitas</p>

    <div class="buy-button">
      <a href="#">Beli $CLINGYP Sekarang</a>
    </div>

    <div class="countdown">
      <h2>Countdown Airdrop</h2>
      <span id="countdown"></span>
    </div>

    <div class="tracker-link">
      <p><a href="https://solscan.io/token/CLINGYP" target="_blank">Lihat di Solscan</a></p>
    </div>

    <script>
      const countdownDate = new Date("2025-05-01T00:00:00").getTime();
      const countdownEl = document.getElementById("countdown");
      const interval = setInterval(() => {
        const now = new Date().getTime();
        const distance = countdownDate - now;

        if (distance < 0) {
          clearInterval(interval);
          countdownEl.innerHTML = "Airdrop Dimulai!";
        } else {
          const days = Math.floor(distance / (1000 * 60 * 60 * 24));
          const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
          const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
          const seconds = Math.floor((distance % (1000 * 60)) / 1000);
          countdownEl.innerHTML = `${days}h ${hours}j ${minutes}m ${seconds}d`;
        }
      }, 1000);
    </script>

    <h2>Penutup</h2>
    <p>
      Clingy Pepes adalah perayaan rasa tidak rela ditinggal, dibungkus dalam meme, dan diperkuat oleh teknologi Solana. Gabung sekarang dan jadi bagian dari gerakan clingy!
    </p>
  </section>

  <footer>
    <p>#TetapClingy | $CLINGYP | Clingy Pepes 2025</p>
  </footer>
</body>
</html>
