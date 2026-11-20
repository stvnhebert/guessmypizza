# Guess my pizza

- Politique de confidentialité : https://stvnhebert.github.io/guessmypizza/
- `config.json` : contenu piloté à distance (lu par le jeu au lancement).

## Lancer une opération partenaire (sans mise à jour App Store)

1. Ouvrir `config-exemple.json`, copier le bloc `campaign` dans `config.json` et l'adapter.
2. `pizzaID` : clé d'une recette du jeu (margherita, marinara, pepperoni, reine, capricciosa, napolitaine, hawaienne, quatreFromages, vegetarienne, calzone, parma, thon, supreme, carbonara, saumon, chevreMiel, savoyarde, barbecue).
3. `start` / `end` : dates ISO (UTC). Hors de ces dates, rien ne s'affiche.
4. Textes : une entrée par langue (fr, en, it, es, pt, zh, ko, ja, ru) ; l'anglais sert de secours.
5. `promoCode` : affiché après chaque victoire, avec un bouton Copier.
6. `interstitialEvery` : une pub plein écran toutes les N parties.
7. Pour arrêter : remettre `"campaign": null`.

Le jeu affiche toujours la mention « PARTENAIRE ». Les changements arrivent chez les joueurs à leur prochaine ouverture du jeu (quelques minutes après la publication sur GitHub).
