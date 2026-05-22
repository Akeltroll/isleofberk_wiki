# Manifeste des médias — Codex Draconum

Liste exhaustive des fichiers à déposer pour que tous les slots d'image s'affichent.
**Aucun fichier n'est obligatoire** : tant qu'un fichier manque, le slot affiche son
placeholder (hachure or + indication du chemin attendu).

---

## Arborescence à créer

```
website/
  assets/
    dragons/            (renders, déjà existants à renommer si besoin)
    screenshots/        (captures en jeu)
    icons/              (icônes d'items)
    hero_dragon.png     (image hero d'accueil)
```

---

## 1. Hero d'accueil (1 image)

| Chemin                                | Notes                                                          |
|---------------------------------------|----------------------------------------------------------------|
| `assets/hero_dragon.png`              | PNG transparent ~1200×600, centré dans le hero, derrière titre |

> Un stub transparent 2×2 est déjà en place pour éviter le 404.
> Remplace-le par ton image quand tu es prêt.

---

## 2. Renders de spécimens (13 images — bestiaire & cards d'accueil)

Format conseillé : `.webp`, ratio 3/4 ou libre, hauteur min. 600px.

| Chemin                          | Spécimen           | Folio   |
|---------------------------------|--------------------|---------|
| `assets/dragons/specimen-01.webp` | I — le Cendreux            | ᚠ |
| `assets/dragons/specimen-02.webp` | II — le Dardé              | ᚢ |
| `assets/dragons/specimen-03.webp` | III — l'Échinée            | ᚦ |
| `assets/dragons/specimen-04.webp` | IV — le Lourdaut           | ᚬ |
| `assets/dragons/specimen-05.webp` | V — le Foudroyeur          | ᚱ |
| `assets/dragons/specimen-06.webp` | VI — le Tridenté           | ᚴ |
| `assets/dragons/specimen-07.webp` | VII — Voilier d'Ombre      | ᚼ |
| `assets/dragons/specimen-08.webp` | VIII — Voilier d'Aube      | ᚾ |
| `assets/dragons/specimen-09.webp` | IX — le Crépusculaire      | ᛁ |
| `assets/dragons/specimen-10.webp` | X — l'Embraseur            | ᛅ |
| `assets/dragons/specimen-11.webp` | XI — Jumeau Brumeux        | ᛋ |
| `assets/dragons/specimen-12.webp` | XII — le Fil-de-Vent       | ᛏ |
| `assets/dragons/specimen-13.webp` | XIII — l'Alpha-Vent        | ᛒ |

Affecté sur : `bestiaire.html`, `index.html` (showcase), `dragons/_template.html` (hero).

---

## 3. Captures en jeu (~26–52 images — pages dragon)

Format conseillé : `.webp`, ratio 16/9, largeur min. 1280px.

Par dragon, 2 à 4 captures. Nommage : `specimen-NN_M.webp` (M = numéro de capture).

| Chemin type                                 | Suggestion de contenu              |
|---------------------------------------------|------------------------------------|
| `assets/screenshots/specimen-07_01.webp`    | Vol nocturne au-dessus des sommets |
| `assets/screenshots/specimen-07_02.webp`    | Charge de la décharge principale   |
| `assets/screenshots/specimen-07_03.webp`    | Premier contact, au crépuscule     |
| `assets/screenshots/specimen-07_04.webp`    | Variante rare relevée              |
| `assets/screenshots/specimen-07_thumb.webp` | Poster de la vidéo (16/9)          |

Réplique le pattern pour chaque spécimen. Le template `dragons/_template.html`
prévoit 4 figures par défaut — tu peux en ajouter ou en retirer.

---

## 4. Captures de nids (4 images — page nids.html)

Format conseillé : `.webp`, ratio 16/10.

| Chemin                                  | Contenu                  |
|-----------------------------------------|--------------------------|
| `assets/screenshots/nest_jungle.webp`   | Nid de Jungle            |
| `assets/screenshots/nest_ice.webp`      | Nid des Glaces           |
| `assets/screenshots/nest_cave.webp`     | Nid de Caverne           |
| `assets/screenshots/nest_taiga.webp`    | Nid de Taïga             |

---

## 5. Vidéos d'aperçu (13 fichiers facultatifs — pages dragon)

Format : `.mp4` H.264, ratio 16/9, durée 5–15 s, sans audio.

| Chemin                                | Spécimen |
|---------------------------------------|----------|
| `assets/videos/specimen-NN.mp4`       | N de 01 à 13 |

Le `<video>` a un fallback stylisé "Vidéo à venir" tant que le fichier manque.

---

## 6. Icônes d'items (~25 images — page dressage.html)

Format conseillé : `.png` carré 64×64 ou 128×128, fond transparent.
Utilise le rendu pixelisé (Minecraft style).

### Nourritures de taming
| Chemin                              | Item                |
|-------------------------------------|---------------------|
| `assets/icons/salmon.png`           | Saumon              |
| `assets/icons/cod.png`              | Morue               |
| `assets/icons/tropical_fish.png`    | Poisson tropical    |
| `assets/icons/mutton.png`           | Mouton (raw/cooked) |
| `assets/icons/chicken.png`          | Poulet              |
| `assets/icons/beef.png`             | Bœuf                |

### Potions (Tier IV)
| Chemin                                       | Potion             |
|----------------------------------------------|--------------------|
| `assets/icons/potion_night_vision.png`       | Vision Nocturne    |
| `assets/icons/potion_invisibility.png`       | Invisibilité       |
| `assets/icons/potion_fire_resistance.png`    | Résistance au Feu  |
| `assets/icons/potion_strength.png`           | Force              |
| `assets/icons/potion_awkward.png`            | Potion neutre      |

### Items du mod
| Chemin                                  | Item                          |
|-----------------------------------------|-------------------------------|
| `assets/icons/belzium.png`              | Minerai liant (Belzium)       |
| `assets/icons/raw_gronckle_iron.png`    | Fer de pierre brut            |
| `assets/icons/gronckle_iron.png`        | Fer de pierre affiné          |
| `assets/icons/dragon_staff.png`         | Bâton du dresseur             |
| `assets/icons/love_filter.png`          | Philtre liant                 |
| `assets/icons/scale_compass.png`        | Écaille-Compas                |

### Ingrédients de recette
| Chemin                              | Item              |
|-------------------------------------|-------------------|
| `assets/icons/amethyst.png`         | Améthyste         |
| `assets/icons/stick.png`            | Bâton (vanille)   |
| `assets/icons/stone_blocks.png`     | Granite/diorite/deepslate/stone |
| `assets/icons/glowstone.png`        | Glowstone         |
| `assets/icons/sandstone.png`        | Sandstone         |
| `assets/icons/iron_ingot.png`       | Lingot de fer     |
| `assets/icons/name_tag.png`         | Name Tag          |

---

## Comment fonctionne le système de slots

### Slot image (`.img-slot`)

```html
<div class="img-slot" style="--src: url('assets/screenshots/foo.webp')">
  <span class="img-slot__path">assets/screenshots/foo.webp</span>
</div>
```

- L'image est définie via la variable CSS `--src`.
- Tant que le fichier n'existe pas, le slot affiche une hachure + le chemin attendu.
- Une fois l'image en place, elle remplit automatiquement le slot.
- Pour cacher l'indication de chemin, supprimer le `<span class="img-slot__path">`
  ou ajouter la classe `img-slot--ok` sur le conteneur.

Variantes d'aspect-ratio :
- `.img-slot--portrait` (3/4)
- `.img-slot--square` (1/1)
- `.img-slot--cinema` (21/9)
- `.img-slot--tall` (2/3)

### Item icon (`.item-icon`)

```html
<span class="item-icon" style="--icon: url('assets/icons/salmon.png')">Saumon</span>
```

- Icône 28×28 par défaut, pixelisée (rendu Minecraft).
- Tant que l'image manque, la case affiche une hachure or.
- Variantes : `.item-icon--sm` (22px), `.item-icon--lg` (36px), `.item-icon--block`
  (effet bloc avec inner-shadow).
- Attribut optionnel `data-qty="30"` ajoute "× 30" en suffixe.

### Image directe (bestiaire, hero dragon)

```html
<img src="assets/dragons/specimen-07.webp"
     alt="Spécimen VII"
     loading="lazy"
     onerror="this.remove()">
```

- Si le fichier manque, l'`onerror` supprime l'image et le placeholder reste visible.

---

## Astuce de migration

Si tu as déjà tes 13 renders avec d'autres noms (par ex. `nightfury.webp`), il y a
deux options :

**Option A — Renommer tes fichiers** vers `specimen-01.webp` ... `specimen-13.webp`
selon le mapping de la section 2 ci-dessus. Aucune modification de code nécessaire.

**Option B — Réécrire les chemins dans le code** : ouvre `bestiaire.html`,
`index.html`, `dragons/_template.html` et fais un find-and-replace
`specimen-07.webp` → `nightfury.webp` (par exemple).

L'option A est plus simple si tu en as 13 à mapper.
