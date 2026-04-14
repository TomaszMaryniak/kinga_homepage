# PRD: 10 wersji strony Femme Vision Kinga Maryniak

## Context

Kinga Maryniak ma stronę wirtualnej asystentki (OBM & SDR). Obecna wersja w `index.html` jest funkcjonalna ale chłodna stylistycznie. Cel: stworzyć 10 różnych wersji designu — ciepłych, z elementami roślinnymi, zachęcających do kontaktu. Każda wersja w osobnym katalogu. Treść identyczna we wszystkich wersjach.

---

## Problem Statement

Obecna strona jest jednowariantowa, utrzymana w chłodnej szaro-beżowej palecie. Brakuje ciepła, elementów roślinnych i różnorodności wizualnej. Klientka chce przetestować 10 różnych podejść stylistycznych i strukturalnych, aby wybrać najlepszy kierunek.

## Solution

10 niezależnych wersji strony, każda w osobnym katalogu (`v01-szalwia/`, `v02-jungle/`, etc.), z identyczną treścią ale różnym designem, paletą kolorów, elementami roślinnymi, strukturą i poziomem animacji.

## User Stories

1. As a visitor, I want the website to feel warm and inviting, so that I feel comfortable reaching out for a consultation
2. As a visitor on mobile, I want the page to work perfectly on my phone, so that I can browse and contact Kinga easily
3. As Kinga, I want 10 different design versions, so that I can compare and choose the best direction
4. As a visitor, I want to see plant/botanical elements, so that the page feels organic and calming
5. As a visitor, I want a clear CTA button linking to Google Calendar, so that I can book a free consultation
6. As a visitor, I want to read testimonials, so that I trust Kinga's services
7. As a visitor, I want to see pricing clearly, so that I can decide if the service fits my budget
8. As Kinga, I want each version in a separate directory, so that I can easily share and compare them
9. As a visitor, I want smooth animations (where applicable), so that the browsing experience feels premium
10. As a visitor, I want a working mobile navigation, so that I can access all sections on my phone
11. As Kinga, I want the same text content across all versions, so that I only compare visual differences
12. As a visitor, I want a contact form in some versions, so that I have an alternative to booking via calendar
13. As a visitor, I want to see Kinga's case study (45,000 zł result), so that I understand the ROI
14. As a visitor, I want the page to load fast, so that I don't leave before it renders
15. As Kinga, I want to experiment with different nav patterns on mobile, so that I find what works best

## Implementation Decisions

### Wersje — 10 koncepcji

| # | Katalog | Nazwa | Paleta | Elementy roślinne | Struktura | Animacje | Nav mobilna |
|---|---------|-------|--------|-------------------|-----------|----------|-------------|
| 1 | `v01-szalwia/` | Szałwia | Kremowy + szałwiowa zieleń | Subtelne SVG liście szałwii w tle | One-page scroll | Subtelne fade-in | Hamburger slide-in |
| 2 | `v02-jungle/` | Jungle | Szmaragd + złoto + krem | Duże tropikalne liście, monstera SVG | One-page full-width | Zaawansowane parallax | Bottom tab bar |
| 3 | `v03-herbarium/` | Herbarium | Oliwka + ecru + miedź | Delikatne ryciny botaniczne pattern | One-page asymetryczny | Subtelne hover + fade | Hamburger overlay |
| 4 | `v04-ogrod/` | Ogród | Pastelowa zieleń + róż + piaskowy | Akwarelowe kwiaty/liście CSS | One-page rounded cards | Micro-interactions | Floating pill nav |
| 5 | `v05-bamboo/` | Bamboo | Matcha + biały + antracyt | Bambusowe linie SVG | One-page zen grid | Minimalne, bez animacji | Minimalist top bar |
| 6 | `v06-greenhouse/` | Greenhouse | Ciemna zieleń + miętowy + biały | Liście za glassmorphism | One-page glass cards | Glassmorphism blur transitions | Side drawer |
| 7 | `v07-terracotta/` | Terracotta | Terrakota + oliwka + krem | Gałązki oliwne SVG | Multi-page (4 strony) | Subtelne page transitions | Hamburger + breadcrumbs |
| 8 | `v08-moss/` | Moss | Ciemny mech + złoto + krem tekst | Mech, paprocie dark SVG | One-page dark mode | Parallax scroll | Sticky minimal nav |
| 9 | `v09-wildflower/` | Wildflower | Lawendowy + miodowy + zieleń | Polne kwiaty, odręczny styl | One-page collage | Artystyczne hover effects | Full-screen menu |
| 10 | `v10-eucalyptus/` | Eucalyptus | Szarozielony + biały + drewno | Gałązki eukaliptusa SVG | Multi-page (4 strony) | Subtelne fade | Scandinavian clean nav |

### Wspólne elementy (wszystkie wersje)

- **Technologia**: Tailwind CSS via CDN, single/multi HTML files (static)
- **Treść**: identyczna — kopiowana z `strona www - finalna wersja 09.04. .md`
- **Zdjęcia**: te same linki Google Photos co w obecnym `index.html`
- **CTA**: link do Google Calendar (`https://calendar.app.google/SgwkkR6YrpGz9JnGA`)
- **Mobile-first**: wszystkie wersje projektowane od mobile w górę
- **Testimonial Kamili**: we wszystkich wersjach
- **Case study 45k zł**: we wszystkich wersjach
- **Instagram/email**: placeholder do uzupełnienia później
- **Ikony usług**: emoji 💎🔄⚙️🚀zastąpione dedykowanymi ikonami (SVG/CSS/Material Symbols) dopasowanymi stylistycznie do palety i estetyki danej wersji — każda wersja ma spójne ikony, nie generyczne emoji

### Formularz kontaktowy

- Wersje 1, 3, 5, 7, 9: tylko CTA z Calendly
- Wersje 2, 4, 6, 8, 10: CTA + prosty formularz kontaktowy (imię, email, wiadomość) — frontend only, bez backendu

### Struktura plików

```
kinga_homepage/
├── index.html                          # obecna wersja (nietknięta)
├── strona www - finalna wersja 09.04. .md
├── v01-szalwia/
│   └── index.html
├── v02-jungle/
│   └── index.html
├── v03-herbarium/
│   └── index.html
├── v04-ogrod/
│   └── index.html
├── v05-bamboo/
│   └── index.html
├── v06-greenhouse/
│   └── index.html
├── v07-terracotta/
│   ├── index.html
│   ├── uslugi.html
│   ├── o-mnie.html
│   └── kontakt.html
├── v08-moss/
│   └── index.html
├── v09-wildflower/
│   └── index.html
└── v10-eucalyptus/
    ├── index.html
    ├── uslugi.html
    ├── o-mnie.html
    └── kontakt.html
```

### Favicon / meta tags

- Pomijamy — nie dotyczy tego etapu

### Kolejność implementacji

1. Zapisać PRD jako `prd.md` w katalogu projektu
2. Budujemy po kolei: v01 → v02 → ... → v10. Każda wersja to osobny commit.

## Testing Decisions

- Każda wersja testowana w przeglądarce (dev server)
- Test mobile viewport (375px) + desktop (1440px)
- Weryfikacja: CTA linki działają, nawigacja działa, treść kompletna
- Porównanie wizualne między wersjami

## Out of Scope

- Backend / formularz z wysyłką
- CMS / system zarządzania treścią
- SEO optymalizacja
- Analytics
- Hosting / deployment
- Instagram i email linki (dodane później)
- Favicon i meta tags

## Further Notes

- Elementy roślinne tworzone jako inline SVG lub CSS — bez zewnętrznych obrazków
- Obecny `index.html` pozostaje nietknienty
- User mówi po polsku — treść strony po polsku
