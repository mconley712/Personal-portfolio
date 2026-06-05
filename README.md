# Personal-portfolio

---
---
:root {
  --white: #FFFFFF;
  --cream: #FDF8F5;
  --blush: #F9EEF0;
  --rose: #E8A0B0;
  --pink: #D4607A;
  --deep-pink: #B8405A;
  --gold: #C9A84C;
  --gold-light: #E2C068;
  --charcoal: #2C2C2C;
  --muted: #7A6E70;
  --border: #EDD8DC;
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body { font-family: 'Lato', sans-serif; background: var(--cream); color: var(--charcoal); overflow-x: hidden; }

/* NAV */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 100;
  display: flex; align-items: center; justify-content: space-between;
  padding: 1.1rem 3rem;
  background: rgba(253,248,245,0.95);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--border);
}
.nav-logo {
  font-family: 'Playfair Display', serif;
  font-size: 1.2rem; font-weight: 600; letter-spacing: 0.06em;
  color: var(--deep-pink); text-decoration: none;
}
.nav-links { display: flex; gap: 2rem; list-style: none; }
.nav-links a {
  font-size: 0.8rem; font-weight: 700; letter-spacing: 0.12em;
  text-transform: uppercase; color: var(--muted); text-decoration: none;
  transition: color 0.2s;
}
.nav-links a:hover { color: var(--deep-pink); }

/* HERO */
#home {
  min-height: 100vh;
  display: grid; grid-template-columns: 1fr 1fr;
  align-items: center;
  padding: 7rem 3rem 4rem;
  gap: 4rem;
  background: linear-gradient(135deg, #FDF8F5 0%, #F9EEF0 100%);
}
.hero-text { max-width: 520px; }
.hero-eyebrow {
  font-size: 0.72rem; font-weight: 700; letter-spacing: 0.22em;
  text-transform: uppercase; color: var(--gold);
  margin-bottom: 1.1rem;
}
.hero-name {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.8rem, 5.5vw, 5rem);
  font-weight: 700; line-height: 1.08;
  color: var(--deep-pink); margin-bottom: 1.1rem;
}
.hero-name em { font-style: italic; color: var(--pink); }
.hero-tagline {
  font-size: 1rem; line-height: 1.8; color: var(--muted);
  margin-bottom: 2rem; max-width: 420px;
}
.hero-pillars { display: flex; gap: 0.75rem; margin-bottom: 2.25rem; flex-wrap: wrap; }
.pillar {
  font-size: 0.7rem; font-weight: 700; letter-spacing: 0.15em;
  text-transform: uppercase; color: var(--deep-pink);
  border: 1.5px solid var(--rose); padding: 0.4rem 1rem;
  background: var(--white); border-radius: 2px;
}
.hero-actions { display: flex; gap: 1rem; flex-wrap: wrap; }
.btn-primary {
  display: inline-flex; align-items: center; gap: 0.5rem;
  background: var(--deep-pink); color: var(--white);
  font-size: 0.78rem; font-weight: 700; letter-spacing: 0.12em;
  text-transform: uppercase; text-decoration: none;
  padding: 0.85rem 1.75rem; border-radius: 2px;
  transition: background 0.2s, transform 0.2s;
}
.btn-primary:hover { background: var(--gold); transform: translateY(-2px); }
.btn-secondary {
  display: inline-flex; align-items: center; gap: 0.5rem;
  border: 1.5px solid var(--deep-pink); color: var(--deep-pink);
  font-size: 0.78rem; font-weight: 700; letter-spacing: 0.12em;
  text-transform: uppercase; text-decoration: none;
  padding: 0.85rem 1.75rem; border-radius: 2px;
  transition: all 0.2s;
}
.btn-secondary:hover { background: var(--deep-pink); color: var(--white); }

.hero-image-wrap { position: relative; display: flex; justify-content: center; }
.hero-image-frame { position: relative; width: 400px; height: 500px; }
.hero-image-frame::before {
  content: ''; position: absolute;
  top: 14px; left: 14px; right: -14px; bottom: -14px;
  border: 2px solid var(--gold); z-index: 0;
}
.hero-photo {
  position: relative; z-index: 1;
  width: 100%; height: 100%; object-fit: cover; object-position: center top;
  display: block;
}
.hero-badge {
  position: absolute; bottom: -20px; left: -20px; z-index: 2;
  background: var(--deep-pink); color: var(--white);
  padding: 1rem 1.25rem;
}
.badge-num {
  font-family: 'Playfair Display', serif;
  font-size: 1.8rem; font-weight: 700; line-height: 1; color: var(--gold-light);
}
.badge-label { font-size: 0.68rem; letter-spacing: 0.1em; text-transform: uppercase; opacity: 0.85; margin-top: 0.2rem; }

/* SECTION SHARED */
section { padding: 5.5rem 3rem; }
.section-label {
  font-size: 0.7rem; font-weight: 700; letter-spacing: 0.22em;
  text-transform: uppercase; color: var(--gold); margin-bottom: 0.6rem;
}
.section-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(1.9rem, 3.5vw, 2.9rem);
  font-weight: 700; line-height: 1.2; color: var(--deep-pink); margin-bottom: 1.25rem;
}
.divider { width: 44px; height: 2px; background: var(--gold); margin-bottom: 1.75rem; }
p { font-size: 0.95rem; line-height: 1.85; color: var(--muted); }

/* ABOUT */
#about { background: var(--deep-pink); }
#about .section-label { color: var(--gold-light); }
#about .section-title { color: var(--white); }
#about p { color: rgba(255,255,255,0.8); }
#about .divider { background: var(--gold-light); }
.about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: start; max-width: 1100px; }
.about-text p + p { margin-top: 1.2rem; }
.about-values { display: flex; flex-direction: column; gap: 1.4rem; }
.value-item { border-left: 3px solid var(--gold-light); padding-left: 1.2rem; }
.value-title { font-family: 'Playfair Display', serif; font-size: 1.15rem; font-weight: 600; color: var(--white); margin-bottom: 0.3rem; }
.value-desc { font-size: 0.88rem; color: rgba(255,255,255,0.65); line-height: 1.7; }

/* LEADERSHIP */
#leadership { background: var(--blush); }
.leadership-feature { display: grid; grid-template-columns: 1fr 1fr; gap: 3.5rem; align-items: center; max-width: 1050px; margin-bottom: 3rem; }
.leadership-photo-wrap { position: relative; }
.leadership-photo-frame { position: relative; width: 100%; max-width: 420px; }
.leadership-photo-frame::before {
  content: ''; position: absolute;
  top: 12px; right: -12px; bottom: -12px; left: 12px;
  border: 2px solid var(--gold); z-index: 0;
}
.leadership-photo { position: relative; z-index: 1; width: 100%; aspect-ratio: 3/4; object-fit: cover; object-position: center; display: block; }
.miss-badge {
  position: absolute; top: -16px; right: 20px; z-index: 3;
  background: var(--gold); color: var(--white);
  font-family: 'Playfair Display', serif;
  font-size: 0.85rem; font-weight: 700;
  padding: 0.5rem 1rem; letter-spacing: 0.05em;
}
.events-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; margin-top: 1.75rem; }
.event-card {
  background: var(--white); border: 1px solid var(--border);
  padding: 1rem 1.1rem; border-radius: 2px;
  transition: border-color 0.2s, transform 0.2s;
}
.event-card:hover { border-color: var(--pink); transform: translateY(-2px); }
.event-icon { font-size: 1.3rem; margin-bottom: 0.4rem; }
.event-name { font-family: 'Playfair Display', serif; font-size: 0.95rem; font-weight: 600; color: var(--deep-pink); line-height: 1.3; }
.event-desc { font-size: 0.78rem; color: var(--muted); margin-top: 0.25rem; line-height: 1.5; }
.roles-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1rem; max-width: 800px; margin-top: 2rem; }
.role-card { background: var(--white); border: 1px solid var(--border); padding: 1.4rem 1.6rem; border-radius: 2px; transition: border-color 0.2s; }
.role-card:hover { border-color: var(--pink); }
.role-org { font-size: 0.68rem; font-weight: 700; letter-spacing: 0.15em; text-transform: uppercase; color: var(--gold); margin-bottom: 0.35rem; }
.role-title { font-family: 'Playfair Display', serif; font-size: 1.15rem; font-weight: 600; color: var(--deep-pink); }

/* SERVICE */
#service { background: var(--white); }
.service-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 3.5rem; align-items: center; max-width: 1050px; }
.service-photo { width: 100%; max-width: 480px; aspect-ratio: 4/3; object-fit: cover; object-position: center top; display: block; border: 1px solid var(--border); }
.service-content p + p { margin-top: 1.1rem; }

/* RESEARCH */
#research { background: var(--cream); }
.research-card { background: var(--white); border: 1px solid var(--border); padding: 2.5rem; max-width: 820px; border-radius: 2px; }
.research-card h3 { font-family: 'Playfair Display', serif; font-size: 1.5rem; font-weight: 600; color: var(--deep-pink); margin-bottom: 0.9rem; }
.research-tags { display: flex; gap: 0.6rem; flex-wrap: wrap; margin-top: 1.4rem; }
.tag { font-size: 0.68rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; color: var(--deep-pink); border: 1px solid var(--border); padding: 0.3rem 0.75rem; border-radius: 2px; background: var(--blush); }

/* ACHIEVEMENTS */
#achievements { background: var(--blush); }
.achievements-list { display: flex; flex-direction: column; gap: 0.9rem; max-width: 700px; }
.achievement { display: flex; align-items: flex-start; gap: 1.1rem; padding: 1.1rem 1.4rem; border: 1px solid var(--border); background: var(--white); border-radius: 2px; }
.achievement-icon { width: 30px; height: 30px; flex-shrink: 0; border: 1.5px solid var(--gold); color: var(--gold); display: flex; align-items: center; justify-content: center; font-size: 0.9rem; }
.achievement-text h4 { font-family: 'Playfair Display', serif; font-size: 1.05rem; font-weight: 600; color: var(--deep-pink); margin-bottom: 0.15rem; }
.achievement-text p { font-size: 0.82rem; }

/* CONTACT */
#contact { background: var(--deep-pink); text-align: center; }
#contact .section-label { color: var(--gold-light); }
#contact .section-title { color: var(--white); }
#contact .divider { margin: 0 auto 1.75rem; background: var(--gold-light); }
#contact > p { color: rgba(255,255,255,0.75); max-width: 480px; margin: 0 auto 2.25rem; }
.contact-links { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }
.contact-link { display: inline-flex; align-items: center; gap: 0.5rem; font-size: 0.78rem; font-weight: 700; letter-spacing: 0.12em; text-transform: uppercase; text-decoration: none; padding: 0.85rem 1.75rem; border-radius: 2px; transition: all 0.2s; }
.contact-link-light { background: var(--white); color: var(--deep-pink); }
.contact-link-light:hover { background: var(--gold-light); color: var(--white); }
.contact-link-outline { border: 1.5px solid rgba(255,255,255,0.45); color: var(--white); }
.contact-link-outline:hover { background: rgba(255,255,255,0.15); }

footer { background: var(--charcoal); color: rgba(255,255,255,0.4); text-align: center; padding: 1.5rem; font-size: 0.78rem; letter-spacing: 0.05em; }

/* ANIMATIONS */
.fade-in { opacity: 0; transform: translateY(18px); transition: opacity 0.65s ease, transform 0.65s ease; }
.fade-in.visible { opacity: 1; transform: translateY(0); }

/* RESPONSIVE */
@media (max-width: 900px) {
  nav { padding: 1rem 1.5rem; }
  #home { grid-template-columns: 1fr; padding: 6rem 1.5rem 3rem; text-align: center; }
  .hero-tagline { margin: 0 auto 2rem; }
  .hero-pillars, .hero-actions { justify-content: center; }
  .hero-image-wrap { display: none; }
  section { padding: 4rem 1.5rem; }
  .about-grid, .leadership-feature, .service-grid { grid-template-columns: 1fr; gap: 2rem; }
  .events-grid, .roles-grid { grid-template-columns: 1fr; }
}
