# Mes compétences

Catalogue personnel de plugins Claude Code (chaque plugin reste dans le dépôt de son auteur).

## Installer sur un PC

```
/plugin marketplace add fabino66/mes-competences
```
```
/plugin install ponytail@mes-competences
```
Choisir la portée **User** pour l'avoir dans tous les projets du PC.

## Activer dans un projet (sessions cloud, téléphone)

Fichier `.claude/settings.json` du projet :

```json
{
  "extraKnownMarketplaces": {
    "mes-competences": {
      "source": { "source": "github", "repo": "fabino66/mes-competences" }
    }
  },
  "enabledPlugins": { "ponytail@mes-competences": true }
}
```

## Ajouter un plugin

Ajouter un bloc dans `plugins` de `.claude-plugin/marketplace.json` :

```json
{ "name": "nom-du-plugin", "source": { "source": "github", "repo": "auteur/depot" } }
```
