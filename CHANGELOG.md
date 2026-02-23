# Changelog

All notable changes to this project will be documented in this file.

## [0.1.0] - 2026-02-20
### Added
- Initial HACS dashboard card: `barocast-ha-card`.
- Defensive rendering for startup/unavailable sensor states.
- Gradient-based polished visual layout for forecast summary.
- Compatibility with `sensor.barocast_forecast` and detail sensors.
- Default card entity IDs use the `sensor.barocast_forecast*` namespace.
- README examples aligned with the Barocast sensor namespace.
- Bilingual documentation (EN/FR).

### Fixed
- Corrected language label mapping by integration language index.
- Added bounds handling for forecast detail code mapping path.

---

# Journal des changements

Toutes les modifications notables de ce projet sont documentées dans ce fichier.

## [0.1.0] - 2026-02-20
### Ajouts
- Première carte dashboard HACS : `barocast-ha-card`.
- Rendu robuste face aux états indisponibles au démarrage.
- Mise en page visuelle améliorée (dégradés + synthèse prévision).
- Compatibilité avec `sensor.barocast_forecast` et capteurs de détail.
- Les IDs d’entités par défaut utilisent l’espace `sensor.barocast_forecast*`.
- Les exemples README sont alignés avec le nouvel espace de noms capteurs.
- Documentation bilingue (EN/FR).

### Corrections
- Correction du mapping des libellés de langue selon l’index de l’intégration.
- Ajout d’une gestion des bornes sur le chemin de mapping du code détail.
