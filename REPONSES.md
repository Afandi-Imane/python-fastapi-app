# TP 6 — Réponses

**Q1 :** GITHUB_ENV rend les variables disponibles uniquement
dans les steps suivantes, pas dans celle qui les définit.

**Q2 :** APP_NAME est vide dans verify-env, car GITHUB_ENV
a une portée limitée au job dans lequel il est utilisé.

**Q3 :** Le symbole > écrase le contenu précédent,
tandis que >> ajoute une nouvelle ligne.

**Q4 :** GITHUB_ENV fonctionne uniquement dans un job.
GITHUB_OUTPUT permet de transmettre des valeurs entre
jobs grâce à outputs et needs.

**Q5 :** Sans needs: build, deploy peut s'exécuter
avant build et ne peut pas récupérer correctement
son output.

**Q6 :** checkout doit s'exécuter avant l'action locale
pour récupérer ses fichiers depuis le dépôt.

**Q7 :** shell: bash est obligatoire pour préciser
l'interpréteur utilisé par les commandes run
dans une action composite.