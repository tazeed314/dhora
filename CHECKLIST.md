# CHECKLIST — Site Dhora Ghimouze (refonte « Porta »)

Refonte visuelle inspirée de Porta : carte crème sur canevas lavande, titres fins avec un mot accentué en gras, boutons pilule, cartes couleur, chiffres 01/03, panneau jaune et cartes « bulle ».

## Design system (TERMINÉ)
- [x] Canevas lavande `#F1EFF4`, carte crème `#FDF6EA`, encre `#211231`
- [x] Accent violet `#501D7A`, jaune soleil `#FADB86`, gris doux `#685E76`
- [x] Typographie unique **Zain** (latin + arabe), poids 200 à 700
- [x] CSS 100 % custom, aucun framework
- [x] Composants : `.page`, `.topbar`, `.hero`, `.visual-panel`, `.color-card`, `.steps`, `.statement`, `.sun-panel`, `.bubbles`, `.faq-grid`, `.form-card`
- [x] Hero visuel : panneau jaune « 10 décembre 2026 » + carte flottante (90 min / 20h00 Alger / en ligne / gratuit)
- [x] Courbes décoratives discrètes dans le panneau jaune (pas de blueprint, pas de sceau, pas de compte à rebours)

## Structure & contenu (TERMINÉ)
- [x] Barre haute : marque, nav, FR/عربي, bouton « Réserver ma place », menu mobile
- [x] Hero : accroche, 2 CTA, 3 chiffres clés
- [x] Services : 3 grandes cartes couleur (violet / jaune / noir)
- [x] Méthode : 3 colonnes numérotées 01/03 → 03/03
- [x] Citation signature en gros texte fin
- [x] À propos : récit + panneau « En bref » (sans photo)
- [x] Masterclass : panneau jaune, 3 cartes bulle (apprendre / public / après inscription) + CTA
- [x] FAQ : 5 questions en cartes bulle, 2 colonnes, accordéon
- [x] Contact : coordonnées + formulaire WhatsApp
- [x] Footer

## Mobile-first (TERMINÉ)
- [x] Menu mobile plein écran (ouverture/fermeture, Échap, fermeture au clic)
- [x] Hero empilé : panneau jaune puis carte d'infos puis texte
- [x] Services en défilement horizontal avec accroche (scroll-snap)
- [x] Grilles qui s'empilent (méthode, à propos, bulles, FAQ, contact)
- [x] Zones tactiles confortables
- [x] Vérifié à 600 px (Chrome headless ignore les largeurs < 500 px)

## Interactivité (TERMINÉ)
- [x] Accordéon FAQ accessible (`aria-expanded`, une seule ouverte)
- [x] Formulaire : nom, téléphone, e-mail facultatif, profession, wilaya, message → ouvre WhatsApp avec le texte prérempli
- [x] Aucun faux backend, aucun faux succès : message clair « il ne reste qu'à envoyer »
- [x] Masquage du bouton d'inscription une fois la date passée (10/12/2026 20:00 UTC+1)
- [x] Révélation au scroll (respecte `prefers-reduced-motion`)

## SEO & technique (TERMINÉ)
- [x] Meta title/description, Open Graph, Twitter Card
- [x] JSON-LD (ProfessionalService + Person)
- [x] `sitemap.xml`, `robots.txt`
- [x] Page 404 au nouveau design
- [x] Accessibilité (skip link, focus visible, aria, libellés de formulaire)

## Bilingue FR / AR (TERMINÉ)
- [x] `ar.html` complet, `lang="ar"` + `dir="rtl"`
- [x] Sélecteur FR / عربي dans l'en-tête et le menu mobile
- [x] Même police Zain pour les deux langues
- [x] Ajustements RTL (flèches, puces, panneau jaune, carte flottante, champs téléphone/e-mail en LTR)
- [x] `hreflang` + `sitemap.xml` bilingue
- [x] Traduction complète de toutes les sections

## Page Formations (TERMINÉ)
- [x] `formations.html` (FR) + `formations-ar.html` (AR, RTL), même coque visuelle
- [x] Note : ouverture au-delà des entrepreneurs BTP, formations à venir, certaines payantes/gratuites
- [x] 4 thématiques en grille 2×2 avec badges Gratuit / Payant / Bientôt
- [x] Bandeau jaune de rappel vers la masterclass
- [x] Liens croisés FR ↔ AR

## Coordonnées (TERMINÉ)
- [x] Téléphone + WhatsApp : **+213 668 11 33 66**
- [x] Aucune adresse e-mail inventée : WhatsApp remplace le mailto
- [x] Inscription masterclass : `https://dhoraghimouze.systeme.io/inscription-11-2026`

## Masterclass
- Date unique : **jeudi 10 décembre 2026, 20h00 heure d'Alger (UTC+1)**
- En ligne, 90 minutes, gratuit
- [x] Date identique dans le hero, le panneau jaune, la FAQ, la page formations et la page arabe
- [ ] Mettre à jour la page Systeme.io (contenu FR fourni séparément)

## À fournir par vous (assets personnels)
- [ ] Vraie photo (facultative) — `assets/portrait.webp` est une silhouette non utilisée
- [ ] Vrais témoignages (section à ajouter quand disponibles)
- [ ] Favicon .png/.ico (optionnel ; lettre « D » en SVG actuellement)

## Déploiement
- [x] Dépôt GitHub : https://github.com/tazeed314/dhora (branche `main`)
- [x] Cloudflare Pages, projet `dhorra` → **https://dhorra.pages.dev**
- [ ] Le site en ligne sert encore l'ancien design : pousser après validation
- [ ] Tester mobile / tablette / desktop en ligne
- [ ] Domaine personnalisé (si disponible)

## Fichiers
- index.html — accueil FR
- ar.html — accueil AR (RTL)
- formations.html / formations-ar.html — pages formations
- css/style.css — design system complet
- 404.html — page d'erreur
- sitemap.xml, robots.txt

## Exclus du dépôt (`.gitignore`)
- `Chantier Aligné.pdf` — document privé
- `pdf_text.txt`, images sources non utilisées
