# Architecture — strip 1.0.0

## Français

`strip.html` regroupe le HTML, les styles, les traitements et le dictionnaire anglais. Il ne nécessite ni serveur applicatif ni compilation. `index.html` présente l’outil et renvoie vers l’application et la documentation, sur le modèle du dépôt Scénoscope.

### Organisation

- CSS : composants, navigation, panneaux, outils flottants et adaptations tactiles. Le titre est centré dans la barre indépendamment des cinq onglets.
- JSZip embarqué : dépendance tierce minifiée, conservée avec ses mentions de licence.
- Navigation : `showTab` active les cinq espaces.
- Gabarit : géométrie en millimètres, SVG, format de travail proportionnel, guides et presets.
- Import complet : canvas, guides tactiles, découpage et compositions.
- Strip libre : séparateurs verticaux et collection de strips en mémoire.
- Images séparées : import, recadrage, déplacement, cases doubles et assemblage.
- Exports : `lastExportSet`, mise au format, résolution PNG et ZIP.
- Traduction : `STRIP_I18N_EN`, messages dynamiques et observation des textes/attributs. Les sources françaises sont conservées dans des WeakMap pour revenir exactement au texte initial. Les noms de presets ne sont pas traduits.

### Persistance

`switch_template_presets_v1` conserve volontairement le nom historique afin de retrouver les presets existants. `strip_lang` conserve la langue. Les dessins et résultats ne sont pas enregistrés dans localStorage. Il n’y a pas de sauvegarde de projet dans cette version.

### Maintenance

Ajouter chaque nouveau libellé au dictionnaire, et chaque message paramétré aux règles de traduction. Ne pas traduire les valeurs techniques, les noms de fichiers ou les textes personnels. Conserver les identifiants DOM utilisés par les modules. Les calculs de découpage n’ont pas été réécrits pour cette stabilisation.

## English

`strip.html` contains the markup, styles, processing code and English dictionary. No application server or build step is needed. `index.html` presents the tool and links to the application and documentation, following the Scénoscope repository structure.

### Structure

- CSS: components, navigation, panels, floating tools and touch layouts. The title is centred within the navigation bar independently of its five tabs.
- Embedded JSZip: minified third-party dependency with its license notices preserved.
- Navigation: `showTab` activates the five workspaces.
- Template: millimetre-based geometry, SVG, proportional working size, guides and presets.
- Complete artwork import: canvas, touch guides, panel cutting and compositions.
- Free strip: vertical separators and an in-memory strip collection.
- Separate images: import, cropping, positioning, double panels and assembly.
- Exports: `lastExportSet`, output sizing, PNG resolution metadata and ZIP.
- Translation: `STRIP_I18N_EN`, dynamic messages and text/attribute observation. French sources are retained in WeakMaps for exact restoration. Personal preset names are excluded.

### Persistence

`switch_template_presets_v1` deliberately retains its historical name to preserve existing presets. `strip_lang` stores the language. Artwork and results are not saved in localStorage. This version has no project-save feature.

### Maintenance

Add new labels to the dictionary and parameterised messages to the translation rules. Do not translate technical values, filenames or personal text. Preserve DOM identifiers used by the modules. Panel-cutting calculations were not rewritten during this stabilisation.
