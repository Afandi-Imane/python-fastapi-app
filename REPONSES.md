# TP 6 — Réponses

**Q1 :** GITHUB_ENV rend les variables disponibles uniquement
dans les steps suivantes, pas dans celle qui les définit.

**Q2 :** APP_NAME est vide dans verify-env, car GITHUB_ENV
a une portée limitée au job dans lequel il est utilisé.