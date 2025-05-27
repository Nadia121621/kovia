<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kopi Hitam Sehat</title>
  <style>
    /* ========================== */
/* Reset dasar dan font family */
/* ========================== */
body, html {
  margin: 0;
  padding: 0;
  font-family: 'Helvetica Neue', sans-serif;
  color: #333;
  line-height: 1.6;
  background-color: #f9f9f9;
}

/* ========================== */
/* Header styling */
/* ========================== */
header {
  background-color: #6f4e37;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 40px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

header .logo {
  display: flex;
  align-items: center;
  background-color: transparent;
  padding: 5px 10px;
  border-radius: 8px;
  transition: background-color 0.3s ease;
}

header .logo:hover {
  background-color: rgba(255, 255, 255, 0.1);
}

header .logo img {
  width: 80px;
  margin-right: 10px;
  border-radius: 8px;
  object-fit: contain;
  background-color: transparent;
  display: block;
}

header .logo h1 {
  font-size: 1.5rem;
  font-weight: normal;
  margin: 0;
  color: #f3e9dc;
  user-select: none;
}

header nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
  margin: 0;
  padding: 0;
}

header nav ul li {
  display: inline;
}

header nav ul li a {
  text-decoration: none;
  color: #f3e9dc;
  font-weight: 500;
  transition: color 0.3s;
}

header nav ul li a:hover {
  color: #d2b48c;
}

/* ========================== */
/* Call to Action Buttons */
/* ========================== */
.cta-buttons {
  margin-top: 20px;
}

.cta-buttons a {
  display: inline-block;
  background-color: #a0522d;
  color: #fff;
  padding: 10px 20px;
  text-decoration: none;
  margin: 5px;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.cta-buttons a:hover {
  background-color: #8b4513;
}

/* ========================== */
/* Sections styling */
/* ========================== */
section, #tips {
  padding: 60px 20px;
  text-align: center;
  background-color: #fff;
  margin: 20px auto;
  max-width: 900px;
  border-radius: 10px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  color: #5a3e28;
  font-family: 'Helvetica Neue', sans-serif;
}

section h2, #tips h2 {
  font-size: 2rem;
  margin-bottom: 20px;
  color: #a0522d;
  text-shadow: 1px 1px 2px #3e2f1c;
}

section p, #tips ul li {
  font-size: 1rem;
  color: #6f4e37;
  line-height: 1.6;
}

section img {
  width: 100%;
  max-width: 500px;
  border-radius: 8px;
  margin: 15px 0;
  display: block;
  margin-left: auto;
  margin-right: auto;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

/* Features styling */
.features {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.feature {
  background-color: #f5f5f5;
  padding: 20px;
  flex: 1 1 250px;
  border-radius: 8px;
  transition: transform 0.3s ease;
}

.feature:hover {
  transform: translateY(-5px);
}

.feature h3 {
  margin-top: 0;
  color: #a0522d;
}

.feature p {
  font-size: 0.9rem;
  color: #555;
}

/* Tentang kami */
#tentang-kami {
  text-align: center;
}

#tentang-kami img {
  max-width: 300px;
  width: 100%;
  height: auto;
  margin: 15px auto;
  display: block;
}

.features {
  display: grid;
  grid-template-columns: 1fr 1fr;  /* 2 kolom untuk 2 gambar di baris atas */
  grid-template-rows: auto auto;   /* 2 baris */
  grid-gap: 20px;
  max-width: 700px;
  margin: 0 auto;
  justify-items: center;  /* Tengahin isi tiap grid item */
}

/* Gambar ketiga di baris bawah dan posisinya di tengah */
.features .feature:nth-child(3) {
  grid-column: 1 / -1;   /* Membentang 2 kolom */
  justify-self: center;
  max-width: 300px;
}

/* Gambar produk */
.feature img {
  width: 100%;
  max-width: 250px;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  object-fit: contain;
  display: block;
}

/* Deskripsi produk di bawah features */
.product-description {
  max-width: 700px;
  margin: 30px auto 0;
  padding: 0 15px;
  color: #5a3e28;
  text-align: center;
  font-family: 'Helvetica Neue', sans-serif;
}

.product-description h3 {
  color: #a0522d;
  margin-bottom: 10px;
}

.product-description p {
  font-size: 1rem;
  line-height: 1.6;
  color: #6f4e37;
}

/* Tips section styling */
#tips {
  background-color: #f5f5f5;
  padding: 40px 20px;
  border-radius: 10px;
  max-width: 900px;
  margin: 40px auto;
  box-shadow: 0 4px 12px rgba(0,0,0,0.3);
  text-align: left;
}

#tips h2 {
  text-align: center;
  font-size: 2.4rem;
  margin-bottom: 25px;
}

#tips ul {
  list-style: none;
  padding-left: 0;
  max-width: 700px;
  margin: 0 auto;
}

#tips ul li {
  position: relative;
  padding-left: 35px;
  margin-bottom: 18px;
  font-size: 1.2rem;
  line-height: 1.5;
  border-left: 5px solid #d2b48c;
  background: #825c3b22;
  border-radius: 5px;
  transition: background-color 0.3s ease;
  cursor: default;
  color: #6f4e37;
}

#tips ul li::before {
  content: "☕";
  position: absolute;
  left: 10px;
  top: 50%;
  transform: translateY(-50%);
  color: #d2b48c;
  font-size: 1.3rem;
}

#tips ul li:hover {
  background-color: #d2b48c44;
  border-left-color: #a0522d;
  color: #5a3e28;
}

/* Links in section */
section a, #tips a {
  color: #a0522d;
  text-decoration: underline;
}

section a:hover, #tips a:hover {
  color: #6f4e37;
}

.cta-buttons {
  display: inline-block;
  padding: 12px 20px;
  background-color: #25D366; /* Hijau WhatsApp */
  color: white;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s;
  font-weight: bold;
}

.cta-buttons:hover {
  background-color: #1ebe57;
}



/* ========================== */
/* Footer styling */
/* ========================== */
footer {
  background-color: #222;
  color: #ccc;
  text-align: center;
  padding: 20px 10px;
}

footer p {
  margin: 0;
  font-size: 0.9rem;
}

/* ========================== */
/* Responsive styling */
/* ========================== */
@media (max-width: 768px) {
  header h1 {
    font-size: 2rem;
  }

  section, #tips {
    padding: 40px 10px;
  }

  .feature {
    flex: 1 1 100%;
  }

  #tips ul li {
    font-size: 1rem;
  }
}

/* ========================== */
/* Fade-in efek gambar */
/* ========================== */
.fade-in {
  opacity: 0;
  transform: translateY(20px);
  transition: opacity 0.8s ease, transform 0.8s ease;
}

.fade-in.visible {
  opacity: 1;
  transform: translateY(0);
}

  </style>
  <link rel="icon" type="image/png" href="img/logo.jpg" /> <!-- Ini untuk favicon -->
</head>
<body>


<header>
  <div class="logo">
    <img src="img/logo.jpg" alt="Logo">
  </div>
  <nav>
  <ul>
    <li><a href="test.html">Beranda</a></li> <!-- tetap link ke beranda -->
    <li><a href="#tentang-kami">Tentang Kami</a></li> <!-- scroll ke section tentang kami -->
    <li><a href="#produk">Produk</a></li>           <!-- scroll ke section produk -->
    <li><a href="#tips">Tips</a></li>               <!-- scroll ke section tips -->
    <li><a href="#kontak">Kontak</a></li>           <!-- scroll ke section kontak -->
  </ul>
</nav>
</header>


<section id="tentang-kami">
  <h2>Tentang Kami</h2>
  <p>Kovia Coffee Dip lahir pada awal 2025 dari keinginan tim pecinta kopi untuk menghadirkan kopi hitam celup rendah kalori dengan pemanis stevia, sebagai alternatif sehat tanpa mengorbankan 
    cita rasa kopi tradisional Indonesia. Setelah riset sederhana menunjukkan tingginya minat masyarakat akan kopi sehat, Kovia 
    berkomitmen menjadi pelopor kopi celup rendah kalori dan simbol gaya hidup sehat bagi penikmat kopi di Indonesia.</p>
  <img src="img/kopi.jpg" alt="Gambar 1" class="fade-in" width="300">
  <img src="img/stevia.jpg" alt="Gambar 2" class="fade-in" width="300">
  <img src="img/kopi2.jpg" alt="Gambar 3" class="fade-in" width="300">
</section>


<section>
  <h2>Mengapa Kovia Didirikan?</h2>
  <div class="features">
    <div class="feature">
      <h3>Obesitas</h3>
      <p>Konsumsi gula tinggi memicu obesitas</p>
    </div>
    <div class="feature">
      <h3>Diabetes Tipe 2</h3>
      <p>Risiko meningkat karena resistensi insulin</p>
    </div>
    <div class="feature">
      <h3>Kurangnya Cita Rasa</h3>
      <p>Kovia menjaga rasa kopi tradisional dengan standar profesional</p>
    </div>
  </div>
</section>

<section>
  <h2>Mengapa Memilih Kovia?</h2>
  <div class="features">
    <div class="feature">Rendah Kalori</div>
    <div class="feature">Menggunakan Stevia Alami</div>
    <div class="feature">Rasa Kopi Otentik</div>
  </div>
</section>

<section id="produk">
  <h2>Produk Kami</h2>
  <div class="features">
    <div class="feature">
      <img src="img/gambarpro_3.jpg" alt="Produk 1">
    </div>
    <div class="feature">
      <img src="img/gambarpro_1.jpg" alt="Produk 2">
    </div>
    <div class="feature">
      <img src="img/gambarpro_2.jpg" alt="Produk 3">
    </div>
  </div>
  <div class="product-description">
    <h3>Kopi Hitam Kovia</h3>
    <p>Kovia hadir sebagai jawaban bagi pecinta kopi hitam yang peduli kesehatan dengan menyediakan 
       kopi hitam rendah kalori menggunakan pemanis alami stevia. Produk utama Kovia adalah kopi hitam dengan 
       merek yang diracik khusus untuk memberikan kenikmatan rasa kopi otentik tanpa mengorbankan kesehatan.</p>
  </div>
</section>


<!-- Section Tips ditambahkan di sini -->
<section id="tips">
  <h2>Tips Menikmati Kopi Sehat</h2>
  <ul>
    <li>Minumlah kopi secara teratur tapi dalam porsi yang wajar untuk menjaga keseimbangan kesehatan.</li>
    <li>Gunakan stevia alami sebagai pemanis agar kalori tetap rendah dan aman bagi penderita diabetes.</li>
    <li>Hindari menambahkan gula pasir atau krimer berlebih untuk menjaga rasa asli kopi hitam.</li>
    <li>Minum air putih yang cukup untuk menjaga hidrasi tubuh saat menikmati kopi.</li>
    <li>Sajikan kopi pada waktu yang tepat, hindari konsumsi terlalu malam agar tidak mengganggu tidur.</li>
  </ul>
</section>

<!-- Tambahkan ini di <head> untuk link Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<section id="kontak" style="text-align: center;">
  <h2>Hubungi Kami</h2>
  <a class="cta-buttons" href="https://wa.me/6285601977410?text=Halo%20admin,%20saya%20tertarik%20dengan%20Kovia!" target="_blank">Chat Admin via WhatsApp</a>

  <div class="info-kontak">
    <p><strong>Alamat:</strong><br>
      Dusun Tanjungsari Rt 03, Rw 01<br>
      Desa Kuwolu, Kec. Bululawang<br>
      Malang, Jawa Timur, Indonesia, 65171
    </p>
    <p>Email: <a href="mailto:koviacoffeedip@gmail.com">koviacoffeedip@gmail.com</a></p>
  </div>

  <div class="sosial-media">
    <a href="https://www.instagram.com/koviacoffeedip31?igsh=NGVxOXUwNW9obnZl" target="_blank" class="instagram">
      <i class="fab fa-instagram"></i>
    </a>
    <a href="https://www.tiktok.com/@kovia.coffee.dip?_t=ZS-8whYogBbfpx&_r=1" target="_blank" class="tiktok">
      <i class="fab fa-tiktok"></i>
    </a>
    <a href="https://www.youtube.com/@kovia" target="_blank" class="youtube">
      <i class="fab fa-youtube"></i>
    </a>
  </div>
</section>


<script>
  document.addEventListener("DOMContentLoaded", function() {
    const images = document.querySelectorAll(".fade-in");

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if(entry.isIntersecting){
          entry.target.classList.add("visible");
        } else {
          entry.target.classList.remove("visible");
        }
      });
    }, {
      threshold: 0.1 // Muncul saat 10% terlihat
    });

    images.forEach(img => {
      observer.observe(img);
    });
  });
</script>


<footer>
  <p>&copy; 2025 Kovia. All Rights Reserved.</p>
</footer>


</body>
</html>
