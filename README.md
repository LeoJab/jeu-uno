# Uno · édition ChadGang

Uno multijoueur pour le hub ChadGangGames. Un seul fichier `index.html`, aucun serveur.

- **En ligne** (dans le hub) : salles de 2 à 8 joueurs, bots possibles, via le SDK `/_sdk.js`.
  L'hôte (premier arrivé) valide les coups et diffuse l'état complet versionné (`keep: true`).
  Si l'hôte part, le suivant reprend la main ; un joueur absent ou inactif 60 s est joué par un bot.
- **Solo** (hors hub ou au choix) : contre 1 à 7 bots, partie sauvegardée dans le navigateur.

Options de salle : cumul des +2 (règle maison), contestation du +4, fin en 1 manche / 250 / 500 points, vitesse des bots.

Test local : `python3 -m http.server` puis ouvrir `http://localhost:8000/?solo`.
