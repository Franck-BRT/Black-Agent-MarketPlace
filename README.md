# Black Agent MarketPlace

Dépôt officiel des modules pour **Black Agent** — l'assistant IA local de Black Room Technologies.

## Modules disponibles

| Module | Version | Catégorie | Description |
|--------|---------|-----------|-------------|
| [Persona Library](modules/persona-library/) | 1.0.0 | Tool | Bibliothèque de personas IA (13 built-in + custom) |

## Installation

### Depuis l'application
1. Ouvrir **Black Agent**
2. Aller dans **Marketplace**
3. Cliquer sur **Installer** sur le module souhaité

### Installation manuelle
1. Télécharger le fichier `.bam` du module
2. Dans Black Agent : **Paramètres > Modules > Importer .bam**
3. Accepter les permissions demandées
4. Activer le module

## Structure

```
catalog.json              # Index des modules (lu par l'app)
modules/
  persona-library/
    persona-library-1.0.0.bam   # Module packagé (.bam = ZIP)
    icon.svg                     # Icône du module
```

## Format .bam

Un fichier `.bam` (Black Agent Module) est une archive ZIP contenant :
- `manifest.json` — métadonnées et permissions
- `backend/module.wasm` — binaire WASM (extism)
- `assets/` — icônes et ressources

## Licence

MIT — Black Room Technologies
