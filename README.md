# 🎯 THL Strat Board

Tableau de coach de la team **THL (Try Hard Life)** pour préparer les scrims **Battlefield 6** en mode **Domination** (4v4 / 5v5).

Le principe est le même qu'un entraîneur qui dessine la tactique au tableau : tu importes la carte, tu places les joueurs et les drapeaux, tu dessines les déplacements, puis tu exportes la strat en image pour la poster sur Discord.

👉 **Utiliser l'outil :** https://leodevtech.github.io/thl-strat-board/

---

## ✨ Fonctionnalités

| Outil | Raccourci | Description |
|---|---|---|
| Déplacer | `V` | Sélectionner et déplacer n'importe quel élément |
| Pion joueur | `J` | Pions numérotés de 1 à 5, en **bleu** (nous) ou en **rouge** (adversaire), avec un **champ de vision de 65°** pour montrer où regarder |
| Drapeau | `D` | Drapeaux **A / B / C**, en jaune (neutre), bleu (à nous) ou rouge (à eux) |
| Dessin libre | `P` | Tracé à main levée, plein ou en pointillé |
| Flèche | `F` | Rushs, rotations, contournements |
| Ping | `G` | Signaler un point précis (angle, danger, cible) |
| Cône de vision | `C` | Zone transparente pour définir une ligne à tenir, avec ouverture réglable de 15° à 180° |
| Smoke | `S` | **Petit nuage** pour pinguer où smoker, ou **zone de fumée** en grand |
| Grenade | `N` | Zone d'explosion avec l'icône de la grenade |
| Texte | `T` | Callouts sur la carte (TRANSIT, JUNGLE…), inclinables pour suivre une rue |
| Gomme | `E` | Effacer un élément au clic ou au glisser |

### 🎨 Couleurs des rôles
Les pions alliés prennent automatiquement la couleur de leur rôle (case **« Couleurs des rôles »**) :

| Pion | Couleur | Rôle |
|---|---|---|
| 1 | 🔵 Bleu | Ancre AC |
| 2 | 🟢 Vert | Flex AC |
| 3 | 🟠 Orange | Entry B |
| 4 | 🔴 Rouge | Support B |
| 5 | 🟣 Violet | Ancre B |

Ces 5 couleurs sont aussi disponibles pour le **stylo**, les **flèches**, les **pings** et les **cônes**, pour dessiner le trajet de chaque joueur dans sa couleur. Un pion allié sélectionné peut aussi changer de couleur à la main.

### 👁️ Champ de vision des pions
- Pose le pion, puis **glisse sans lâcher** vers l'endroit où il doit regarder.
- Pour le réorienter, sélectionne le pion et attrape le **rond blanc** au bout du cône.
- La case **« Champ de vision 65° »** l'active ou le désactive.

### 🔤 Texte
- Touche la carte à l'endroit voulu, écris, puis valide avec **Entrée**.
- Pour l'**incliner** le long d'une rue, sélectionne le texte et fais tourner le **rond blanc** au bout (l'angle s'aimante tous les 15°).
- Pour corriger un texte, sélectionne-le et modifie-le dans le panneau. La couleur et la taille se changent aussi depuis le panneau.

### ☁️ Smokes et grenades
- **Clic simple** : l'objet est posé au point d'impact.
- **Glisser du lanceur vers l'impact** : la trajectoire s'affiche en pointillé.
- **Pivoter la trajectoire** : sélectionne la smoke ou la grenade, puis attrape le **rond blanc** au point de lancer. La trajectoire pivote autour du nuage. Ramène le rond sur le nuage pour supprimer la trajectoire.

**Et aussi :**
- 🗺️ Import de **n'importe quelle carte** : bouton, glisser-déposer ou `Ctrl+V` d'une capture d'écran
- 🔢 Touches `1` à `5` pour choisir directement le numéro du pion
- 📐 Grille tactique optionnelle (A–J / 1–10) pour les callouts
- 🔍 Zoom à la molette ou au pincement, déplacement de la carte au clic droit ou avec `Espace` + glisser
- ↩️ Annuler / rétablir (`Ctrl+Z` / `Ctrl+Y`)
- 🖼️ **Export PNG** en haute résolution avec un bandeau THL (nom de la strat, carte, date)
- 📋 **Copier l'image** pour la coller directement dans Discord
- 💾 **Sauver / ouvrir une strat** au format `.json`, carte et annotations comprises, pour la reprendre plus tard ou l'envoyer à un mate

---

## 🚀 Utilisation rapide

1. Ouvre l'outil dans ton navigateur (PC ou mobile).
2. Clique sur **Importer une carte** et choisis ta capture de la map.
3. Donne un nom à ta **strat** (par exemple « Spawn ouest · prise de B »).
4. Place les drapeaux A, B et C, puis tes pions 1 à 5 en les orientant vers l'angle à tenir.
5. Dessine les flèches de déplacement, puis ajoute les smokes, les grenades et les pings.
6. Clique sur **Exporter l'image**, puis sur **Copier l'image**, et colle-la dans Discord.

> 💡 Chacun travaille sur sa propre copie, dans son navigateur. Pour partager une strat modifiable, envoie le fichier `.json` obtenu avec **Sauver la strat**. Ton mate l'ouvre ensuite avec **Ouvrir une strat**.

---

## 📝 Nouveautés

- **Novembre 2026** : outil Texte pour les callouts, couleurs des rôles (pions, stylo, flèches, pings), trajectoire des smokes et grenades réglable avec une poignée, champ de vision de 65° sur les pions, cône de vision réglable, smoke (petit nuage ou zone) et grenade avec trajectoire de lancer.
- **Octobre 2026** : première version (pions, drapeaux, dessin, flèches, ping, export PNG, sauvegarde `.json`).

---

## 🛠️ Technique

- Un seul fichier `index.html`, en HTML, CSS et JavaScript vanilla, avec un rendu sur `<canvas>`
- Aucune dépendance, aucun build, aucun serveur
- Tout se passe en local dans le navigateur : aucune carte ni strat n'est envoyée en ligne
- Hébergement via **GitHub Pages**

### Lancer en local

Clone le dépôt, puis ouvre `index.html` dans ton navigateur :

```bash
git clone https://github.com/leodevtech/thl-strat-board.git
cd thl-strat-board
# puis double-clic sur index.html
```

---

## 👥 Team

Développé pour la team **THL – Try Hard Life** par [Léo DevTech](https://leodevtech.fr).

Une idée d'amélioration ou un bug ? Ouvre une *issue* ou passe le message sur le Discord de la team.
