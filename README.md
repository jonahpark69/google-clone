# 🔎 Exercice — Reproduire la homepage de **Google**

> Exercice scolaire : **reproduction statique** de la page d’accueil de google.com (mise en page, hiérarchie, interactions de base). Projet purement **pédagogique**, sans usage de marques/ressources propriétaires en production.

---

## 📑 Sommaire

* [Aperçu](#-aperçu)
* [Objectifs pédagogiques](#-objectifs-pédagogiques)
* [Contraintes de l’exercice](#-contraintes-de-lexercice)
* [Fonctionnalités réalisées](#-fonctionnalités-réalisées)
* [Stack & démarrage](#-stack--démarrage)
* [Arborescence](#-arborescence)
* [Notes techniques](#-notes-techniques)
* [Accessibilité & SEO](#-accessibilité--seo)
* [Captures](#-captures)
* [Améliorations possibles](#-améliorations-possibles)
* [Licence & mentions](#-licence--mentions)

---

## 👀 Aperçu

Reproduction **front-only** de la page d’accueil de Google : **logo**, **barre de recherche**, **boutons d’action**, **en‑tête** et **footer**.

---

## 🎯 Objectifs pédagogiques

* Structurer une page avec **HTML sémantique**.
* Maîtriser **CSS Grid/Flexbox** pour l’alignement central.
* Recréer une **UI fidèle** (espacements, tailles, focus states).
* Gérer **responsive** simple (desktop → mobile).

---

## 📏 Contraintes de l’exercice

* **Pas de framework** (pas de Bootstrap/Tailwind).
* **Pas de JS** (ou **JS minimal** uniquement pour l’UX, si autorisé).
* **Aucune dépendance externe** obligatoire (fonts système ok).
* **Pas d’assets propriétaires** : logo/illustrations **recréés** en placeholder si nécessaire.

---

## ✨ Fonctionnalités réalisées

* Barre de recherche **centrée** avec icônes (loupe, micro, lens placeholders).
* Boutons **“Recherche Google”** et **“J’ai de la chance”**.
* En‑tête : liens de navigation (Gmail, Images) + avatar placeholder.
* Footer : liens pays/infos (maquette).
* **Focus/hover states** cohérents.
* **Responsive** (empilement propre sur mobile).

---

## 🧱 Stack & démarrage

* **HTML5 / CSS3** (vanilla)
* (Optionnel) **JS** léger pour interactions (non requis)

**Démarrage local**

```bash
# Lancer un serveur statique simple (au choix)
python3 -m http.server 5173
# ou
npx serve .
# puis ouvrir http://localhost:5173
```

---

## 🌲 Arborescence

```
exercise-google-homepage/
├─ assets/
│  ├─ css/style.css
│  ├─ js/main.js         # (optionnel)
│  └─ images/            # placeholders (logo, icônes)
├─ index.html            # page d'accueil
└─ README.md
```

---

## 🛠️ Notes techniques

* **Layout principal** centré via Flexbox (body → min-height: 100vh).
* **Search bar** : conteneur arrondi, icônes en pseudo‑éléments ou SVG inline.
* **Grille** : zones header/main/footer ; espacement via `gap`/`margin` simples.
* **Typo** : pile **system‑ui** (compatibilité GitHub/OS).
* **Unités** : `px` / `rem`, pas de `clamp()` pour rester lisible.

---

## ♿ Accessibilité & SEO

* Attributs `aria-label` sur la barre de recherche et les boutons.
* Ordre de tabulation logique, **focus-ring visible**.
* `alt` sur images/icônes, `lang="fr"` dans `<html>`.
* Meta de base : `title`, `meta viewport`.

---

## 📸 Captures

*(À ajouter)*

* Vue desktop
* Vue mobile
* Focus sur barre de recherche

---

## 🗺️ Améliorations possibles

* Simuler une **liste de suggestions** (JS optionnel).
* Ajouter une **version sombre**.
* Renforcer la **prise en charge clavier** et lecteurs d’écran.

---

## 📜 Licence & mentions

* Projet **pédagogique** — **non affilié** à Google.
* Marque et logos **appartiennent à leurs détenteurs** ; les versions utilisées ici sont **placeholders** de démonstration.
* Licence : **privé** (exercice de formation).
