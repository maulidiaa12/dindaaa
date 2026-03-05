<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dinda Maulidya | Portfolio</title>

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="style.css">
</head>
<body>

<header class="navbar">
    <h1 class="logo">Dnd.id</h1>
    <nav>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#portfolio">Portofolio</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

<section class="hero" id="home">
    <div class="hero-wrapper">

       <div class="hero-text">
    <h1 class="typing delay">Halo, Saya Dinda Maulidya</h1>
    <h2>Mahasiswi Sistem Informasi</h2>
        </div>

        <div class="lanyard">
            <div class="hero-image">
                <img src="foto12.jpeg" alt="Foto Dinda" class="profile">
            </div>
        </div>

    </div>
</section>

<section id="about" class="section">
    <div class="container">
        <h2 class="title">About Me</h2>

        <div class="about-grid">

            
            <div class="about-card">
                <h3>Deskripsi Diri</h3>
                <p>
                    Saya adalah mahasiswi Program Studi Sistem Informasi 
                    Universitas Muhammadiyah Sumatera Utara yang memiliki 
                    minat dalam pengembangan web dan sistem informasi. 
                    Saya memiliki sikap disiplin, bertanggung jawab, serta 
                    mampu bekerja secara individu maupun dalam tim.
                </p>
            </div>

            
            <div class="about-card">
                <h3>Pendidikan</h3>
                <ul class="edu-list">
                    <li>2010 - 2016 | SD Tamansiswa</li>
                    <li>2016 - 2019 | SMP Tamansiswa</li>
                    <li>2019 - 2022 | SMK Sandhy Putra 2 | Teknik Komputer dan Jaringan (TKJ)</li>
                    <li>2024 - Sekarang | S1 Sistem Informasi | Universitas Muhammadiyah Sumatera Utara</li>
                </ul>
            </div>

        
            <div class="about-card full">
                <h3>Hobi</h3>

                <ul class="hobby-list">
                    <li>Mendaki dan menikmati alam terbuka</li>
                    <li>Belajar hal baru yang bermanfaat</li>
                    <li>Hunting dan eksplorasi kuliner</li>
                    <li>Traveling untuk menambah wawasan</li>
                </ul>

                <div class="hobby-gallery">
                    <img src="Traveling.jpeg" alt="Traveling">
                    <img src="Kuliner.jpeg" alt="Kuliner">
                </div>

            </div>

        </div>
    </div>
</section>

<section id="portfolio" class="section">
  <div class="container">

    <h2 class="title">My Portfolio</h2>

    <div class="grid">

      <div class="card">
        <img src="menu1.png" alt="Website Menu Warung">
        <h3>Website Menu Warung Nasi Goreng</h3>
        <p>
          Website sederhana yang menampilkan menu makanan seperti 
          Nasi Goreng, Mie Goreng, Mie Tiaw, Ifumie, dan Capcay 
          dengan tampilan menarik menggunakan HTML dan CSS.
        </p>
        <a href="https://github.com/maulidiaa12/dindaaa" target="_blank">
          Lihat di GitHub
        </a>
      </div>

    </div>

  </div>
</section>

<section id="skills" class="section">
  <div class="container">
    <h2 class="title">Skills</h2>

    <div class="grid">

      <div class="skill-card">
        <div class="skill-card__icon">💻</div>
        <h3>HTML & CSS</h3>
        <p>Responsive layout dan modern design.</p>
      </div>

      <div class="skill-card">
        <div class="skill-card__icon">⚡</div>
        <h3>JavaScript Dasar</h3>
        <p>Interaktif dan dinamis.</p>
      </div>

      <div class="skill-card">
        <div class="skill-card__icon">🗄️</div>
        <h3>Database Dasar</h3>
        <p>Design, implementation, dan manajemen database.</p>
      </div>

    </div>
  </div>
</section>

<section id="contact" class="section">
    <div class="container">
        <h2 class="title">Contact</h2>

        <div class="contact-wrapper">

            <div class="contact-info card">

                <div class="contact-item">
                    <div class="contact-icon">📧</div>
                    <div>
                        <h3>Email</h3>
                        <p>maulidiad82@gmail.com</p>
                    </div>
                </div>

                <div class="contact-item">
                    <div class="contact-icon">📱</div>
                    <div>
                        <h3>No Telepon</h3>
                        <p>089613905022</p>
                    </div>
                </div>

            </div>

            <div class="contact-form card">
                <h3>Kirim Pesan</h3>

                <form>
                    <input type="text" placeholder="Nama Anda" required>
                    <input type="email" placeholder="Email Anda" required>
                    <textarea placeholder="Pesan Anda..." rows="4"></textarea>

                    <button type="submit" class="contact-btn">
                        Kirim Pesan
                    </button>
                </form>

            </div>

        </div>
    </div>
</section>

<footer>
    <p>© 2026 Dinda Maulidya</p>
</footer>

<script>
const farm = document.getElementById("farm");
const coinText = document.getElementById("coin");
let coins = 0;

for (let i = 0; i < 9; i++) {
    const plot = document.createElement("div");
    plot.classList.add("plot");
    plot.onclick = function() {
        if (!plot.classList.contains("grown")) {
            plot.classList.add("grown");
        } else {
            coins += 10;
            coinText.textContent = coins;
            plot.classList.remove("grown");
        }
    };
    farm.appendChild(plot);
}

function resetFarm() {
    coins = 0;
    coinText.textContent = coins;
    document.querySelectorAll(".plot").forEach(p => p.classList.remove("grown"));
}
</script>

</body>
</html>
