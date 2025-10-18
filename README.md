<!doctype html>
<html lang="en">
<head>
 <header class="header-centered">
  <img src="logo.jpg" alt="Bangkok Siam Logo" class="logo" />
  <div class="brand">
    <h1 class="restaurant-name">Bangkok Siam</h1>
    <p class="tagline">Authentic Thai & Vietnamese Cuisine — Full Dining Experience</p>
  </div>
  <div class="cta">
    <button class="btn" onclick="window.print()">Print Menu</button>
    <a class="btn secondary" href="#contact">Contact</a>
  </div>
  <hr class="gold-divider" />
</header>

  <style> /* === Bangkok Siam Fine-Dining Theme === */

/* Base Colors */
:root {
  --gold: #d4af37;
  --deep-gold: #b8860b;
  --ivory: #fffaf0;
  --text-dark: #1f1f1f;
  --text-muted: #666;
  --accent-bg: #ffffff;
}

/* --- Global Reset --- */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
html, body {
  font-family: "Inter", "Segoe UI", Roboto, Arial, sans-serif;
  background: var(--ivory);
  color: var(--text-dark);
  line-height: 1.6;
}

/* --- Header --- */
.header-centered {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin-bottom: 40px;
  padding-top: 25px;
  background: linear-gradient(to bottom, #fffef9 0%, #ffffff 85%);
  box-shadow: 0 4px 20px rgba(0,0,0,0.05);
}
.header-centered .logo {
  width: 180px;
  height: auto;
  margin-bottom: 10px;
  border-radius: 50%;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
}
.restaurant-name {
  font-family: "Playfair Display", serif;
  font-size: 38px;
  letter-spacing: 1px;
  color: var(--deep-gold);
  font-weight: 700;
  margin-bottom: 6px;
}
.tagline {
  font-size: 15px;
  font-style: italic;
  color: var(--text-muted);
  margin-bottom: 12px;
}
.gold-divider {
  width: 120px;
  height: 3px;
  background: linear-gradient(to right, var(--gold), #f9e8a5);
  border: none;
  border-radius: 2px;
  margin: 12px 0 0;
}

/* --- Buttons --- */
.btn {
  background: var(--deep-gold);
  color: #fff;
  padding: 8px 14px;
  border-radius: 8px;
  border: none;
  cursor: pointer;
  font-weight: 600;
  transition: 0.3s ease;
}
.btn:hover {
  background: var(--gold);
  transform: translateY(-2px);
}
.btn.secondary {
  background: #2c3e50;
}
.btn.secondary:hover {
  background: #3c5472;
}

/* --- Main Layout --- */
main {
  display: grid;
  grid-template-columns: 1fr 360px;
  gap: 28px;
  margin-top: 20px;
}
@media (max-width: 980px) {
  main {
    grid-template-columns: 1fr;
  }
}

/* --- Menu Cards --- */
.menu-card {
  background: var(--accent-bg);
  border-radius: 14px;
  padding: 22px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.06);
  border: 1px solid rgba(212,175,55,0.15);
}
h2.section-title {
  font-family: "Playfair Display", serif;
  font-size: 22px;
  margin-bottom: 12px;
  color: var(--deep-gold);
  border-bottom: 2px solid var(--gold);
  display: inline-block;
  padding-bottom: 4px;
}

.category {
  margin-bottom: 22px;
}
.item {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 10px 0;
  border-bottom: 1px dashed rgba(212,175,55,0.2);
}
.item:last-child {
  border-bottom: none;
}
.item .name {
  font-weight: 600;
}
.item .desc {
  font-size: 13.5px;
  color: var(--text-muted);
  margin-top: 5px;
}
.price {
  white-space: nowrap;
  color: var(--deep-gold);
  font-weight: 700;
}

/* --- Sidebar --- */
.sidebar {
  background: var(--accent-bg);
  border-radius: 14px;
  padding: 20px;
  border: 1px solid rgba(212,175,55,0.15);
  box-shadow: 0 8px 20px rgba(0,0,0,0.05);
}
.sidebar h3 {
  color: var(--deep-gold);
  font-family: "Playfair Display", serif;
}
.spice-row {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
  margin-top: 10px;
}
.spice {
  padding: 6px 10px;
  border-radius: 8px;
  border: 1px solid var(--gold);
  color: var(--deep-gold);
  cursor: pointer;
  transition: 0.3s ease;
}
.spice:hover {
  background: var(--gold);
  color: #fff;
}
.spice.active {
  background: var(--deep-gold);
  color: #fff;
}

/* --- Footer --- */
footer {
  margin-top: 40px;
  text-align: center;
  color: var(--text-muted);
  font-size: 14px;
  padding: 20px 0;
  border-top: 1px solid rgba(212,175,55,0.2);
  background: linear-gradient(to top, #fffdf6, #ffffff);
}
footer span {
  color: var(--deep-gold);
}

/* --- Print --- */
@media print {
  .cta, .sidebar { display: none; }
  main { grid-template-columns: 1fr; }
  .menu-card { box-shadow: none; border: none; }
}

    
    /* --- Basic Reset --- */
    *{box-sizing:border-box;margin:0;padding:0}
    html,body{font-family:Inter,Segoe UI,Roboto,Arial,sans-serif;color:#222;background:#faf8f6}
    a{color:inherit;text-decoration:none}

    /* --- Layout --- */
    .container{max-width:1100px;margin:28px auto;padding:20px}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;flex-direction:column}
    .brand h1{font-size:28px;letter-spacing:1px;margin-bottom:4px}
    .brand p{color:#666;font-size:14px}

    .cta{display:flex;gap:8px;align-items:center}
    .btn{background:#c0392b;color:#fff;padding:8px 12px;border-radius:8px;border:0;cursor:pointer;font-weight:600}
    .btn.secondary{background:#2c3e50}

    main{display:grid;grid-template-columns:1fr 360px;gap:24px;margin-top:20px}
    @media (max-width:980px){main{grid-template-columns:1fr}}
    .menu-card{background:#fff;border-radius:12px;padding:18px;box-shadow:0 6px 18px rgba(20,20,20,0.06)}
    h2.section-title{font-size:20px;margin-bottom:10px;color:#1f3b2e}

    /* --- Menu items --- */
    .category{margin-bottom:16px}
    .item{display:flex;justify-content:space-between;padding:8px 0;border-bottom:1px dashed #eee}
    .item:last-child{border-bottom:0}
    .item .name{font-weight:600}
    .item .desc{font-size:13px;color:#666;margin-top:6px}
    .price{white-space:nowrap;color:#1f3b2e;font-weight:700}

    /* --- Sidebar --- */
    aside{position:relative}
    .sidebar{position:sticky;top:24px;background:#fff;padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(20,20,20,0.06)}
    .spice-row{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px}
    .spice{padding:8px 10px;border-radius:8px;border:1px solid #eee;cursor:pointer}
    .spice.active{background:#c0392b;color:#fff;border-color:#c0392b}

    /* --- Footer / print --- */
    footer{margin-top:20px;text-align:center;color:#666;font-size:13px}
    @media print{
      body{background:#fff}
      .cta, .sidebar{display:none}
      main{grid-template-columns:1fr}
      .menu-card{box-shadow:none}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <h1>Bangkok Siam</h1>
        <p>Authentic Thai & Vietnamese Cuisine — Full Dining Experience</p>
      </div>
      <div class="cta">
        <button class="btn" onclick="window.print()">Print Menu</button>
        <a class="btn secondary" href="#contact">Contact</a>
      </div>
    </header>

    <main>
      <!-- Main menu column -->
      <div>
        <section class="menu-card" id="menu">
          <h2 class="section-title">Appetizers</h2>

          <div class="category">
            <div class="item">
              <div>
                <div class="name">Pork Egg Roll (2)</div>
                <div class="desc">Crispy egg rolls — $6.75</div>
              </div>
              <div class="price">$6.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Vegetable Egg Roll (3)</div>
                <div class="desc">Vegetarian egg rolls — $6.75</div>
              </div>
              <div class="price">$6.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Shrimp Roll (5)</div>
                <div class="desc">Shrimp rolls — $8.95</div>
              </div>
              <div class="price">$8.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Spicy Grilled Beef</div>
                <div class="desc">Thai-style grilled beef — $6.75</div>
              </div>
              <div class="price">$6.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Fried Tofu (6)</div>
                <div class="desc">Golden tofu served with dipping sauce — $6.75</div>
              </div>
              <div class="price">$6.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Fish Cake (5)</div>
                <div class="desc">Thai fish cakes with sweet chili — $8.95</div>
              </div>
              <div class="price">$8.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Crab Cheese Wonton (5)</div>
                <div class="desc">Crispy wontons with crab & cheese — $6.75</div>
              </div>
              <div class="price">$6.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Chicken Potstickers (6)</div>
                <div class="desc">Pan-fried dumplings — $7.75</div>
              </div>
              <div class="price">$7.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Chicken Dumplings (6)</div>
                <div class="desc">Steamed dumplings — $7.75</div>
              </div>
              <div class="price">$7.75</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Chicken Satay (4)</div>
                <div class="desc">Grilled marinated chicken with peanut sauce — $9.95</div>
              </div>
              <div class="price">$9.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Shrimp Spring Roll (2)</div>
                <div class="desc">Fresh spring rolls with shrimp — $7.75</div>
              </div>
              <div class="price">$7.75</div>
            </div>
          </div>

          <!-- Salads -->
          <h2 class="section-title">Salads</h2>
          <div class="category">
            <div class="item">
              <div>
                <div class="name">Papaya Salad (choice of shrimp)</div>
                <div class="desc">Shredded green papaya with chili, lime, peanuts — $12.99</div>
              </div>
              <div class="price">$12.99</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Num Tok</div>
                <div class="desc">Choice of beef or pork, red onion, cilantro, mint — $14.50</div>
              </div>
              <div class="price">$14.50</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Larb</div>
                <div class="desc">Choice of meat (beef/pork/chicken), fresh herbs — $14.50</div>
              </div>
              <div class="price">$14.50</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Yum Woon Sen (Noodle Salad)</div>
                <div class="desc">Ground pork, white onion, tomato, celery — $14.50</div>
              </div>
              <div class="price">$14.50</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Seafood Salad</div>
                <div class="desc">Seafood with white onion, tomato, celery — $18.99</div>
              </div>
              <div class="price">$18.99</div>
            </div>
          </div>

          <!-- Noodles -->
          <h2 class="section-title">Noodle</h2>
          <div class="category">
            <p style="font-size:13px;color:#666;margin-bottom:8px">
              Choice of meat: Chicken, Pork, Beef, Tofu, Veggie (Shrimp/Seafood/Combination +$3.00)
            </p>

            <div class="item">
              <div>
                <div class="name">N1. Pad Thai</div>
                <div class="desc">Rice noodle, egg, tofu, bean sprout, ground peanut, fresh lime — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">N2. Drunken Noodle</div>
                <div class="desc">Flat rice noodle with basil, chili, peppers — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">N3. Pad Se Ew</div>
                <div class="desc">Wide rice noodle, egg, Chinese broccoli — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">N4. Pad Woon Sen</div>
                <div class="desc">Glass noodle stir-fry with mixed vegetables — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">N5. Lad Na</div>
                <div class="desc">Flat noodle with creamy soup and veggies — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">N6. Tom Yum Noodle Soup</div>
                <div class="desc">Tom yum creamy soup with fish ball & fried wonton — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>
          </div>

          <!-- Rice plates -->
          <h2 class="section-title">Thai Rice Plate</h2>
          <div class="category">
            <p style="font-size:13px;color:#666;margin-bottom:8px">Choice of meat: Chicken, Pork, Beef, Tofu, Veggie (Shrimp/Seafood/Combination +$3.00)</p>

            <div class="item">
              <div>
                <div class="name">T1. Thai Fried Rice</div>
                <div class="desc">Jasmine rice, egg, vegetables — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">T2. Pineapple Fried Rice</div>
                <div class="desc">Pineapple, cashew, raisin, coconut flake — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">T3. Green Curry Fried Rice</div>
                <div class="desc">Green curry paste, eggplant, basil — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">T4. Red Curry Fried Rice</div>
                <div class="desc">Red curry paste, veggies — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">T5. Crab Fried Rice</div>
                <div class="desc">Crab meat, veggies — $18.95</div>
              </div>
              <div class="price">$18.95</div>
            </div>
          </div>

          <!-- Stir fried, Soups, Curry, Specials condensed -->
          <h2 class="section-title">Stir-Fried / Curries / Soups / Specials</h2>
          <div class="category">
            <div class="item">
              <div>
                <div class="name">F1. Pad Kra Pao (Basil Stir Fried)</div>
                <div class="desc">Served with jasmine rice — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">F2. Pad Cashew Nut</div>
                <div class="desc">Cashews, peppers, onions — $15.95</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Tom Kha / Tom Yum</div>
                <div class="desc">Regular $14.50 / Large $21.95 — choice of meat with herbs</div>
              </div>
              <div class="price">$14.50 / $21.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">C1–C5. Curries (Red / Green / Panang / Massaman / Pineapple)</div>
                <div class="desc">Choice of meat — $15.95 each (served with jasmine rice)</div>
              </div>
              <div class="price">$15.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Special: Fried Lime Fish</div>
                <div class="desc">Whole fish — $34.95</div>
              </div>
              <div class="price">$34.95</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Special: Steam Lime Fish</div>
                <div class="desc">Whole fish steamed with lime — $34.95</div>
              </div>
              <div class="price">$34.95</div>
            </div>
          </div>

          <!-- Vietnamese / Pho -->
          <h2 class="section-title">Pho & Vietnamese Noodle Soups</h2>
          <div class="category">
            <p style="font-size:13px;color:#666;margin-bottom:8px">
              Regular $14.50 / Large $15.95. Many pho choices; combination options and seafood add-ons noted on menu.
            </p>

            <div class="item">
              <div>
                <div class="name">P1. Combination Pho (+$1.00)</div>
                <div class="desc">Steak, brisket, tendon, flank, tripe, beef ball</div>
              </div>
              <div class="price">see menu</div>
            </div>

            <div class="item">
              <div>
                <div class="name">K1–K8. Pho (various cuts)</div>
                <div class="desc">Kid-friendly and classic pho options — $7.99 (kids/side sizes listed)</div>
              </div>
              <div class="price">$7.99</div>
            </div>

            <div class="item">
              <div>
                <div class="name">V1–V5. Vermicelli Bowls</div>
                <div class="desc">Combination & grilled proteins — $15.50–$17.50</div>
              </div>
              <div class="price">$15.50–$17.50</div>
            </div>
          </div>

          <h2 class="section-title">Desserts & Kids</h2>
          <div class="category">
            <div class="item">
              <div>
                <div class="name">Mango Sticky Rice</div>
                <div class="desc">Sweet sticky rice with coconut & fresh mango — $9.00</div>
              </div>
              <div class="price">$9.00</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Vietnamese Coffee Flan</div>
                <div class="desc">Coffee-infused custard — $8.00</div>
              </div>
              <div class="price">$8.00</div>
            </div>

            <div class="item">
              <div>
                <div class="name">Kid Fried Rice</div>
                <div class="desc">Smaller portion for kids — $7.99</div>
              </div>
              <div class="price">$7.99</div>
            </div>
          </div>

        </section>
      </div>

      <!-- Sidebar -->
      <aside>
        <div class="sidebar" id="controls">
          <h3 style="margin-bottom:8px">Dining Info & Controls</h3>
          <p style="color:#555;font-size:14px">All Thai dishes: select spice level when ordering.</p>

          <div style="margin-top:12px">
            <strong>Spice level</strong>
            <div class="spice-row" id="spiceRow">
              <div class="spice" data-level="Mild">Mild</div>
              <div class="spice" data-level="Medium">Medium</div>
              <div class="spice" data-level="Hot">Hot</div>
              <div class="spice" data-level="Very Hot">Very Hot</div>
              <div class="spice" data-level="Thai Hot">Thai Hot</div>
            </div>
          </div>

          <div style="margin-top:14px">
            <strong>Hours</strong>
            <p style="font-size:14px;color:#666;margin-top:6px">Mon–Sun: 11:00 AM – 9:30 PM</p>
          </div>

          <div style="margin-top:14px">
            <strong>Contact</strong>
            <p style="font-size:14px;color:#666;margin-top:6px">Phone: (XXX) XXX-XXXX<br/>Address: 123 Example Street</p>
          </div>

          <div style="margin-top:14px">
            <button class="btn" onclick="scrollToMenu()">View Full Menu</button>
          </div>

          <div style="margin-top:12px;font-size:13px;color:#999">
            <em>Menu content sourced from uploaded PDF.</em>
          </div>
        </div>
      </aside>
    </main>

    <footer id="contact">
      <p>© <span id="year"></span> Bangkok Siam — Authentic Thai & Vietnamese Cuisine</p>
    </footer>
  </div>

  <script>
    // Spice buttons
    const spiceRow = document.getElementById('spiceRow');
    spiceRow.addEventListener('click', (e) => {
      if(!e.target.classList.contains('spice')) return;
      document.querySelectorAll('.spice').forEach(s=>s.classList.remove('active'));
      e.target.classList.add('active');
      // store preference (demo only)
      localStorage.setItem('spicePref', e.target.dataset.level);
      alert('Spice level set to: ' + e.target.dataset.level);
    });

    // restore if set
    const pref = localStorage.getItem('spicePref');
    if(pref){
      const el = [...document.querySelectorAll('.spice')].find(s=>s.dataset.level===pref);
      if(el) el.classList.add('active');
    }

    // set year
    document.getElementById('year').textContent = new Date().getFullYear();

    function scrollToMenu(){ document.getElementById('menu').scrollIntoView({behavior:'smooth'}); }
  </script>
</body>
</html>
