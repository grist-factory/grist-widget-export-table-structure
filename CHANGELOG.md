# Changelog

Le format suit [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/) ; les versions suivent [SemVer](https://semver.org/lang/fr/).
*The format follows Keep a Changelog; versions follow SemVer.*

## 1.0.0-beta.1 — 2026-10-05

Première version publique (Beta). *First public release (Beta).*

### Ajouté / Added

- **Import** : analyse du code Python d'une table (Code View de Grist ou export du widget), aperçu colonne par colonne, création de tables ou ajout des colonnes manquantes à une table existante, avec choix des éléments repris (libellés, descriptions, listes de choix, formats, colonne affichée des références, liens bidirectionnels, formules).
  *Import: analysis of a table's Python code, column-by-column preview, creation of tables or addition of the missing columns to an existing table, with a choice of the elements to copy.*
- **Export** : choix des tables et des colonnes, mêmes éléments, génération du code au format de la Code View, bandeau des tables référencées.
  *Export: choice of tables and columns, same elements, code generated in the Code View format, banner of the referenced tables.*
- **Confirmation avant toute écriture**, avertissement quand des formules vont s'exécuter (et quand l'une appelle `REQUEST`), annulation par le bouton Annuler de Grist.
  *Confirmation before any write, warning when formulas are about to run, undo through Grist's Undo button.*
- Interface en français et en anglais, thèmes système, clair et sombre, identité Grist Factory, accessibilité (cibles de 24 px, contrastes 4,5:1, focus piégé dans les boîtes de dialogue).
  *French and English interface, system / light / dark themes, Grist Factory identity, accessibility.*
- Publication GitHub Pages avec l'API officielle de Grist servie avec la page (aucun domaine tiers).
  *GitHub Pages publication with Grist's official API served with the page (no third-party domain).*

### Sécurité / Security

- Le texte collé n'est jamais exécuté ; aucune écriture avant confirmation ; ajouts seulement ; formules décochées par défaut ; politique de sécurité (CSP) stricte, sans appel réseau. Voir [SECURITY.md](SECURITY.md).
  *The pasted text is never executed; no write before confirmation; additions only; formulas unticked by default; strict CSP with no network call.*
