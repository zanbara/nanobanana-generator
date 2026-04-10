# 🍌 Nano Banana Generator

**Outil SaaS de génération de prompts marketing pour l'e-commerce mobile COD**

[![Version](https://img.shields.io/badge/version-4.0%20Pro-b5f23c?style=flat-square)](.)
[![Langue](https://img.shields.io/badge/langues-8%20marchés-blue?style=flat-square)](.)
[![Licence](https://img.shields.io/badge/licence-MIT-green?style=flat-square)](.)
[![Deploy](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)](.)

---

## 📌 À propos du projet

**Nano Banana Generator** est une application web mono-fichier conçue pour aider les e-commerçants à générer rapidement trois types de contenus marketing prêts à l'emploi :

1. **Prompts de landing page** pour le générateur d'images Nano Banana
2. **Scripts vidéo** pour les créatifs TikTok, Reels et Facebook Ads
3. **Fiches produit complètes** prêtes à coller sur YouCan ou Shopify

L'application fonctionne **100% côté navigateur**, sans serveur, sans base de données, sans clé API. Un seul fichier HTML suffit.

---

## 🎯 Cas d'usage

- Vendeurs e-commerce COD en Afrique francophone, au Maroc et dans les pays du Golfe
- Créateurs de landing pages sur [YouCan](https://youcan.shop)
- Marketeurs cherchant à générer du contenu culturellement adapté à leur marché cible
- Dropshippers internationaux (FR, EN, ES, IT, DE)

---

## ✨ Fonctionnalités

### 🍌 Module 1 — Landing Prompt Generator
Génère un prompt visuel ultra-long (ratio 9:32) pour Nano Banana, structuré en 9 sections :

| Section | Contenu |
|---|---|
| Hero / WOW | Titre fort, produit en avant, badge "Nouveauté" |
| Problème | Question douleur, icônes frustration |
| Solution | Révélation produit avec aura lumineuse |
| Avant / Après | Contraste visuel gauche/droite |
| Features | Close-up produit + badges caractéristiques |
| Comparaison | Notre produit vs concurrent |
| Lifestyle | Personnage du marché cible en action |
| Avis clients | Stars + noms locaux + avatars culturels |
| CTA final | Bouton commande + urgence stock |

### 🎬 Module 2 — Video Script Generator
Génère **3 scénarios distincts** (Direct / Émotionnel / Agressif), chacun composé de :
- 🎣 **Hook** (3–6 sec) — durée contrôlée par slider
- 📣 **Body** (12–25 sec) — durée contrôlée par slider
- 🛒 **CTA** (3–6 sec) — durée contrôlée par slider

Options disponibles :
- **6 angles marketing** : Douleur, Transformation, Opportunité, FOMO, Preuve sociale, Curiosité
- **4 formats vidéo** : Face cam UGC, Voice Over + B-Roll, Storytelling, Démo produit
- Détection automatique du type de produit (résolution de problème vs effet Wow)

### 📝 Module 3 — Product Page Copy Generator
Génère une **fiche produit complète** en 7 sections (section 7 visuelle uniquement) :

| # | Section |
|---|---|
| 1 | Titre WOW + Introduction |
| 2 | Description produit |
| 3 | Comment utiliser |
| 4 | Caractéristiques & Avantages |
| 5 | Avant / Après |
| 6 | Pourquoi choisir ce produit |
| 8 | Avis clients (cartes visuelles) |

Options :
- **6 tons de copywriting** : Réponse directe, Premium, Émotionnel, Problème/Solution, Friendly/Trust, Curiosité
- **3 longueurs** : Court, Moyen, Long
- Toggle titres auto-générés
- Toggle version alternative B

---

## 🌍 Marchés et langues supportés

| Drapeau | Marché | Langue | Avatars |
|---|---|---|---|
| 🌍 | Afrique francophone COD | Français | Personnages africains subsahariens |
| 🇲🇦 | Maroc — Local COD | Darija marocaine | Personnages marocains |
| 🇸🇦 | Pays du Golfe | Arabe du Golfe | Personnages moyen-orientaux |
| 🌐 | Global — Dropshipping | Anglais | Personnages diversifiés |
| 🇫🇷 | France & Europe | Français standard | Personnages européens |
| 🇪🇸 | Amérique latine & Espagne | Espagnol | Personnages latinos |
| 🇮🇹 | Italie | Italien | Personnages italiens |
| 🇩🇪 | Allemagne & Europe centrale | Allemand | Personnages germaniques |

Chaque marché adapte automatiquement : les textes, les prénoms, les villes de référence, les avatars culturels et le ton persuasif.

---

## 🚀 Installation et déploiement

### Utilisation locale
Aucune installation requise. Téléchargez `index.html` et ouvrez-le dans un navigateur.

```bash
# Cloner le dépôt
git clone https://github.com/zanbara/nanobanana-generator.git

# Ouvrir directement dans le navigateur
open index.html
```

### Déploiement GitHub Pages
1. Forkez ou clonez ce dépôt
2. Renommez le fichier principal en `index.html`
3. Allez dans **Settings → Pages**
4. Sélectionnez la branche `main` comme source
5. Votre app sera disponible sur `https://votre-username.github.io/nanobanana-generator`

### Déploiement Netlify (drag & drop)
1. Allez sur [netlify.com/drop](https://app.netlify.com/drop)
2. Glissez-déposez le fichier `index.html`
3. Votre URL publique est générée instantanément

---

## 🖥️ Stack technique

| Technologie | Usage |
|---|---|
| HTML5 | Structure de l'application |
| CSS3 (variables, grid, flexbox) | Design system complet |
| JavaScript vanilla (ES6+) | Logique métier et génération |
| [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) | Police principale (titres) |
| [DM Sans](https://fonts.google.com/specimen/DM+Sans) | Police corps de texte |
| Google Fonts CDN | Chargement des polices |

**Zéro dépendance externe.** Aucun framework, aucune librairie JS, aucun appel API.

---

## 📁 Structure du projet

```
nanobanana-generator/
│
├── index.html          # Application complète (fichier unique)
└── README.md           # Documentation du projet
```

---

## 🧠 Architecture de l'application

```
INPUT PANEL (gauche)
├── Section 1  — Langue du marché cible
├── Section 2  — Type d'offre (Single / Bundle)
├── Section 3  — Caractéristiques du produit
├── Section 4  — Avis clients (manuel ou auto-généré)
├── ── Module Script Vidéo ──
├── Section 5  — Angle marketing
├── Section 6  — Format vidéo
├── Section 7  — Durée des parties (sliders)
├── ── Module Fiche Produit ──
├── Section 8  — Ton de copywriting
├── Section 9  — Longueur des sections
└── Section 10 — Options avancées

OUTPUT PANEL (droite)
├── Tab 1 🍌  Landing Prompt
├── Tab 2 🎬  Scripts Vidéo (3 scénarios)
└── Tab 3 📝  Fiche Produit (7 sections)
```

---

## 📸 Aperçu

> L'interface est en dark mode premium avec une palette `#0c0c0f` (fond) et `#b5f23c` (accent vert Nano Banana).

**Modules accessibles via les onglets du panel de droite :**

- **🍌 Landing Prompt** — prompt prêt à coller dans Nano Banana
- **🎬 Scripts Vidéo** — 3 scénarios Hook/Body/CTA collapsibles
- **📝 Fiche Produit** — sections copiables individuellement ou en bloc

---

## ⚙️ Personnalisation

Pour adapter l'application à votre marque ou ajouter un nouveau marché, modifiez le tableau `LANGS` dans la section `<script>` de `index.html` :

```javascript
{
  code: 'votre-code',
  flag: '🏳️',
  name: 'Nom du marché',
  mkt: 'Description courte',
  avatar: 'Description des personnages pour les prompts',
  names: ['Prénom1', 'Prénom2', ...],
  cities: ['Ville1, Pays', 'Ville2, Pays', ...],
  ctaDefault: 'Texte du bouton CTA',
  urgency: '⚠️ Message d\'urgence',
  trust: 'Badges de confiance',
  lang: 'Langue de génération',
  visuals: 'Description du contexte visuel',
  tone: 'Ton de copywriting',
  textSample: { hero: '...', problem: '...', solution: '...', cta: '...' }
}
```

---

## 🗺️ Feuille de route

- [ ] Export de l'historique des prompts générés
- [ ] Sauvegarde des modèles favoris (localStorage)
- [ ] Support Shopify avec sections de thème prédéfinies
- [ ] Ajout de nouveaux marchés (Portugal, Sénégal Wolof, Turquie)
- [ ] Mode dark/light toggle
- [ ] Export PDF de la fiche produit

---

## 🤝 Contribution

Les contributions sont les bienvenues. Pour proposer une amélioration :

1. Forkez le dépôt
2. Créez une branche : `git checkout -b feature/nouvelle-fonctionnalite`
3. Commitez vos changements : `git commit -m 'Ajout de la fonctionnalité X'`
4. Poussez la branche : `git push origin feature/nouvelle-fonctionnalite`
5. Ouvrez une Pull Request

---

## 📄 Licence

Ce projet est distribué sous licence **MIT**. Voir le fichier `LICENSE` pour plus de détails.

---

## 👤 Auteur

Développé par **[@zanbara](https://github.com/zanbara)**

> Outil conçu pour les e-commerçants COD des marchés francophones africains, marocains et du Golfe.

---

<div align="center">
  <sub>Fait avec ❤️ pour l'e-commerce mobile africain et maghrébin</sub>
</div>
