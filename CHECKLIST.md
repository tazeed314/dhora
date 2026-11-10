# CHECKLIST — Site Dhora Ghimouze (refonte premium, sans logo)

Refonte dramatique : design éditorial haut de gamme, mobile-first, marque personnelle (pas de logo).

## Design system (TERMINÉ)
- [x] Palette premium : bleu nuit (`#14161f`) + or (`#b08948`) + crème (`#f7f3ec`)
- [x] Typographie : Fraunces (titres éditoriaux) + Inter (corps)
- [x] CSS 100% custom (plus de CDN Tailwind) → rapide, cohérent, unique
- [x] Composants : boutons, cartes, piliers, diagramme, accordéon, formulaires
- [x] Hero visuel : SVG d'architecture (blueprint) sur mesure — pas d'image externe
- [x] Sceau "A·O·S" (Anticiper / Organiser / Sécuriser)

## Structure & contenu (TERMINÉ)
- [x] Header fixe avec état au scroll, marque textuelle + tagline
- [x] Hero : accroche éditoriale, 2 CTA, 3 chiffres clés
- [x] Bandeau thématique (contrats, marchés, assurances, sous-traitance, BTP)
- [x] Méthode en 3 piliers numérotés (01/02/03)
- [x] Diagramme d'alignement : Contrat + Assurance + Sous-traitant → Marge sécurisée
- [x] Bande citation signature (fond sombre)
- [x] À propos : portrait (placeholder) + récit en blocs + faits (ville, métier, spécialisation)
- [x] Services : 3 cartes (conseil juridique, formation & webinars, accompagnement chantier)
- [x] Masterclass : section sombre de conversion (date, compte à rebours, bénéfices, présenté par)
- [x] FAQ : accordéon (4 questions)
- [x] Contact : coordonnées + formulaire (mailto, pas de faux backend)
- [x] Footer complet

## Mobile-first (TERMINÉ)
- [x] Menu mobile plein écran (ouverture/fermeture, overlay z-index, fermeture au clic)
- [x] Boutons pleine largeur sur petit écran
- [x] Hero : visuel recadré (4/3), sceau réduit, tailles de police ajustées
- [x] Grilles qui s'empilent (piliers, services, diagramme, contact)
- [x] Zones tactiles ≥ 48px
- [x] `overflow-x: hidden` pour éviter les débordements
- [x] Tablette (641–980px) : espacements adaptés

## Interactivité (TERMINÉ)
- [x] Compte à rebours en direct (4 cellules) + état "session à venir"
- [x] Accordéon FAQ accessible (aria-expanded, une seule ouverte)
- [x] Formulaire → prépare un mailto (honnête, pas de faux succès)
- [x] Révélation au scroll (respecte `prefers-reduced-motion`)
- [x] Header qui change au scroll

## SEO & technique (TERMINÉ)
- [x] Meta title/description, Open Graph, Twitter Card
- [x] JSON-LD (LegalService + Person)
- [x] sitemap.xml, robots.txt
- [x] Page 404 au nouveau design
- [x] Styles d'impression
- [x] Accessibilité (skip link, focus visible, aria, alt/role sur SVG)

## Bilingue FR / AR (TERMINÉ)
- [x] Page arabe complète `ar.html` avec `lang="ar"` + `dir="rtl"`
- [x] Sélecteur de langue dans l'en-tête et le menu mobile (FR / AR)
- [x] Police arabe éditoriale : Amiri (titres) + Tajawal (corps)
- [x] Ajustements RTL dans le CSS (flèches, soulignés, badge portrait, citation)
- [x] `hreflang` alternates + `sitemap.xml` bilingue
- [x] Traduction complète de toutes les sections

## Police Zain (TERMINÉ)
- [x] Police unique **Zain** (latin + arabe) sur tout le site
- [x] Liens Google Fonts mis à jour (index, ar, formations, formations-ar, 404)
- [x] Variables CSS `--serif` et `--sans` + override RTL pointent vers Zain

## En-tête desktop corrigé (TERMINÉ)
- [x] Grille `1fr auto 1fr` : marque à gauche, menu centré, actions à droite
- [x] Sélecteur de langue (FR / AR) placé à l'extrême droite, après le bouton CTA
- [x] Comportement mobile inchangé (menu plein écran)

## Page Formations (TERMINÉ)
- [x] `formations.html` (FR) + `formations-ar.html` (AR, RTL)
- [x] Note : élargissement au-delà des « Entrepreneurs BTP », formations à venir, certaines payantes/gratuites
- [x] Aperçu de 4 thématiques (droit des contrats, assurances, marchés, risques & sous-traitance) avec badges Gratuit/Payant/Bientôt
- [x] Lien « Formations / التكوينات » ajouté aux nav (desktop + mobile) et footers
- [x] Sélecteur de langue croisé entre les deux pages formations
- [x] `sitemap.xml` mis à jour (4 URLs)

## Portrait (TERMINÉ)
- [x] Image `assets/portrait.webp` intégrée dans « À propos » (FR + AR)
- Remarque : il s'agit d'une illustration silhouette (pas une photo réelle) — remplaçable par une vraie photo plus tard

## À fournir par vous (assets personnels)
- [ ] Vrai e-mail (dans Contact + lien mailto du formulaire + masterclass)
- [ ] Vrai téléphone (section Contact)
- [ ] Vrais témoignages (section à ajouter quand disponibles)
- [ ] Favicon .png/.ico (optionnel, lettre "D" actuelle sur fond nuit/or)

## Déploiement
- [ ] Pousser sur GitHub (`dhora-website`)
- [ ] Lier à Cloudflare Pages (build vide, output `/`)
- [ ] Tester mobile/tablette/desktop en ligne
- [ ] Domaine personnalisé (si disponible)

## Fichiers
- index.html — site complet
- css/style.css — design system + mobile-first
- 404.html — page d'erreur
- sitemap.xml, robots.txt
- Chantier Aligné.pdf — guide masterclass
