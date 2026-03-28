<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio Abdul Wakhid | Design Grafis & Editing Video</title>
  <meta name="description" content="Portfolio Abdul Wakhid, spesialis desain grafis dan editing video dari Indramayu, Jawa Barat. Menyediakan desain promosi, konten media sosial, banner, thumbnail, dan video edit." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>

    :root {
      --bg: #0f172a;
      --bg-soft: #111827;
      --card: rgba(255,255,255,0.08);
      --line: rgba(255,255,255,0.12);
      --text: #f8fafc;
      --muted: #cbd5e1;
      --primary: #38bdf8;
      --secondary: #a78bfa;
      --accent: #f59e0b;
      --success: #22c55e;
      --shadow: 0 20px 50px rgba(0,0,0,0.28);
      --radius: 24px;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      min-width: 0;
    }

    html {
      scroll-behavior: smooth;
      -webkit-text-size-adjust: 100%;
    }

    body {
      min-width: 320px;
      font-family: 'Poppins', sans-serif;
      background:
        radial-gradient(circle at top left, rgba(56,189,248,0.18), transparent 30%),
        radial-gradient(circle at top right, rgba(167,139,250,0.18), transparent 28%),
        linear-gradient(135deg, #020617 0%, #0f172a 48%, #111827 100%);
      color: var(--text);
      line-height: 1.7;
      overflow-x: hidden;
      word-wrap: break-word;
    }

    body.menu-open {
      overflow: hidden;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img,
    video,
    svg,
    canvas {
      max-width: 100%;
      height: auto;
      display: block;
    }

    section[id] {
      scroll-margin-top: 110px;
    }

    .container {
      width: min(1120px, calc(100% - 32px));
      margin: 0 auto;
    }

    .section {
      padding: clamp(64px, 8vw, 96px) 0;
    }

    .section-title {
      font-size: clamp(1.8rem, 3vw, 2.6rem);
      font-weight: 800;
      margin-bottom: 14px;
      line-height: 1.2;
    }

    .section-subtitle {
      color: var(--muted);
      max-width: 680px;
      margin-bottom: 38px;
      font-size: clamp(0.96rem, 1.4vw, 1rem);
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 10px 16px;
      border: 1px solid var(--line);
      background: rgba(255,255,255,0.06);
      border-radius: 999px;
      color: #e2e8f0;
      font-size: 0.92rem;
      backdrop-filter: blur(12px);
      max-width: 100%;
      flex-wrap: wrap;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(2,6,23,0.7);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }

    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
      min-height: 76px;
      position: relative;
    }

    .logo {
      font-size: 1.25rem;
      font-weight: 800;
      letter-spacing: 0.4px;
      flex-shrink: 0;
    }

    .logo span {
      color: var(--primary);
    }

    .nav-toggle {
      width: 46px;
      height: 46px;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 14px;
      background: rgba(255,255,255,0.04);
      display: none;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      gap: 5px;
      cursor: pointer;
      transition: 0.3s ease;
      margin-left: auto;
    }

    .nav-toggle:hover {
      background: rgba(255,255,255,0.1);
    }

    .nav-toggle span {
      width: 20px;
      height: 2px;
      background: #fff;
      border-radius: 999px;
      display: block;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 24px;
      flex-wrap: wrap;
      margin-left: auto;
    }

    .nav-links a {
      color: #e2e8f0;
      font-size: 0.96rem;
      transition: 0.3s ease;
      white-space: nowrap;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      padding: 14px 24px;
      border-radius: 14px;
      font-weight: 600;
      transition: 0.3s ease;
      border: none;
      cursor: pointer;
      text-align: center;
    }

    .btn-primary {
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      color: #fff;
      box-shadow: var(--shadow);
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      filter: brightness(1.06);
    }

    .btn-outline {
      border: 1px solid var(--line);
      color: #fff;
      background: rgba(255,255,255,0.04);
    }

    .btn-outline:hover {
      background: rgba(255,255,255,0.1);
    }

    .hero {
      min-height: min(920px, calc(100vh - 76px));
      display: flex;
      align-items: center;
      padding: clamp(40px, 6vw, 64px) 0 40px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(320px, 0.8fr);
      gap: clamp(24px, 4vw, 36px);
      align-items: center;
    }

    .hero h1 {
      font-size: clamp(2.3rem, 5vw, 4.5rem);
      line-height: 1.12;
      margin: 18px 0 18px;
      font-weight: 800;
    }

    .hero h1 span {
      background: linear-gradient(135deg, #7dd3fc, #c4b5fd);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      color: var(--muted);
      max-width: 62ch;
      font-size: clamp(0.98rem, 1.5vw, 1.02rem);
      margin-bottom: 28px;
    }

    .hero-actions {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
      margin-bottom: 28px;
    }

    .hero-highlights {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 16px;
    }

    .highlight-card,
    .glass-card {
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: clamp(18px, 4vw, var(--radius));
      backdrop-filter: blur(18px);
      box-shadow: var(--shadow);
    }

    .highlight-card {
      padding: 18px;
    }

    .highlight-card strong {
      display: block;
      font-size: 1.35rem;
      margin-bottom: 6px;
    }

    .highlight-card span {
      color: var(--muted);
      font-size: 0.92rem;
    }

    .profile-card {
      padding: clamp(22px, 3vw, 28px);
      position: relative;
      overflow: hidden;
      width: 100%;
    }

    .profile-card::before {
      content: '';
      position: absolute;
      width: 180px;
      height: 180px;
      top: -70px;
      right: -40px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(56,189,248,0.3), transparent 70%);
    }

    .avatar {
      width: clamp(112px, 25vw, 140px);
      height: clamp(112px, 25vw, 140px);
      border-radius: 50%;
      margin: 0 auto 20px;
      display: grid;
      place-items: center;
      font-size: clamp(2rem, 4vw, 2.4rem);
      font-weight: 800;
      color: #fff;
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      box-shadow: 0 16px 34px rgba(56,189,248,0.28);
      border: 4px solid rgba(255,255,255,0.14);
      overflow: hidden;
    }

    .avatar img {
      width: 100%;
      height: 120%;
      object-fit: cover;
      object-position: center top;
    }

    .profile-card h3 {
      text-align: center;
      font-size: 1.45rem;
      margin-bottom: 6px;
    }

    .profile-card .role {
      text-align: center;
      color: #cbd5e1;
      margin-bottom: 22px;
    }

    .bio-list {
      display: grid;
      gap: 12px;
    }

    .bio-item {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 12px;
      flex-wrap: wrap;
      padding: 12px 14px;
      border-radius: 14px;
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.08);
      font-size: 0.95rem;
    }

    .bio-item span:first-child {
      color: var(--muted);
      flex: 1 1 160px;
    }

    .bio-item span:last-child {
      flex: 1 1 220px;
      text-align: right;
    }

    .about-grid,
    .contact-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 28px;
    }

    .content-card {
      padding: clamp(22px, 3vw, 30px);
    }

    .content-card p {
      color: var(--muted);
      margin-bottom: 16px;
    }

    .tag-list,
    .service-list,
    .tool-list,
    .portfolio-grid,
    .experience-grid {
      display: grid;
      gap: 18px;
    }

    .tool-list,
    .service-list,
    .portfolio-grid,
    .experience-grid,
    .contact-grid.cards {
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    }

    .tool-item,
    .service-item,
    .experience-item,
    .portfolio-item,
    .contact-card {
      padding: 22px;
      border-radius: 22px;
      background: var(--card);
      border: 1px solid var(--line);
      backdrop-filter: blur(12px);
      transition: 0.3s ease;
    }

    .tool-item:hover,
    .service-item:hover,
    .experience-item:hover,
    .portfolio-item:hover,
    .contact-card:hover {
      transform: translateY(-4px);
      border-color: rgba(56,189,248,0.35);
    }

    .tool-item h4,
    .service-item h4,
    .experience-item h4,
    .portfolio-item h4,
    .contact-card h4 {
      font-size: 1.05rem;
      margin-bottom: 10px;
    }

    .tool-item p,
    .service-item p,
    .experience-item p,
    .portfolio-item p,
    .contact-card p,
    .contact-card a {
      color: var(--muted);
      font-size: 0.95rem;
      overflow-wrap: anywhere;
    }

    .portfolio-thumb {
      height: clamp(150px, 22vw, 180px);
      border-radius: 16px;
      margin-bottom: 18px;
      background:
        linear-gradient(135deg, rgba(56,189,248,0.2), rgba(167,139,250,0.22)),
        rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.08);
      display: grid;
      place-items: center;
      font-size: 0.95rem;
      color: #dbeafe;
      text-align: center;
      padding: 14px;
    }

    .experience-item .year {
      display: inline-block;
      margin-bottom: 12px;
      color: #fff;
      background: rgba(34,197,94,0.14);
      border: 1px solid rgba(34,197,94,0.24);
      padding: 8px 12px;
      border-radius: 999px;
      font-size: 0.84rem;
      font-weight: 600;
    }

    .cta {
      text-align: center;
      padding: clamp(24px, 4vw, 38px);
    }

    .cta p {
      color: var(--muted);
      max-width: 680px;
      margin: 14px auto 26px;
    }

    footer {
      padding: 28px 0 42px;
      border-top: 1px solid rgba(255,255,255,0.08);
      color: var(--muted);
      text-align: center;
    }

    .small-text {
      font-size: 0.92rem;
      color: var(--muted);
    }

    @media (max-width: 1024px) {
      .hero {
        min-height: auto;
      }

      .hero-grid,
      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .profile-card {
        max-width: 720px;
        margin: 0 auto;
      }
    }

    @media (max-width: 768px) {
      nav {
        min-height: 72px;
        padding: 12px 0;
      }

      .nav-toggle {
        display: inline-flex;
      }

      .nav-links {
        position: absolute;
        top: calc(100% + 10px);
        left: 0;
        right: 0;
        display: grid;
        gap: 8px;
        padding: 16px;
        background: rgba(2,6,23,0.96);
        border: 1px solid rgba(255,255,255,0.08);
        border-radius: 18px;
        box-shadow: var(--shadow);
        backdrop-filter: blur(16px);
        opacity: 0;
        pointer-events: none;
        transform: translateY(-8px);
        transition: 0.25s ease;
        margin-left: 0;
      }

      .nav-links[data-open="true"] {
        opacity: 1;
        pointer-events: auto;
        transform: translateY(0);
      }

      .nav-links a {
        padding: 12px 14px;
        border-radius: 12px;
        background: rgba(255,255,255,0.03);
      }

      .hero {
        padding-top: 32px;
      }

      .hero-actions .btn {
        width: 100%;
      }
    }

    @media (max-width: 520px) {
      .container {
        width: min(1120px, calc(100% - 24px));
      }

      .section-subtitle,
      .tool-item p,
      .service-item p,
      .experience-item p,
      .portfolio-item p,
      .contact-card p,
      .contact-card a,
      .hero p {
        font-size: 0.95rem;
      }

      .bio-item {
        padding: 12px;
      }

      .bio-item span:last-child {
        text-align: left;
        flex-basis: 100%;
      }

      .profile-card,
      .content-card,
      .tool-item,
      .service-item,
      .experience-item,
      .portfolio-item,
      .contact-card {
        padding: 18px;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      html {
        scroll-behavior: auto;
      }

      *,
      *::before,
      *::after {
        transition: none !important;
        animation: none !important;
      }
    }

  </style>
</head>
<body>
  <header>
    <div class="container">
      <nav>
        <a href="#home" class="logo">Abdul<span>Wakhid</span></a>
        <button class="nav-toggle" type="button" aria-label="Buka menu navigasi" aria-controls="nav-links" aria-expanded="false">
          <span></span>
          <span></span>
          <span></span>
        </button>
        <div class="nav-links" id="nav-links" data-open="false">
          <a href="#tentang">Tentang</a>
          <a href="#skill">Skill</a>
          <a href="#layanan">Layanan</a>
          <a href="#pengalaman">Pengalaman</a>
          <a href="#portfolio">Portfolio</a>
          <a href="#kontak">Kontak</a>
        </div>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container hero-grid">
        <div>
          <div class="badge">Design Grafis &amp; Editing Video • Siap Proyek Freelance</div>
          <h1>Halo, saya <span>Abdul Wakhid</span><br>Designer grafis dan editor video yang fokus pada visual rapi, kuat, dan enak dilihat.</h1>
          <p>
            Saya membantu pembuatan berbagai kebutuhan visual digital seperti poster, banner, feed media sosial, thumbnail, video promosi, dan konten singkat yang komunikatif serta menarik. Setiap desain saya kerjakan dengan pendekatan yang rapi, jelas, dan menyesuaikan kebutuhan brand maupun personal project.
          </p>
          <div class="hero-actions">
            <a href="#portfolio" class="btn btn-primary">Lihat Portfolio</a>
            <a href="https://wa.me/6285924063022" class="btn btn-outline" target="_blank" rel="noreferrer">Hubungi Saya</a>
          </div>
          <div class="hero-highlights">
            <div class="highlight-card">
              <strong>Desain Visual</strong>
              <span>Poster, banner, feed, thumbnail, dan materi promosi</span>
            </div>
            <div class="highlight-card">
              <strong>Video Editing</strong>
              <span>Konten pendek, video promosi, dan editing visual untuk media digital</span>
            </div>
            <div class="highlight-card">
              <strong>Siap Kolaborasi</strong>
              <span>Terbuka untuk kebutuhan personal, bisnis, organisasi, dan UMKM</span>
            </div>
          </div>
        </div>

        <div class="glass-card profile-card">
          <div class="avatar"><img src="Foto Biodata 2.jpg" alt="Abdul Wakhid"></div>
          <h3>Abdul Wakhid</h3>
          <div class="role">Design Grafis &amp; Editing Video</div>
          <div class="bio-list">
            <div class="bio-item"><span>Domisili</span><span>Indramayu, Jawa Barat</span></div>
            <div class="bio-item"><span>Email</span><span>Abdulwakhid017@gmail.com</span></div>
            <div class="bio-item"><span>WhatsApp</span><span>085924063022</span></div>
            <div class="bio-item"><span>Instagram</span><span>@AbdulWakhid_017</span></div>
            <div class="bio-item"><span>Status</span><span>Open Project &amp; Kolaborasi</span></div>
            <div class="bio-item"><span>Fokus</span><span>Desain promosi, konten media sosial, thumbnail, dan video edit</span></div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="tentang">
      <div class="container">
        <h2 class="section-title">Perkenalan & Biodata Diri</h2>
        <p class="section-subtitle">Ringkasan singkat tentang profil, fokus kerja, dan nilai yang saya tawarkan dalam setiap proyek desain maupun editing video.</p>

        <div class="about-grid">
          <div class="glass-card content-card">
            <h3 style="margin-bottom:16px; font-size:1.35rem;">Tentang Saya</h3>
            <p>
              Saya adalah desainer grafis dan editor video yang fokus pada tampilan visual yang rapi, komunikatif, dan sesuai tujuan. Saya senang membantu klien menghadirkan materi visual yang tidak hanya menarik, tetapi juga mudah dipahami.
            </p>
            <p>
              Saya terbiasa mengerjakan kebutuhan promosi digital seperti poster, banner, feed media sosial, thumbnail, dan video singkat. Setiap pekerjaan saya usahakan tetap konsisten secara visual agar hasil akhirnya terlihat profesional.
            </p>
            <p>
              Saya terbuka untuk proyek personal, usaha, organisasi, maupun kebutuhan branding sederhana. Prioritas saya adalah hasil yang enak dilihat, jelas pesannya, dan nyaman dipakai di berbagai platform.
            </p>
          </div>

          <div class="glass-card content-card">
            <h3 style="margin-bottom:16px; font-size:1.35rem;">Biodata Singkat</h3>
            <div class="bio-list">
              <div class="bio-item"><span>Nama Lengkap</span><span>Abdul Wakhid</span></div>
              <div class="bio-item"><span>Profesi</span><span>Design Grafis &amp; Editing Video</span></div>
              <div class="bio-item"><span>Domisili</span><span>Indramayu, Jawa Barat</span></div>
              <div class="bio-item"><span>Email</span><span>Abdulwakhid017@gmail.com</span></div>
              <div class="bio-item"><span>WhatsApp</span><span>085924063022</span></div>
              <div class="bio-item"><span>Spesialisasi</span><span>Desain promosi digital, konten sosial media, thumbnail, dan video edit</span></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="skill">
      <div class="container">
        <h2 class="section-title">Keahlian Utama</h2>
        <p class="section-subtitle">Beberapa jenis kemampuan utama yang saya tawarkan untuk membantu kebutuhan visual digital dan konten promosi.</p>

        <div class="tool-list">
          <div class="tool-item">
            <h4>Desain Poster</h4>
            <p>Membuat poster promosi yang kuat secara visual, rapi secara layout, dan jelas saat menyampaikan informasi utama.</p>
          </div>
          <div class="tool-item">
            <h4>Feed Media Sosial</h4>
            <p>Menyusun desain konten sosial media yang konsisten agar akun terlihat lebih profesional dan menarik.</p>
          </div>
          <div class="tool-item">
            <h4>Banner &amp; Publikasi</h4>
            <p>Mengerjakan banner kegiatan, materi publikasi, dan kebutuhan promosi digital maupun cetak dengan tampilan bersih.</p>
          </div>
          <div class="tool-item">
            <h4>Thumbnail Konten</h4>
            <p>Membuat thumbnail yang lebih menonjol, mudah dibaca, dan sesuai karakter konten video atau promosi.</p>
          </div>
          <div class="tool-item">
            <h4>Editing Video</h4>
            <p>Mengedit video singkat untuk reels, promosi produk, dokumentasi, maupun kebutuhan konten digital lainnya.</p>
          </div>
          <div class="tool-item">
            <h4>Visual Branding Sederhana</h4>
            <p>Membantu merapikan tampilan visual brand agar lebih serasi, konsisten, dan mudah dikenali di berbagai platform.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="layanan">
      <div class="container">
        <h2 class="section-title">Layanan yang Saya Terima</h2>
        <p class="section-subtitle">Saya menerima berbagai kebutuhan desain dan editing video untuk promosi, branding, maupun konten digital sehari-hari.</p>

        <div class="service-list">
          <div class="service-item">
            <h4>Poster Promosi</h4>
            <p>Desain poster untuk event, produk, jasa, atau publikasi kegiatan dengan tampilan yang jelas dan menarik.</p>
          </div>
          <div class="service-item">
            <h4>Banner Digital &amp; Cetak</h4>
            <p>Pembuatan banner untuk kebutuhan usaha, acara, organisasi, dan promosi visual lainnya.</p>
          </div>
          <div class="service-item">
            <h4>Feed Sosial Media</h4>
            <p>Desain feed yang konsisten untuk Instagram dan platform lain agar tampilan akun lebih profesional.</p>
          </div>
          <div class="service-item">
            <h4>Thumbnail Konten</h4>
            <p>Thumbnail video atau promosi yang lebih menonjol dan mudah menarik perhatian audiens.</p>
          </div>
          <div class="service-item">
            <h4>Editing Video Pendek</h4>
            <p>Editing reels, video promosi, video produk, dan potongan konten singkat untuk kebutuhan digital.</p>
          </div>
          <div class="service-item">
            <h4>Konten Visual Lainnya</h4>
            <p>Terbuka untuk kebutuhan desain lain sesuai brief, gaya visual, dan target penggunaan yang diinginkan.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="pengalaman">
      <div class="container">
        <h2 class="section-title">Fokus Pengerjaan</h2>
        <p class="section-subtitle">Beberapa area kerja utama yang menjadi fokus saya dalam membantu kebutuhan visual klien.</p>

        <div class="experience-grid">
          <div class="experience-item">
            <div class="year">Desain</div>
            <h4>Materi Promosi yang Rapi dan Menjual</h4>
            <p>Saya fokus membuat desain promosi yang enak dilihat, mudah dipahami, dan cocok dipakai untuk kebutuhan usaha maupun publikasi kegiatan.</p>
          </div>
          <div class="experience-item">
            <div class="year">Konten</div>
            <h4>Visual Sosial Media yang Konsisten</h4>
            <p>Saya membantu menyusun tampilan konten agar feed, poster, banner, dan thumbnail memiliki arah visual yang lebih serasi.</p>
          </div>
          <div class="experience-item">
            <div class="year">Video</div>
            <h4>Editing Singkat untuk Platform Digital</h4>
            <p>Saya juga menangani editing video pendek untuk kebutuhan reels, promosi, dokumentasi, dan konten visual yang butuh gerak lebih dinamis.</p>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="portfolio">
      <div class="container">
        <h2 class="section-title">Portfolio</h2>

        <div class="portfolio-grid">
          <a href="https://drive.google.com/drive/folders/14jNXuxP5M2eeybXTIup7TvoBJsQwfWjj?usp=sharing" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 01 • Poster Promosi</div>
            <h4>Poster Promosi Usaha</h4>
            <p>Contoh karya untuk kebutuhan promosi produk atau jasa dengan fokus pada headline yang kuat dan visual yang bersih.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1nBmiEFTEZcpIOhSavbxofdMmHDgTFMw7?usp=drive_link" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 02 • Feed Sosial Media</div>
            <h4>Feed Instagram Brand</h4>
            <p>Konsep feed yang konsisten untuk memperkuat tampilan akun dan membuat identitas visual terlihat lebih rapi.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1KvTAUYfGVBCzn5uJO_u94Waz_IByeP5T?usp=drive_link" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 03 • Banner</div>
            <h4>Banner Event atau Promosi</h4>
            <p>Desain banner yang informatif dan tetap menarik untuk kebutuhan acara, publikasi, atau promosi digital.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1OQJ_ecNrw81CM8fp7QS9OWQDFoMRCn60?usp=drive_link" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 04 • Thumbnail</div>
            <h4>Thumbnail Konten Video</h4>
            <p>Thumbnail dengan tampilan yang menonjol agar konten lebih mudah menarik perhatian saat tampil di platform digital.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1d4_HvQEN5h-f0imPHphTA2rYbxksEU6R?usp=drive_link" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 05 • Video Edit</div>
            <h4>Video Reels Promosi</h4>
            <p>Editing video singkat untuk kebutuhan promosi, highlight produk, atau potongan konten media sosial.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1TLE2iXTTDv3P4hdiIz-bR5szOsY3uiRt?usp=drive_link" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 06 • Highlight Video</div>
            <h4>Video Highlight Acara</h4>
            <p>Rangkuman visual acara atau dokumentasi singkat yang dibuat agar lebih hidup, ringkas, dan nyaman ditonton.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1XGgWefhg4y8mfsSO23_I_LT2nXbZizrN?usp=sharing" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 07 • Design Signage</div>
            <h4>Design Signage</h4>
            <p>Desain tanda, penanda ruang, dan signage untuk memberikan informasi dan petunjuk di ruang publik atau interior.</p>
          </a>
          <a href="https://drive.google.com/drive/folders/1g3NePHvMn_NtawU9fTe-7sUgPbGZvsYn?usp=sharing" target="_blank" rel="noreferrer" class="portfolio-item">
            <div class="portfolio-thumb">Project 08 • Design Piagam</div>
            <h4>Design Piagam</h4>
            <p>Desain piagam penghargaan atau sertifikat untuk menciptakan tampilan yang estetik dan profesional.</p>
          </a>
        </div>
      </div>
    </section>

    <section class="section" id="kontak">
      <div class="container">
        <div class="glass-card cta">
          <h2 class="section-title" style="margin-bottom:0;">Siap Bekerja Sama?</h2>
          <p>
            Saya terbuka untuk proyek desain grafis, editing video, maupun kolaborasi konten digital. Jika Anda membutuhkan visual yang rapi, menarik, dan komunikatif, silakan hubungi saya.
          </p>
          <a href="https://mail.google.com/mail/?view=cm&fs=1&to=abdulwakhid017@gmail.com" class="btn btn-primary" target="_blank" rel="noreferrer">Kirim Email</a>
        </div>

        <div class="section" style="padding-bottom:0;">
          <h2 class="section-title">Kontak</h2>
          <p class="section-subtitle">Hubungi saya melalui email, WhatsApp, atau Instagram untuk diskusi proyek dan kerja sama.</p>
          <div class="contact-grid cards">
            <div class="contact-card">
              <h4>Email</h4>
              <a href="mailto:Abdulwakhid017@gmail.com">Abdulwakhid017@gmail.com</a>
            </div>
            <div class="contact-card">
              <h4>WhatsApp</h4>
              <a href="https://wa.me/6285924063022" target="_blank" rel="noreferrer">085924063022</a>
            </div>
            <div class="contact-card">
              <h4>Instagram</h4>
              <a href="https://instagram.com/AbdulWakhid_017" target="_blank" rel="noreferrer">@AbdulWakhid_017</a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>© 2026 Abdul Wakhid • Portfolio Design Grafis &amp; Editing Video</p>
      <p class="small-text"> 
    </div>
  </footer>

  <script>
    document.addEventListener('DOMContentLoaded', function () {
      const toggle = document.querySelector('.nav-toggle');
      const navLinks = document.querySelector('.nav-links');

      if (!toggle || !navLinks) return;

      function closeMenu() {
        navLinks.setAttribute('data-open', 'false');
        toggle.setAttribute('aria-expanded', 'false');
        document.body.classList.remove('menu-open');
      }

      toggle.addEventListener('click', function () {
        const isOpen = navLinks.getAttribute('data-open') === 'true';
        navLinks.setAttribute('data-open', String(!isOpen));
        toggle.setAttribute('aria-expanded', String(!isOpen));
        document.body.classList.toggle('menu-open', !isOpen);
      });

      navLinks.querySelectorAll('a').forEach(function (link) {
        link.addEventListener('click', closeMenu);
      });

      window.addEventListener('resize', function () {
        if (window.innerWidth > 768) {
          closeMenu();
        }
      });
    });
  </script>

</body>
</html>
