# Courrier Express

Runner western du lanceur **Mes Jeux** : le cavalier du Pony Express galope dans
le désert au coucher du soleil. Tape pour sauter (double saut possible), évite
rochers et cactus, attrape les lettres ✉️ et les pièces 🪙.

Jouable sur https://pierreflory-web.github.io/courrier/

## Règles

- La vitesse augmente sans fin : la course s'arrête au premier obstacle touché.
- Lettres = points pour le lanceur · pièces = créditées directement sur ta bourse.

## Intégration au lanceur

- Charge `https://pierreflory-web.github.io/jeux/points.js` et appelle
  `MesJeux.award('courrier', lignes, { m, lettres })` en fin de course.
- Badges gérés par le lanceur : **📬 Postier** (10 lettres d'une course),
  **🐎 Grand Galop** (1 000 m), **📯 Messager Légendaire** (2 000 m).
- Défi du jour : « Attrape 10 lettres et plus » → pièces doublées.

## Structure

- `index.html` — tout le jeu (canvas plein écran, dessin cartoon western).
- `manifest.webmanifest` + `icons/` + `sw.js` — PWA installable sur iPhone.
