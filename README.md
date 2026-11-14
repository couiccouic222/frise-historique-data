# frise-historique-data

Dépôt **public** contenant la source de vérité des données de la frise historique : `events.json` à la racine.

- L'app (locale ou hébergée sur Mistral Studio) charge ce fichier en raw : `https://raw.githubusercontent.com/couiccouic222/frise-historique-data/main/events.json`
- Un simple push de `events.json` ici met la frise à jour au prochain rafraîchissement (F5) — **aucun redéploiement** de l'app.
- Le dépôt de l'app (`frise_historique_app`, privé) garde une copie embarquée (`apps/web/events.json` + `apps/web/events-data.js`) utilisée comme repli en `file://` / hors ligne.
