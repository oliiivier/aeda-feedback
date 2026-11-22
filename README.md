# Aeda — liseuse EPUB qui lit vos livres à voix haute

Aeda est une liseuse EPUB pour Android. Elle lit vos livres à voix haute avec des voix de synthèse naturelles et surligne le texte au fil de la lecture, phrase par phrase puis mot par mot. Toute la synthèse vocale est calculée **sur le téléphone** : aucun texte ne part vers un service en ligne.

Ce dépôt sert à recueillir vos **retours** : problèmes rencontrés, idées et suggestions. Le code de l'application n'y est pas publié.

## Ce que fait Aeda

- **Lecture à voix haute** de vos EPUB, en français, en anglais et en espagnol, avec un choix de voix par langue et un aperçu de chacune.
- **Surbrillance synchronisée** de la phrase et du mot lus, en mode page ou en défilement continu.
- **Livres audio** : Aeda lit les EPUB 3 avec narration synchronisée (Media Overlays) et peut associer un livre audio M4B à son EPUB pour suivre le texte pendant l'écoute.
- **Export** d'un livre narré au format EPUB 3 Media Overlays, lisible dans d'autres liseuses (Thorium, Apple Books…).
- **Bibliothèque** : connexion à votre serveur [Calibre-Web](https://github.com/janeczku/calibre-web), exploration par séries, auteurs et genres, même hors ligne ; découverte de classiques libres sur [Project Gutenberg](https://www.gutenberg.org/).

## Vie privée

- La synthèse vocale et l'analyse du texte tournent sur l'appareil.
- Aeda ne contacte que votre serveur Calibre-Web, Project Gutenberg et GitHub (téléchargement des modèles de voix, depuis les [releases](../../releases) de ce dépôt).
- Aucune donnée d'usage n'est collectée, aucune publicité.

## Contenus générés par IA

Les narrations sont produites par des voix de synthèse. L'application les signale par l'étiquette « IA », y compris dans les livres audio exportés.

## Donner votre avis

Ouvrez une [issue](../../issues/new) en précisant :

- pour un **problème** : la version d'Aeda (Réglages › À propos), le modèle du téléphone, ce que vous avez fait, ce qui s'est passé et ce que vous attendiez ; une capture d'écran aide souvent ;
- pour une **idée** : ce que vous aimeriez pouvoir faire et dans quelle situation.

Merci de ne joindre ni livre protégé par le droit d'auteur ni donnée personnelle.

## Licences et crédits

Aeda s'appuie sur des modèles, voix, données linguistiques et bibliothèques tiers (Pocket TTS de Kyutai, Qwen3-TTS, Lexique, Readium…). Leur liste complète, avec leurs licences, figure dans l'application : **Réglages › À propos**.

Les modèles que l'application télécharge sont hébergés dans les [releases](../../releases) de ce dépôt, sous leur licence d'origine, avec attribution et mention des modifications : voir [NOTICE.md](NOTICE.md) et [`licenses/`](licenses/).

- **Pocket TTS · Mimi** © Kyutai, export ONNX de stephvax — [CC BY 4.0](licenses/LICENSE-CC-BY-4.0.txt) ; fichiers inchangés.
- **wav2vec2 XLSR-53 espeak** © Meta AI, conversion ONNX de qnighy — [Apache 2.0](licenses/LICENSE-Apache-2.0.txt) ; quantifié en int8 pour Aeda.

---

## English

Aeda is an Android EPUB reader that reads your books aloud with natural synthetic voices, computed entirely on the device, and highlights each sentence and word as it is read. It supports French, English and Spanish, EPUB 3 Media Overlays, M4B audiobooks and Calibre-Web libraries. No usage data is collected.

This repository collects feedback only: please [open an issue](../../issues/new) to report a problem (include the app version from Settings › About and your phone model) or suggest an idea.

---

© 2026 Aeda · [caere.fr](https://caere.fr)
