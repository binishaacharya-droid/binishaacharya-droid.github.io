<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>The Bini's | Binisha Acharya</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet" />

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Poppins", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: #f5f1ee;
      color: #222;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      display: block;
      max-width: 100%;
    }

    .page {
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 16px 50px 16px;
    }

    /* ---------- NAVBAR ---------- */
    header {
      background: #ffffff;
      border-bottom: 1px solid #e1dedb;
      box-shadow: 0 4px 12px rgba(0,0,0,0.04);
    }

    .nav {
      max-width: 1100px;
      margin: 0 auto;
    padding: 4px 16px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
    }

    .nav-left {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .nav-pill {
      padding: 6px 10px;
      border-radius: 999px;
      background: #b36b76;
      color: #fff;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
    }
/* Make each form row vertical: label on top, input/textarea under it */
.contact-card form > div {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

    .nav-brand {
      font-family: "Great Vibes", cursive;
      font-size: 5rem;
      color: #b36b76;
      white-space: nowrap;
    }

    .nav-right a {
      padding: 6px 14px;
      margin-left: 8px;
      font-size: 0.9rem;
      border-radius: 20px;
      background: #f5f5f5;
      border: 1px solid #dfdbd8;
      transition: 0.16s;
    }

    .nav-right a:hover {
      background: #b36b76;
      color: #fff;
      border-color: #b36b76;
      box-shadow: 0 6px 14px rgba(179, 107, 118, 0.4);
    }

    @media (max-width: 650px) {
      .nav {
        flex-direction: column;
        align-items: flex-start;
      }
      .nav-right a {
        margin-left: 0;
      }
    }

    /* ---------- HERO ---------- */
    .hero {
      margin-top: 0;
    }

    .hero-top {
      background: #A97881; /* dusty pink */
      min-height: 350px;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    .hero-photo {
      position: relative;
      z-index: 2;
    }

    .hero-photo img {
      max-height: 900px;
      object-fit: contain;
    }

    .hero-name {
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      bottom: 40px;
      font-size: clamp(2.3rem, 3.3vw, 3.2rem);
      font-weight: 700;
      color: #ffffff;
      letter-spacing: 0.05em;
      text-shadow:
        4px 4px 0 #000000;
    }
/* Make each form row vertical: label on top, box under it */
.contact-card form div {
  display: flex !important;
  flex-direction: column !important;
  align-items: flex-start;
}

/* Make labels actually sit above */
.contact-card form label {
  display: block;
  margin-bottom: 4px;
}

/* Make inputs + textarea fill the width */
.contact-card form input,
.contact-card form textarea {
  width: 100%;
}

    .hero-signature {
      position: absolute;
      right: 40px;
      bottom: 20px;
      font-family: "Great Vibes", cursive;
      font-size: 2rem;
      color: #fbe9e8;
      opacity: 0.9;
    }

    .hero-bottom {
      background: #ffffff;
      padding: 26px 20px 28px 20px;
      border-bottom-left-radius: 30px;
      border-bottom-right-radius: 30px;
      box-shadow: 0 26px 60px rgba(0,0,0,0.18);
    }

    .hero-bottom-inner {
      display: grid;
      grid-template-columns: minmax(0, 2.2fr) minmax(0, 1.8fr);
      gap: 18px;
    }

    @media (max-width: 800px) {
      .hero-bottom-inner {
        grid-template-columns: 1fr;
      }
    }

    .hero-heading {
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: #8e7a7c;
      margin-bottom: 8px;
    }

    .hero-text {
      font-size: 0.95rem;
      color: #3b3031;
      line-height: 1.8;
    }

    .hero-text span {
      font-style: italic;
      color: #8c525e;
    }

    .hero-favs {
      font-size: 0.9rem;
      color: #7d6668;
      line-height: 1.7;
      background: #f9f0ec;
      border-radius: 18px;
      border: 1px solid #e2d2cd;
      padding: 12px 14px;
    }

    /* ---------- GENERIC SECTION STYLES ---------- */
    main {
      margin-top: 50px;
    }

    section {
      margin-bottom: 60px;
    }

    .section-label {
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: #8e7a7c;
      margin-bottom: 6px;
    }

    .section-title {
      font-size: 1.8rem;
      margin-bottom: 10px;
      color: #37282a;
    }

    .section-intro {
      font-size: 0.95rem;
      color: #7c6a6d;
      max-width: 640px;
      line-height: 1.8;
      margin-bottom: 18px;
    }

    .card-row {
      display: grid;
      grid-template-columns: minmax(0, 1.7fr) minmax(0, 1.3fr);
      gap: 18px;
    }

    @media (max-width: 800px) {
      .card-row {
        grid-template-columns: 1fr;
      }
    }

    .card {
      background: #ffffff;
      border-radius: 20px;
      padding: 18px 18px 16px 18px;
      border: 1px solid #e2d2cd;
      box-shadow: 0 20px 40px rgba(0,0,0,0.06);
      font-size: 0.9rem;
      color: #7c686a;
      line-height: 1.8;
    }

    .pill-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 10px;
    }

    .pill {
      font-size: 0.78rem;
      padding: 5px 10px;
      border-radius: 999px;
      border: 1px solid #e2d2cd;
      background: #f9f0ec;
      color: #7c686a;
    }

    /* BLOG CARDS */
    .blog-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 16px;
    }

    @media (max-width: 900px) {
      .blog-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }

    @media (max-width: 620px) {
      .blog-grid {
        grid-template-columns: 1fr;
      }
    }

    .post {
      background: #ffffff;
      border-radius: 18px;
      padding: 14px 14px 12px 14px;
      border: 1px solid #e2d2cd;
      box-shadow: 0 18px 34px rgba(0,0,0,0.05);
      transition: 0.15s;
    }

    .post:hover {
      transform: translateY(-3px);
      box-shadow: 0 22px 42px rgba(0,0,0,0.08);
    }

    .post-tag {
      font-size: 0.72rem;
      text-transform: uppercase;
      letter-spacing: 0.14em;
      color: #8e7a7c;
    }

    .post-title {
      font-size: 1rem;
      margin: 4px 0;
      color: #3b262a;
      font-weight: 600;
    }

    .post-text {
      font-size: 0.86rem;
      color: #7c686a;
      line-height: 1.7;
    }

    /* CONTACT */
    .contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr; /* two equal columns */
  align-items: start;
  gap: 20px;
}

    @media (max-width: 800px) {
      .contact-grid {
        grid-template-columns: 1fr;
      }
    }

    .contact-card {
      background: #ffffff;
      border-radius: 20px;
      border: 1px solid #e2d2cd;
      padding: 18px 18px 16px 18px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.06);
      font-size: 0.9rem;
      color: #7c686a;
      line-height: 1.8;
    }

    form {
      margin-top: 8px;
      display: flex;
      flex-direction: column;
      gap: 9px;
      font-size: 0.86rem;
    }

    label {
      font-weight: 500;
      margin-bottom: 2px;
    }

    input, textarea {
      border-radius: 14px;
      border: 1px solid #e2d2cd;
      padding: 8px 11px;
      font: inherit;
      background: #fdf7f2;
      resize: vertical;
    }

    input:focus, textarea:focus {
      outline: none;
      border-color: #b36b76;
      box-shadow: 0 0 0 2px rgba(179, 107, 118, 0.25);
    }

    textarea {
      min-height: 90px;
    }

    .btn {
      align-self: flex-start;
      margin-top: 4px;
      padding: 8px 18px;
      border-radius: 999px;
      border: none;
      background: linear-gradient(135deg, #f3c0c8, #b36b76);
      color: #fff;
      font-size: 0.86rem;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 14px 32px rgba(179, 107, 118, 0.55);
      transition: 0.16s;
    }

    .btn:hover {
      transform: translateY(-1px);
      box-shadow: 0 18px 42px rgba(179, 107, 118, 0.7);
    }

    footer {
      margin-top: 20px;
      padding-top: 10px;
      border-top: 1px solid #e2d2cd;
      font-size: 0.78rem;
      color: #8e7a7c;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 6px;
    }
    .contact-grid-fixed {
  display: grid !important;
  grid-template-columns: 1fr 1fr !important;
  gap: 30px;
  align-items: flex-start;
  margin-top: 20px;
}

@media (max-width: 800px) {
  .contact-grid-fixed {
    grid-template-columns: 1fr !important;
  }
}

  </style>
</head>

<body>
  <!-- NAVBAR -->
  <header>
    <div class="nav">
      <div class="nav-left">
        <div class="nav-brand">The Bini's</div>
      </div>
      <nav class="nav-right">
        <a href="#home">Home</a>
        <a href="#about">About me</a>
        <a href="#blog">Blog</a>
        <a href="#contact">Contact me</a>
      </nav>
    </div>
  </header>

  <div class="page">
    <!-- HERO -->
    <section id="home" class="hero">
      <div class="hero-top">
        <div class="hero-photo">
          <!-- 🔻🔻 REPLACE IMAGE_URL_HERE WITH YOUR IMAGE LINK 🔻🔻 -->
          <img
            src="binisha pic.jpg"
            alt="Binisha on stage"
          />
          <!-- 🔺🔺 ONLY CHANGE THE src ABOVE, NOTHING ELSE 🔺🔺 -->
        </div>
      </div>

      <div class="hero-bottom">
        <div class="hero-bottom-inner">
          <div>
            <div class="hero-heading">Introduction</div>
            <p class="hero-text">I’m Binisha. I like building things like melodies, ideas, small experiments, and moments that feel warm.
I’m not defined by one label, I move between music, art, coding, and anything that teaches me something new.
              <span>a jack of all trades.. master of none</span>,
              but often times better than master of one.
            </p>
          </div>
          <div class="hero-favs">
            <strong>Things that feel like home:</strong><br/>
            I love coffee,  me-time, the cozy feeling of autumn, and a playlist playing in the background.
          </div>
        </div>
      </div>
    </section>

    <main>
      <!-- ABOUT -->
      <section id="about">
        <div class="section-label">About me</div>
        <h2 class="section-title">More than just one label.</h2>
        <p class="section-intro">
          I’m not just “the girl who sings” or “the one who codes”.
          I live somewhere between music, art, slideshows, and random experiments.
          This is the part where all of those pieces come together.
        </p>

        <div class="card-row">
          <div class="card">
            I’m the kind of person who will learn a new song on guitar,
            sketch something half-finished, open a coding project,
            and design a dramatic PowerPoint, all in the same week.
            I don’t fit into one neat box, and I like it that way.
            Trying different things keeps life fun.
            <div class="pill-row">
             <span class="pill">music</span>
             <span class="pill">reading</span>
             <span class="pill">art</span>
             <span class="pill">coding</span>
             <span class="pill">design</span>
             <span class="pill">writing</span>
             <span class="pill">learning</span>
            </div>
          </div>
          <div class="card">
            I’m happiest in cozy spaces: a mug of coffee, headphones on,
            autumn outside the window, and something creative open in front of me.
            I love soft aesthetics, warm tones, and anything that feels like
            comfort and growth at the same time.
            <div class="pill-row">
              <span class="pill">coffee moments</span>
              <span class="pill">me-time</span>
              <span class="pill">autumn vibes</span>
              <span class="pill">soft aesthetics</span>
            </div>
          </div>
        </div>
      </section>

      <!-- BLOG -->
      <section id="blog">
        <div class="section-label">Blog</div>
        <h2 class="section-title">Future posts from The Bini's.</h2>
        <p class="section-intro">
          These are placeholders for now — titles and ideas for the kind of
          things I might write about when I turn my thoughts into real blog posts.
        </p>

        <div class="blog-grid">
          <article class="post">
            <div class="post-tag">music</div>
            <div class="post-title">Guitar strings & late-night thoughts</div>
            <p class="post-text">
              About how music keeps me grounded, the songs that feel like
              home, and the calm that comes when everyone else is asleep.
            </p>
          </article>

          <article class="post">
            <div class="post-tag">life</div>
            <div class="post-title">Being a jack of all trades</div>
            <p class="post-text">
              Why I love trying different things, learning in every direction,
              and not limiting myself to just one talent or path.
            </p>
          </article>

          <article class="post">
            <div class="post-tag">aesthetic</div>
            <div class="post-title">Coffee, autumn, and cozy playlists</div>
            <p class="post-text">
              Romanticising the small rituals: first sip of coffee, layered
              outfits, and playlists that make life feel like a movie.
            </p>
          </article>
        </div>
      </section>

      <!-- CONTACT -->
      <section id="contact">
        <section id="contact">
  <div class="section-label">Contact</div>
  <h2 class="section-title">Say hi to The Bini's.</h2>
  <p class="section-intro">
    Whether it’s a sweet message, a collab idea, or just “this feels like me too”,
    you’re always welcome to reach out.
  </p>

  <!-- FIXED HORIZONTAL GRID -->
  <div class="contact-grid-fixed">

    <!-- LEFT CARD -->
    <div class="contact-card">
      <strong>Email:</strong><br/>
      <a href="mailto:binishaacharya602@gmail.com">binishaacharya602@gmail.com</a>

      <p style="margin-top:8px;">You can also connect with me on social media.</p>

      <p style="margin-top:10px; font-size:0.85rem; color:#7c686a;">
        Instagram and TikTok are currently inactive.<br>
        You can still contact me on WhatsApp or email.
      </p>

      <div class="pill-row" style="margin-top:10px;">
        <a class="pill" href="https://instagram.com/thebinishae" target="_blank">Instagram</a>
        <a class="pill" href="https://www.tiktok.com/@binishaa_2" target="_blank">TikTok</a>
        <a class="pill" href="https://wa.me/9842564406" target="_blank">WhatsApp</a>
      </div>
    </div>

    <!-- RIGHT CARD (FORM) -->
    <div class="contact-card">
      <strong>Send me a message</strong>

      <form action="https://formsubmit.co/binishaacharya602@gmail.com" method="POST">
        <input type="hidden" name="_captcha" value="false">
        <input type="hidden" name="_next" value="https://binishaacharya-droid.github.io/">

        <div>
          <label for="name">Name</label>
          <input id="name" name="name" type="text" placeholder="Your name" required />
        </div>

        <div>
          <label for="emailInput">Email</label>
          <input id="emailInput" name="email" type="email" placeholder="your@email.com" required />
        </div>

        <div>
          <div>
  <label for="message">Message</label>
  <textarea
    id="message"
    name="message"
    placeholder="Type Something"
    required
  ></textarea>

</div>

        <button type="submit" class="btn">Send</button>
      </form>
    </div>

  </div>
</section>

      </section>
    </main>

    <footer>
      <span>© 2025 The Bini's — Binisha Acharya.</span>
      <span>Designed by me • Hosted on GitHub Pages</span>
    </footer>
  </div>
</body>
</html>
