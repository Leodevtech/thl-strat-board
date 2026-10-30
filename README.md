# 🎯 THL Strat Board

Tableau de coach de la team **THL (Try Hard Life)** pour préparer les scrims **Battlefield 6** en mode **Domination** (4v4 / 5v5).

Le principe est le même qu'un entraîneur qui dessine la tactique au tableau : tu importes la carte, tu places les joueurs et les drapeaux, tu dessines les déplacements, puis tu exportes la strat en image pour la poster sur Discord.

👉 **Utiliser l'outil :** https://leodevtech.github.io/thl-strat-board/

---

## ✨ Fonctionnalités

| Outil | Raccourci | Description |
|---|---|---|
| Déplacer | `V` | Sélectionner et déplacer n'importe quel élément |
| Pion joueur | `J` | Pions numérotés de 1 à 5, en **bleu** (nous) ou en **rouge** (adversaire) |
| Drapeau | `D` | Drapeaux **A / B / C**, en jaune (neutre), bleu (à nous) ou rouge (à eux) |
| Dessin libre | `P` | Tracé à main levée, plein ou en pointillé |
| Flèche | `F` | Rushs, rotations, contournements |
| Ping | `G` | Signaler un point précis (angle, danger, cible) |
| Gomme | `E` | Effacer un élément au clic ou au glisser |

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
4. Place les drapeaux A, B et C, puis tes pions 1 à 5 et ceux de l'adversaire.
5. Dessine les flèches de déplacement et ajoute des pings.
6. Clique sur **Exporter l'image**, puis sur **Copier l'image**, et colle-la dans Discord.

> 💡 Chacun travaille sur sa propre copie, dans son navigateur. Pour partager une strat modifiable, envoie le fichier `.json` obtenu avec **Sauver la strat**. Ton mate l'ouvre ensuite avec **Ouvrir une strat**.

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
