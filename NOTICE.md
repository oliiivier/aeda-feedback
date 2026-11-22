# Avis et attributions — modèles distribués par ce dépôt

Les modèles téléchargés par l'application Aeda sont hébergés dans les
[releases](../../releases) de ce dépôt. Le dépôt ne contient pas le code d'Aeda ;
chaque release joint ses propres `LICENSE-*.txt` et `NOTICE.md`, repris ici.

Les textes complets des licences sont dans [`licenses/`](licenses/).

## Pocket TTS (release `pocket-v1`) — CC BY 4.0

Licence : Creative Commons Attribution 4.0 International
([texte](licenses/LICENSE-CC-BY-4.0.txt), <https://creativecommons.org/licenses/by/4.0/>).

Travaux d'origine :

- Pocket TTS et codec audio Mimi, © Kyutai — <https://huggingface.co/kyutai/pocket-tts> (CC BY 4.0)
- Export ONNX et quantification int8 : stephvax — <https://huggingface.co/stephvax/pocket-tts-onnx>
  (révision `9dd58b75ba672bb75df1c62a493f6db7c80de6d1`, CC BY 4.0)

Modifications : conversion des modèles au format ONNX et quantification int8 de
`flow_lm_main` par stephvax. Aeda ne modifie pas ces fichiers : ils sont recopiés à
l'identique (mêmes SHA-256), renommés `<langue>-<fichier>.onnx` (`en`, `fr`, `es`).

Aucune garantie. Kyutai et stephvax ne cautionnent ni Aeda ni cette redistribution.

## wav2vec2 XLSR-53 espeak (release `phonrec-v1`) — Apache 2.0

Licence : Apache License 2.0 ([texte](licenses/LICENSE-Apache-2.0.txt)).

Travaux d'origine :

- facebook/wav2vec2-large-xlsr-53 — Meta Platforms / Facebook AI (Apache-2.0)
- facebook/wav2vec2-xlsr-53-espeak-cv-ft — Meta Platforms / Facebook AI (Apache-2.0)
- qnighy/wav2vec2-xlsr-53-espeak-cv-ft-ONNX — conversion ONNX et `vocab.json` (Apache-2.0)

Modifications : `model_int8_keep_conv.onnx` est la conversion ONNX de qnighy quantifiée
dynamiquement en int8 (ONNX Runtime, QInt8) pour Aeda, en conservant les convolutions en
fp32. `vocab.json` est inchangé.
