<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SOS Fibre Optique | Technicien Télécom</title>
  <meta name="description" content="SOS Fibre Optique intervient dans les départements 72, 53, 28, 41, 61, 37 et 49. Réparation des gaines bouchées ou écrasées, remise en conformité après échec de raccordement et dépannage fibre." />
  <style>
    :root{
      --bg:#04101d;
      --bg2:#071a31;
      --card:rgba(10, 22, 40, .72);
      --stroke:rgba(255,255,255,.10);
      --text:#eff6ff;
      --muted:#a6bdd8;
      --blue:#18a4ff;
      --cyan:#3bd6ff;
      --green:#2de3a5;
      --shadow:0 24px 70px rgba(0,0,0,.38);
      --radius:28px;
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family:Arial, Helvetica, sans-serif;
      color:var(--text);
      background:
        radial-gradient(circle at 15% 10%, rgba(24,164,255,.16), transparent 30%),
        radial-gradient(circle at 85% 0%, rgba(59,214,255,.13), transparent 24%),
        linear-gradient(180deg, var(--bg) 0%, var(--bg2) 100%);
      min-height:100vh;
    }

    a{color:inherit;text-decoration:none}
    .container{
      width:min(1180px, calc(100% - 32px));
      margin:0 auto;
    }

    header{
      position:sticky;
      top:0;
      z-index:40;
      background:rgba(4,16,29,.78);
      backdrop-filter:blur(16px);
      border-bottom:1px solid var(--stroke);
    }

    .nav{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      padding:14px 0;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:14px;
    }

    .brand img{
      width:108px;
      height:auto;
      background:#fff;
      border-radius:14px;
      object-fit:contain;
      box-shadow:0 10px 26px rgba(0,0,0,.28);
    }

    .brand-text{
      font-weight:900;
      letter-spacing:.01em;
      line-height:1.1;
    }

    .brand-text span{
      display:block;
      color:var(--muted);
      font-size:13px;
      margin-top:4px;
      font-weight:700;
    }

    .phone-badge{
      display:inline-flex;
      align-items:center;
      gap:10px;
      padding:14px 18px;
      border-radius:999px;
      background:linear-gradient(135deg, rgba(24,164,255,.26), rgba(45,227,165,.16));
      border:1px solid rgba(59,214,255,.28);
      box-shadow:0 12px 30px rgba(0,0,0,.24);
      font-weight:900;
      white-space:nowrap;
    }

    .hero{
      padding:34px 0 18px;
    }

    .hero-grid{
      display:grid;
      grid-template-columns:1.15fr .85fr;
      gap:20px;
      align-items:stretch;
    }

    .hero-main{
      position:relative;
      overflow:hidden;
      background:linear-gradient(180deg, rgba(14,29,52,.86), rgba(8,19,35,.76));
      border:1px solid var(--stroke);
      border-radius:34px;
      padding:32px;
      box-shadow:var(--shadow);
    }

    .hero-main:before{
      content:"";
      position:absolute;
      inset:auto -130px -130px auto;
      width:300px;
      height:300px;
      background:radial-gradient(circle, rgba(24,164,255,.22), transparent 68%);
      pointer-events:none;
    }

    .tag{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:10px 14px;
      border-radius:999px;
      background:rgba(45,227,165,.10);
      border:1px solid rgba(45,227,165,.22);
      color:#baffea;
      font-weight:800;
      font-size:14px;
      margin-bottom:16px;
    }

    h1{
      margin:0;
      font-size:clamp(36px,5vw,64px);
      line-height:1.02;
      letter-spacing:-.05em;
    }

    .subtitle{
      margin:16px 0 0;
      font-size:18px;
      line-height:1.72;
      color:var(--muted);
      max-width:60ch;
    }

    .stats{
      display:grid;
      grid-template-columns:repeat(2,1fr);
      gap:14px;
      margin-top:24px;
    }

    .stat{
      background:rgba(255,255,255,.04);
      border:1px solid var(--stroke);
      border-radius:20px;
      padding:18px;
    }

    .stat-label{
      font-size:13px;
      color:var(--muted);
      text-transform:uppercase;
      letter-spacing:.08em;
      font-weight:800;
      margin-bottom:8px;
    }

    .stat-value{
      font-size:24px;
      font-weight:900;
      line-height:1.15;
    }

    .stat-value.blue{color:#7ddcff}
    .stat-value.green{color:#a8ffe3}

    .cta-row{
      display:flex;
      flex-wrap:wrap;
      gap:12px;
      margin-top:24px;
    }

    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      padding:14px 20px;
      border-radius:16px;
      border:1px solid var(--stroke);
      background:rgba(255,255,255,.04);
      color:var(--text);
      font-weight:800;
    }

    .btn.primary{
      background:linear-gradient(135deg, var(--blue), var(--cyan));
      border:none;
      color:#fff;
      box-shadow:0 12px 30px rgba(24,164,255,.30);
    }

    .side{
      display:flex;
      flex-direction:column;
      gap:14px;
    }

    .visual, .panel, .map-card, .form-card{
      border-radius:28px;
      overflow:hidden;
      border:1px solid var(--stroke);
      box-shadow:var(--shadow);
      background:rgba(255,255,255,.04);
    }

    .visual{
      min-height:290px;
    }

    .visual img, .map-card img{
      width:100%;
      height:100%;
      display:block;
      object-fit:cover;
    }

    .panel{
      padding:20px;
    }

    .panel h3{
      margin:0 0 8px;
      font-size:18px;
    }

    .panel p{
      margin:0;
      color:var(--muted);
      line-height:1.65;
    }

    section{
      padding:16px 0 42px;
    }

    .section-title{
      margin:0 0 16px;
      font-size:28px;
      letter-spacing:-.02em;
    }

    .service-grid{
      display:grid;
      grid-template-columns:repeat(2,1fr);
      gap:16px;
    }

    .service{
      padding:22px;
      background:rgba(255,255,255,.04);
      border:1px solid var(--stroke);
      border-radius:24px;
      box-shadow:var(--shadow);
    }

    .service h3{
      margin:0 0 10px;
      font-size:18px;
    }

    .service p{
      margin:0;
      color:var(--muted);
      line-height:1.65;
    }

    .zones-map-wrap{
      display:grid;
      grid-template-columns:1.25fr .75fr;
      gap:18px;
      align-items:stretch;
    }

    .zones-map-card{
      padding:14px;
    }

    .zones{
      display:flex;
      flex-wrap:wrap;
      gap:10px;
      align-content:flex-start;
      padding-top:4px;
    }

    .zone{
      padding:10px 14px;
      border-radius:999px;
      background:rgba(255,255,255,.06);
      border:1px solid var(--stroke);
      font-weight:800;
      color:#d7f0ff;
    }

    .contact{
      background:linear-gradient(135deg, rgba(24,164,255,.18), rgba(45,227,165,.12));
      border:1px solid rgba(255,255,255,.14);
      border-radius:32px;
      padding:26px;
      box-shadow:var(--shadow);
      display:grid;
      grid-template-columns:1fr auto;
      gap:18px;
      align-items:center;
    }

    .contact strong{
      display:block;
      font-size:15px;
      color:#d7f3ff;
      text-transform:uppercase;
      letter-spacing:.08em;
      margin-bottom:6px;
    }

    .contact .big{
      font-size:36px;
      font-weight:900;
      line-height:1.05;
      color:#fff;
    }

    .contact .small{
      color:var(--muted);
      margin-top:8px;
      line-height:1.6;
    }

    .call{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      padding:18px 24px;
      border-radius:18px;
      background:linear-gradient(135deg, #2de3a5, #18a4ff);
      font-size:20px;
      font-weight:900;
      color:#fff;
      box-shadow:0 14px 32px rgba(45,227,165,.22);
      white-space:nowrap;
    }

    .gallery{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:16px;
    }

    .gallery img{
      width:100%;
      height:240px;
      object-fit:cover;
      border-radius:20px;
      border:1px solid var(--stroke);
      box-shadow:var(--shadow);
    }

    .form-card{
      padding:22px;
    }

    .form-grid{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:12px;
      margin-top:10px;
    }

    input, textarea{
      width:100%;
      padding:14px 16px;
      border-radius:14px;
      border:1px solid rgba(255,255,255,.12);
      background:rgba(255,255,255,.05);
      color:var(--text);
      font:inherit;
      outline:none;
    }

    textarea{
      min-height:120px;
      grid-column:1/-1;
      resize:vertical;
    }

    .submit{
      margin-top:12px;
      width:100%;
      border:none;
      cursor:pointer;
    }

    footer{
      padding:24px 0 40px;
      text-align:center;
      color:var(--muted);
      font-size:14px;
    }

    @media (max-width: 900px){
      .hero-grid, .service-grid, .gallery, .contact, .zones-map-wrap, .form-grid{
        grid-template-columns:1fr;
      }
      .stats{
        grid-template-columns:1fr;
      }
      .nav{
        flex-direction:column;
        align-items:flex-start;
      }
      .phone-badge{
        width:100%;
        justify-content:center;
      }
      .gallery img{
        height:220px;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <img src="4946.jpg" alt="SOS Fibre Optique logo" />
        <div class="brand-text">
          SOS Fibre Optique
          <span>Intervention fibre & télécom</span>
        </div>
      </div>
      <a class="phone-badge" href="tel:0624122187">📞 06 24 12 21 87</a>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-grid">
        <div class="hero-main">
          <div class="tag">UN PROBLÈME AVEC LA FIBRE !?</div>
          <h1>Technicien fibre optique à votre service</h1>
          <p class="subtitle">
            Réparation des gaines bouchées ou écrasées, remise en conformité après échec de raccordement,
            déplacement de prise optique et dépannage rapide avec devis gratuit.
          </p>

          <div class="stats">
            <div class="stat">
              <div class="stat-label">Zone géographique</div>
              <div class="stat-value blue">72 / 53 / 28 / 41 / 61 / 37 / 49</div>
            </div>
            <div class="stat">
              <div class="stat-label">Téléphone direct</div>
              <div class="stat-value green">06 24 12 21 87</div>
            </div>
          </div>

          <div class="cta-row">
            <a class="btn primary" href="tel:0624122187">Appeler maintenant</a>
            <a class="btn" href="#services">Découvrir les services</a>
          </div>
        </div>

        <div class="side">
          <div class="visual">
            <img src="4945.jpg" alt="Technicien fibre optique en intervention" />
          </div>
          <div class="panel">
            <h3>Disponible 7j/7</h3>
            <p>Travail soigné, professionnalisme garanti et interventions sur rendez-vous.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <h2 class="section-title">Travaux que nous pouvons faire</h2>
        <div class="service-grid">
          <div class="service">
            <h3>Réparation des gaines bouchées et écrasées</h3>
            <p>Intervention sur les passages de câbles pour rétablir un cheminement propre et fonctionnel.</p>
          </div>
          <div class="service">
            <h3>Remise en conformité après échec de raccordement</h3>
            <p>Correction de l’installation après un raccordement non abouti pour permettre la mise en service.</p>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container">
        <h2 class="section-title">Carte géographique et zones d’intervention</h2>
        <div class="zones-map-wrap">
          <div class="map-card zones-map-card">
            <img src="zones_map.png" alt="Carte géographique des zones d'intervention 72 53 28 41 61 37 49" />
          </div>
          <div class="zones">
            <span class="zone">72</span>
            <span class="zone">53</span>
            <span class="zone">28</span>
            <span class="zone">41</span>
            <span class="zone">61</span>
            <span class="zone">37</span>
            <span class="zone">49</span>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container contact">
        <div>
          <strong>Contact immédiat</strong>
          <div class="big">06 24 12 21 87</div>
          <div class="small">Zones 72 / 53 / 28 / 41 / 61 / 37 / 49 • Devis gratuit • Disponible 7j/7 sur rendez-vous</div>
        </div>
        <a class="call" href="tel:0624122187">📞 Appeler</a>
      </div>
    </section>

    <section>
      <div class="container">
        <h2 class="section-title">Galerie</h2>
        <div class="gallery">
          <img src="4946.jpg" alt="Logo SOS Fibre Optique" />
          <img src="4945.jpg" alt="Intervention télécom" />
          <img src="4944.jpg" alt="Travail fibre optique" />
        </div>
      </div>
    </section>

    <section>
      <div class="container">
        <h2 class="section-title">Formulaire de devis</h2>
        <div class="form-card">
          <form action="#" method="post">
            <div class="form-grid">
              <input type="text" name="nom" placeholder="Nom" />
              <input type="tel" name="telephone" placeholder="Téléphone" />
              <input type="email" name="email" placeholder="Email" />
              <input type="text" name="ville" placeholder="Ville / département" />
              <textarea name="message" placeholder="Décrivez votre problème fibre"></textarea>
            </div>
            <button class="btn primary submit" type="submit">Envoyer ma demande</button>
          </form>
        </div>
      </div>
    </section>
  </main>

  <footer>
    © 2026 SOS Fibre Optique — Intervention fibre optique dans les zones 72, 53, 28, 41, 61, 37 et 49
  </footer>
</body>
</html>
