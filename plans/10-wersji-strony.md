# Plan: 10 wersji strony Femme Vision Kinga Maryniak

> Source PRD: `prd.md`

## Architectural decisions

- **Technologia**: Tailwind CSS CDN, statyczny HTML, Google Fonts (Noto Serif + Manrope + Material Symbols Outlined)
- **Struktura katalogów**: `v01-szalwia/` ... `v10-eucalyptus/`, każdy z `index.html` (+ podstrony w v07, v10)
- **Treść**: identyczna we wszystkich wersjach — źródło: obecny `index.html`
- **Zdjęcia**: te same Google Photos URLs co w obecnym `index.html`
- **CTA**: link do Google Calendar `https://calendar.app.google/SgwkkR6YrpGz9JnGA`
- **Mobile-first**: wszystkie wersje projektowane od mobile w górę
- **Formularz kontaktowy**: wersje parzyste (2,4,6,8,10) — frontend-only, bez backendu (imię, email, wiadomość)
- **Instagram/email**: placeholder — linki do uzupełnienia później
- **Sekcje wspólne**: Hero, Problem, O mnie, Usługi SDR, OBM, Opinie (testimonial Kamili + case study 45k zł), Cennik, CTA/Kontakt, Footer
- **Ikony usług**: emoji (💎🔄⚙️🚀) zastąpione dedykowanymi ikonami (SVG/CSS/Material Symbols) dopasowanymi do estetyki każdej wersji — spójne wizualnie, nie generyczne emoji

---

## Phase 1: v01-szalwia — minimalistyczna baza

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 10, 11, 14, 15

### What to build

Pierwsza wersja strony — minimalistyczna, dużo białej przestrzeni. Paleta: kremowy + szałwiowa zieleń. Subtelne inline SVG liście szałwii jako dekoracja w tle sekcji. One-page scroll. Subtelne fade-in animacje przy scrollu (IntersectionObserver). Mobilna nawigacja: hamburger z slide-in panelem. Ta wersja ustala wzorzec struktury HTML dla kolejnych wersji.

### Acceptance criteria

- [ ] Katalog `v01-szalwia/index.html` istnieje i renderuje się poprawnie
- [ ] Paleta: kremowy (#FFFDF7 rodzina) + szałwiowa zieleń (#7C9A82 rodzina)
- [ ] SVG liście szałwii widoczne jako dekoracja w tle (min. 2 sekcje)
- [ ] Wszystkie 8 sekcji treści obecne z identycznym tekstem
- [ ] Mobile-first: poprawny widok na 375px
- [ ] Hamburger menu slide-in działa na mobile
- [ ] CTA linkuje do Google Calendar
- [ ] Fade-in animacje przy scrollu
- [ ] Zdjęcia z Google Photos wyświetlają się poprawnie

---

## Phase 2: v02-jungle — bujny tropik

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15

### What to build

Odważna, bujna wersja. Paleta: szmaragd + złoto + krem. Duże inline SVG ilustracje tropikalnych liści (monstera, bananowiec). Sekcje full-width bez max-width ograniczeń. Zaawansowane animacje parallax przy scrollu. Mobilna nawigacja: bottom tab bar (stały pasek na dole). Formularz kontaktowy obok CTA.

### Acceptance criteria

- [ ] Katalog `v02-jungle/index.html` renderuje się poprawnie
- [ ] Paleta: szmaragd (#065F46 rodzina) + złoto (#D4A843 rodzina) + krem
- [ ] Duże SVG monstera/tropikalne liście (min. 3 dekoracje)
- [ ] Sekcje full-width
- [ ] Parallax efekt na min. 2 sekcjach
- [ ] Bottom tab bar nawigacja na mobile
- [ ] Formularz kontaktowy (imię, email, wiadomość) — frontend only
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 3: v03-herbarium — vintage botaniczny

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 14, 15

### What to build

Elegancka, vintage-botaniczna wersja. Paleta: oliwka + ecru + miedź. Delikatne ryciny botaniczne jako CSS/SVG pattern w tle. Asymetryczne layouty sekcji (grid z nierównymi kolumnami, przesunięcia). Subtelne hover efekty i fade-in. Mobilna nawigacja: hamburger z full-screen overlay.

### Acceptance criteria

- [ ] Katalog `v03-herbarium/index.html` renderuje się poprawnie
- [ ] Paleta: oliwka (#6B705C rodzina) + ecru (#FFF8E7) + miedź (#B87333 rodzina)
- [ ] Botaniczne patterny/ryciny widoczne w tle
- [ ] Asymetryczny layout (min. 2 sekcje z nierównym gridem)
- [ ] Hover efekty na kartach usług
- [ ] Full-screen overlay menu na mobile
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 4: v04-ogrod — miękki organiczny

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15

### What to build

Miękka, organiczna wersja. Paleta: pastelowa zieleń + róż + piaskowy. Akwarelowe kwiaty i liście jako CSS gradienty/SVG. Karty z mocno zaokrąglonymi rogami (rounded-3xl+). Micro-interactions (hover scale, przejścia kolorów, pulsujące CTA). Mobilna nawigacja: floating pill nav (zaokrąglony pasek nawigacji unoszący się nad treścią). Formularz kontaktowy.

### Acceptance criteria

- [ ] Katalog `v04-ogrod/index.html` renderuje się poprawnie
- [ ] Paleta: pastelowa zieleń (#A8C5A0) + róż (#E8B4B8) + piaskowy (#F5E6CC)
- [ ] Akwarelowe elementy dekoracyjne (CSS gradienty lub SVG)
- [ ] Karty z dużymi zaokrągleniami
- [ ] Micro-interactions na hover (min. 3 elementy)
- [ ] Floating pill nav na mobile
- [ ] Formularz kontaktowy
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 5: v05-bamboo — zen minimalizm

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 10, 11, 14, 15

### What to build

Japoński minimalizm, zen. Paleta: matcha + biały + antracyt. Bambusowe pionowe linie jako SVG dekoracja. Bardzo dużo białej przestrzeni. Prosty grid layout. Zero animacji — szybkie ładowanie, czysty design. Mobilna nawigacja: minimalistyczny top bar (tylko logo + hamburger icon).

### Acceptance criteria

- [ ] Katalog `v05-bamboo/index.html` renderuje się poprawnie
- [ ] Paleta: matcha (#C8D5B9 rodzina) + biały + antracyt (#2D2D2D)
- [ ] Bambusowe SVG linie dekoracyjne
- [ ] Dużo white space (padding/margin większy niż inne wersje)
- [ ] Zero animacji CSS/JS
- [ ] Minimalistyczna nawigacja top bar
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 6: v06-greenhouse — glassmorphism

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15

### What to build

Nowoczesna wersja z efektem szklarni. Paleta: ciemna zieleń + miętowy + biały. Liście SVG widoczne za półprzezroczystymi kartami (glassmorphism: backdrop-blur + rgba tła). Blur transitions między sekcjami. Mobilna nawigacja: side drawer (wysuwa się z boku). Formularz kontaktowy.

### Acceptance criteria

- [ ] Katalog `v06-greenhouse/index.html` renderuje się poprawnie
- [ ] Paleta: ciemna zieleń (#1B4332 rodzina) + miętowy (#95D5B2) + biały
- [ ] Glassmorphism karty (backdrop-blur, półprzezroczyste tło)
- [ ] SVG liście widoczne za kartami
- [ ] Blur/fade transitions
- [ ] Side drawer nawigacja na mobile
- [ ] Formularz kontaktowy
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 7: v07-terracotta — multi-page śródziemnomorski

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 14, 15

### What to build

Ciepła, śródziemnomorska wersja rozłożona na 4 strony HTML. Paleta: terrakota + oliwka + krem. Gałązki oliwne jako inline SVG dekoracja. Subtelne page transitions (CSS). Mobilna nawigacja: hamburger + breadcrumbs na podstronach.

Strony:
- `index.html` — Hero + Problem + skrót usług + CTA
- `uslugi.html` — Pełna oferta SDR + OBM
- `o-mnie.html` — O mnie + Opinie + Case study
- `kontakt.html` — Cennik + CTA + 3 kroki

### Acceptance criteria

- [ ] 4 pliki HTML w `v07-terracotta/`
- [ ] Paleta: terrakota (#C67C4E rodzina) + oliwka (#6B705C) + krem
- [ ] SVG gałązki oliwne dekoracyjne
- [ ] Nawigacja między stronami działa
- [ ] Breadcrumbs na podstronach (mobile + desktop)
- [ ] Hamburger menu na mobile
- [ ] Wszystkie treści rozłożone na 4 strony

---

## Phase 8: v08-moss — dark premium

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15

### What to build

Dark mode premium. Paleta: ciemny mech (tło) + złoto (akcenty) + kremowy tekst. Mech i paprocie jako ciemne SVG dekoracje. Parallax scroll na sekcjach z dekoracjami. Mobilna nawigacja: sticky minimal nav (cienki pasek, pojawia się po scrollu). Formularz kontaktowy.

### Acceptance criteria

- [ ] Katalog `v08-moss/index.html` renderuje się poprawnie
- [ ] Dark mode: ciemne tło (#1A2E1A rodzina) + złote akcenty (#C5A55A) + kremowy tekst
- [ ] SVG mech/paprocie dekoracje
- [ ] Parallax efekt na min. 2 sekcjach
- [ ] Sticky nav pojawia się po scrollu
- [ ] Formularz kontaktowy
- [ ] Czytelność tekstu na ciemnym tle (kontrast WCAG AA)
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 9: v09-wildflower — artystyczny collage

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 14, 15

### What to build

Artystyczna, odręczna wersja. Paleta: lawendowy + miodowy + zieleń. Polne kwiaty w odręcznym stylu jako SVG. Collage-style layout (elementy nachodzą na siebie, obrócone karty, asymetryczne rozmieszczenie). Artystyczne hover effects (rotacja, scale, color shift). Mobilna nawigacja: full-screen menu z animacją.

### Acceptance criteria

- [ ] Katalog `v09-wildflower/index.html` renderuje się poprawnie
- [ ] Paleta: lawendowy (#B8A9C9) + miodowy (#DAA520 rodzina) + zieleń (#6B8E6B)
- [ ] SVG polne kwiaty w odręcznym stylu
- [ ] Collage layout (elementy nachodzące, rotacje)
- [ ] Hover effects artystyczne
- [ ] Full-screen menu z animacją na mobile
- [ ] Wszystkie sekcje treści kompletne

---

## Phase 10: v10-eucalyptus — skandynawski multi-page

**User stories**: 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15

### What to build

Clean, skandynawski design na 4 stronach. Paleta: szarozielony + biały + ciepłe drewno. Gałązki eukaliptusa jako proste, geometryczne SVG. Subtelne fade animacje. Mobilna nawigacja: scandinavian clean nav (prosta, przestronna). Formularz kontaktowy.

Strony:
- `index.html` — Hero + Problem + CTA
- `uslugi.html` — SDR + OBM pełna oferta
- `o-mnie.html` — O mnie + Opinie + Case study
- `kontakt.html` — Cennik + Formularz + CTA + 3 kroki

### Acceptance criteria

- [ ] 4 pliki HTML w `v10-eucalyptus/`
- [ ] Paleta: szarozielony (#8B9D83 rodzina) + biały + drewno (#D4A574 rodzina)
- [ ] SVG gałązki eukaliptusa
- [ ] Subtelne fade-in animacje
- [ ] Clean nav — przestronna, prosta
- [ ] Formularz kontaktowy
- [ ] Nawigacja między stronami działa
- [ ] Wszystkie treści rozłożone na 4 strony
