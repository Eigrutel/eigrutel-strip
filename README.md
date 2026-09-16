# strip

**Version 1.0.0 · 16-09-2026 · Français / English**

Programme conçu et développé par **Simon Léturgie**, dans le cadre d’**Eigrutel BD Academy**.  
Program designed and developed by **Simon Léturgie** as part of **Eigrutel BD Academy**.

[Ouvrir / Open](https://eigrutel.github.io/eigrutel-strip/strip.html) · [Accueil / Home](https://eigrutel.github.io/eigrutel-strip/) · [Logithèque](https://www.stripmee.com/logitheque/) · [Soutenir / Support](https://fr.tipeee.com/leturgie/)

Les liens GitHub Pages ci-dessus fonctionneront après publication du dépôt `Eigrutel/eigrutel-strip`.  
The GitHub Pages links above will work once `Eigrutel/eigrutel-strip` is published.

## Français

### Présentation

strip prépare les gabarits, découpe les dessins et compose les sorties d’un strip de bande dessinée. Il permet de passer d’une disposition horizontale à une grille 2 × 2 ou à une lecture verticale Yonkoma, puis de préparer des images pour les réseaux ou l’impression.

### Les cinq espaces

1. **Gabarit** : disposition, hauteur des cases, échelle du format de travail, contour extérieur, fond perdu, diagonales, tiers, portées de lettrage, graduations et couleurs de lignes. Presets nommés. Export SVG, PNG 300 dpi et impression/PDF par le navigateur.
2. **2a. Strip / 2 × 2** : import d’un dessin complet, réglage des guides de découpe, choix du découpage, du débord et de la marge. Conversion entre les dispositions proposées. Les variantes avec cases doubles limitent les sorties compatibles, notamment Yonkoma.
3. **2b. Strip libre** : cadrage d’un strip, ajout de séparations verticales, mémorisation de plusieurs strips et production d’images individuelles. En mode multi-strips, aucun strip complet n’est produit.
4. **2c. Images séparées** : import groupé ou individuel, zoom, déplacement, réorganisation, cases doubles, cadre et inter-iconiques. Les cases sans image sont produites en blanc.
5. **Exports** : sélection des images, du strip, du 2 × 2 et du Yonkoma disponibles ; nom personnalisé ; profil Réseaux ou Print 300 dpi ; PNG ou ZIP pour une sélection multiple.

### Démarrage

Ouvrir `strip.html` dans un navigateur récent. Aucune installation, compilation ou connexion à un compte n’est nécessaire. Le bouton **FR / EN**, en bas à droite, change la langue. Le français est utilisé par défaut.

Pour un usage local, conserver le dossier `favicon/` à côté du HTML si l’on souhaite afficher l’icône. JSZip est intégré au HTML : les exports ZIP fonctionnent aussi hors connexion.

### Formats de sortie

| Profil Réseaux | Dimensions |
| --- | --- |
| Images individuelles et 2 × 2 | 1080 × 1350 px |
| Strip horizontal | 1080 × 566 px |
| Yonkoma | 1080 × 1920 px |

Le dessin est ajusté sur fond blanc sans recadrage. Le profil Print utilise les dimensions du gabarit et inscrit une résolution de 300 dpi dans les PNG. Augmenter les dimensions ne crée pas de détail absent du dessin source.

Le bouton **×** près de **Produire** vide et réinitialise uniquement l’espace 2a, 2b ou 2c concerné. En 2b, il efface également les strips mémorisés. Les sorties de cet espace sont retirées des exports ; les autres espaces et les presets de gabarit sont conservés.

### Données et sauvegardes

Les images sont traitées dans le navigateur, sans envoi à un serveur. Les presets de gabarit et la langue sont conservés dans le stockage local lorsque le navigateur l’autorise. La clé des anciens presets est conservée pour la compatibilité.

**Les images importées, les strips mémorisés et les sorties calculées restent uniquement en mémoire pendant la session.** Recharger ou fermer la page les efface. Exporter les résultats avant de quitter. Changer de navigateur ou d’adresse d’hébergement ne transfère pas les presets.

### Compatibilité

Interface adaptée aux ordinateurs, tablettes et téléphones ; souris et interactions tactiles. Navigateurs modernes visés : Safari, Chrome, Edge et Firefox. Les téléchargements et l’impression/PDF suivent le fonctionnement du navigateur.

## English

### Overview

strip creates templates, cuts artwork into panels and assembles comic strip outputs. It supports horizontal strips, 2 × 2 grids and vertical Yonkoma layouts, with output profiles for social media and print.

### Five workspaces

1. **Template**: layout, panel height, working scale, outer border, bleed, diagonals, thirds, lettering guides, rulers and line colours. Named presets. SVG, 300 dpi PNG and browser printing/PDF.
2. **2a. Strip / 2 × 2**: import complete artwork, adjust cutting guides, choose panel layout, overflow and margins. Convert between supported layouts. Double-panel variants restrict compatible outputs, including Yonkoma.
3. **2b. Free strip**: frame a strip, add vertical separators, store several strips and produce individual images. Multiple stored strips do not generate a single complete strip.
4. **2c. Separate images**: batch or individual import, zoom, positioning, reordering, double panels, frames and gutters. Missing images become blank panels.
5. **Exports**: select available individual images, strip, 2 × 2 and Yonkoma; set an output name; choose Social or Print 300 dpi; download PNG or ZIP for multiple files.

### Getting started

Open `strip.html` in a recent browser. No installation, build step or account is required. The **FR / EN** button at the bottom right switches languages. French is the default.

Keep the `favicon/` folder beside the HTML to display the icon locally. JSZip is embedded in the HTML, so ZIP exports work offline.

### Output sizes

| Social profile | Dimensions |
| --- | --- |
| Individual images and 2 × 2 | 1080 × 1350 px |
| Horizontal strip | 1080 × 566 px |
| Yonkoma | 1080 × 1920 px |

Artwork is fitted on a white background without cropping. Print uses the template dimensions and records 300 dpi resolution in the PNG files. Enlarging an image does not add missing source detail.

The **×** button beside **Produce** clears and resets only its own workspace (2a, 2b or 2c). In 2b, it also clears stored strips. That workspace’s outputs are removed from exports; other workspaces and template presets are preserved.

### Data and saving

Images are processed in the browser without server uploads. Template presets and the selected language are saved locally when browser storage is available. The old preset key is preserved for compatibility.

**Imported images, stored strips and generated outputs remain in session memory only.** Reloading or closing the page clears them. Export results before leaving. Presets do not transfer automatically between browsers or hosting addresses.

### Compatibility

The interface adapts to desktop, tablet and phone screens and supports mouse and touch interaction. Intended browsers: modern Safari, Chrome, Edge and Firefox. Downloads and printing/PDF depend on the browser.

## Fichiers / Files

| Fichier / File | Rôle / Purpose |
| --- | --- |
| `strip.html` | Application autonome FR/EN / Standalone FR/EN application |
| `index.html` | Page de présentation bilingue / Bilingual landing page |
| `favicon/favstrip.png` | Icône à ajouter / Icon to supply |
| `README.md` | Utilisation / Usage |
| `ARCHITECTURE.md` | Organisation du code / Code structure |
| `CHANGELOG.md` | Historique / Change log |
| `LICENSE.md`, `NOTICE.md` | Licences et attribution / Licensing and attribution |
| `PUBLICATION.md` | Dépôt, commit, release et Pages / Repository, commit, release and Pages |

## Licences / Licenses

Code : **GNU AGPL v3.0 ou version ultérieure / or later**.  
Documentation et modèles / Documentation and templates : **CC BY-SA 4.0**, sauf mention contraire / unless otherwise stated.  
Marques, logos et signes distinctifs Eigrutel réservés / Eigrutel trademarks, logos and distinctive signs reserved.

Les dessins importés restent soumis aux droits de leurs auteurs. / Imported artwork remains subject to its authors’ rights.
