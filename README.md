# Théon · Rapports

Site statique des **rapports du matin** et **bilans du soir** du second cerveau Théon.

## Fonctionnement

- Profil Hermes `assistant` → cron `rapport-matin` (7h) et `bilan-soir` (21h).
- Chaque rapport est écrit dans `_posts/YYYY-MM-DD-{matin|soir}.md` (Markdown + frontmatter Jekyll), puis commit + push.
- GitHub Pages (Jekyll) reconstruit et publie le site automatiquement.

## Structure

```
_config.yml          Configuration Jekyll
index.md             Page d'accueil (liste des rapports)
_layouts/            Gabarits HTML
_posts/              Les rapports, un fichier par jour/type
```
