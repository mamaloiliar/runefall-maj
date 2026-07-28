# Runefall — mises à jour de contenu

Dépôt public servant **uniquement** à distribuer les mises à jour du jeu
[Runefall](https://github.com/mamaloiliar/runefall) (dépôt de développement,
privé).

L'application installée sur le téléphone interroge `maj.json` à chaque
lancement. Si la version annoncée est plus récente que celle installée, elle
télécharge `runefall.pck` (quelques centaines de kilo-octets) et l'applique
au lancement suivant — sans réinstallation.

| Fichier | Rôle |
|---|---|
| `maj.json` | Manifeste : version, nom du correctif, taille, empreinte SHA-256 |
| `runefall.pck` | Le contenu du jeu : scènes, scripts, runes, sons |

Le moteur de jeu, lui, reste dans l'APK et ne change qu'en cas de mise à jour
de Godot ou de réglages de projet.
