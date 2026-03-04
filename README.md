<!GET YOUR FREE GAMES l>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ManyMods - Premium Modded Apps Collection</title>

  <!-- External CSS -->
  <style>
    /* Global styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #121212;
      color: #fff;
      line-height: 1.6;
    }

    /* Header Section */
    .header {
      background-color: #1e1e1e;
      padding: 40px;
      text-align: center;
    }

    .header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    .header p {
      font-size: 1.2rem;
    }

    /* Featured Mods Section */
    .featured-mods {
      background-color: #2c2c2c;
      padding: 40px 0;
    }

    .featured-mods h2 {
      font-size: 2rem;
      text-align: center;
      margin-bottom: 20px;
    }

    .mod-cards {
      display: flex;
      justify-content: center;
      gap: 30px;
    }

    .mod-card {
      background-color: #3b3b3b;
      padding: 20px;
      text-align: center;
      border-radius: 10px;
      width: 200px;
    }

    .mod-card img {
      width: 100%;
      border-radius: 10px;
    }

    .mod-card p {
      margin-top: 10px;
    }

    .mod-card span {
      display: block;
      margin-top: 5px;
      color: #ffd700;
    }

    /* Limited Time Offer Section */
    .limited-time-offer {
      background-color: #ff6f61;
      text-align: center;
      padding: 30px 0;
    }

    .limited-time-offer h2 {
      font-size: 2rem;
    }

    .limited-time-offer p {
      font-size: 1.2rem;
      margin-top: 10px;
    }

    .countdown {
      margin-top: 20px;
      font-size: 2rem;
      font-weight: bold;
    }

    /* Download Section */
    .download-section {
      padding: 40px 0;
      text-align: center;
    }

    .download-btn {
      background-color: #28a745;
      color: white;
      padding: 15px 30px;
      font-size: 1.5rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .download-btn:hover {
      background-color: #218838;
    }

    /* Footer Section */
    .footer {
      background-color: #2c2c2c;
      padding: 20px;
      text-align: center;
    }
  </style>

  <!-- External JS -->
  <script>
    // Countdown Timer Functionality
    function updateCountdown() {
      const timerElement = document.getElementById('countdown-timer');
      let countdown = timerElement.innerText.split(":");
      let hours = parseInt(countdown[0]);
      let minutes = parseInt(countdown[1]);
      let seconds = parseInt(countdown[2]);

      if (seconds > 0) {
        seconds--;
      } else if (minutes > 0) {
        minutes--;
        seconds = 59;
      } else if (hours > 0) {
        hours--;
        minutes = 59;
        seconds = 59;
      }

      timerElement.innerText = `${String(hours).padStart(2, '0')}:${String(minutes).padStart(2, '0')}:${String(seconds).padStart(2, '0')}`;
    }

    // Update the countdown every second
    setInterval(updateCountdown, 1000);
  </script>
</head>
<body>
  <!-- Header Section -->
  <header class="header">
    <div class="container">
      <h1>ManyMods</h1>
      <p>Premium modded apps collection</p>
    </div>
  </header>

  <!-- Featured Mods Section -->
  <section class="featured-mods">
    <div class="container">
      <h2>Featured Mods</h2>
      <div class="mod-cards">
        <!-- Mod 1 -->
        <div class="mod-card">
          <img src="https://via.placeholder.com/150" alt="Red Dead Redemption">
          <p>Red Dead Redemption</p>
          <span>4.9 <i class="fas fa-star"></i></span>
        </div>
        <!-- Mod 2 -->
        <div class="mod-card">
          <img src="https://via.placeholder.com/150" alt="GTA 5 Mobile">
          <p>GTA 5 Mobile</p>
          <span>4.7 <i class="fas fa-star"></i></span>
        </div>
        <!-- Mod 3 -->
        <div class="mod-card">
          <img src="https://via.placeholder.com/150" alt="FC Mobile">
          <p>FC Mobile 25</p>
          <span>4.9 <i class="fas fa-star"></i></span>
        </div>
      </div>
    </div>
  </section>

  <!-- Limited Time Offer Section -->
  <section class="limited-time-offer">
    <div class="container">
      <h2>Limited Time Offer!</h2>
      <p>Get exclusive mod packs for free - Offer ends soon!</p>
      <div class="countdown">
        <span id="countdown-timer">23:59:59</span>
      </div>
    </div>
  </section>

  <!-- Download Button -->
  <section class="download-section">
    <div class="container">
      <h2>Download Your Favorite Mods Now!</h2>
      <button class="download-btn">Download Now</button>
    </div>
  </section>

  <!-- Footer Section -->
  <footer class="footer">
    <div class="container">
      <p>&copy; 2026 ManyMods. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>
