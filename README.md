# plico-models

Modelli di traduzione automatica usati da **Plico** (lettore ed editor di PDF che lavora sul dispositivo) per le lingue
che il progetto Bergamot non pubblica: **polacco** e **olandese**, da e verso l'inglese.

L'app li scarica una volta (con verifica SHA-256) e li tiene in cache: la traduzione avviene poi nel dispositivo, il testo
dei documenti non viene inviato a nessun servizio.

## Origine

File copiati senza modifiche dai modelli di **Firefox Translations** di Mozilla (Remote Settings, raccolta
`translations-models`; repository originale https://github.com/mozilla/firefox-translations-models, ora
https://github.com/mozilla/translations). Motore compatibile: [bergamot-translator](https://github.com/browsermt/bergamot-translator).

| Direzione | File | Versione | Dimensione | SHA-256 |
|---|---|---|---|---|
| en → pl | `enpl/vocab.enpl.spm` | 2.1 | 0.8 MB | `2000f182efa8ce5f…` |
| en → pl | `enpl/model.enpl.intgemm.alphas.bin` | 2.1 | 31.6 MB | `b0b59716bcc8f46b…` |
| en → pl | `enpl/lex.50.50.enpl.s2t.bin` | 2.1 | 3.5 MB | `d7d7b364673f6337…` |
| pl → en | `plen/lex.50.50.plen.s2t.bin` | 2.0 | 5.0 MB | `b295dfefa7022a62…` |
| pl → en | `plen/model.plen.intgemm.alphas.bin` | 2.0 | 31.6 MB | `06dbab3baa3bbcea…` |
| pl → en | `plen/vocab.plen.spm` | 2.0 | 0.8 MB | `2000f182efa8ce5f…` |
| en → nl | `ennl/model.ennl.intgemm.alphas.bin` | 2.1 | 31.6 MB | `7e8402da61972dc2…` |
| en → nl | `ennl/vocab.ennl.spm` | 2.1 | 0.8 MB | `c09588ca5662b230…` |
| en → nl | `ennl/lex.50.50.ennl.s2t.bin` | 2.1 | 4.0 MB | `bb4922718f8ca6d7…` |
| nl → en | `nlen/vocab.nlen.spm` | 2.0 | 0.8 MB | `c09588ca5662b230…` |
| nl → en | `nlen/model.nlen.intgemm.alphas.bin` | 2.0 | 31.6 MB | `ff987741ff15a5d9…` |
| nl → en | `nlen/lex.50.50.nlen.s2t.bin` | 2.0 | 4.9 MB | `811ac8f9dcbd1270…` |

## Licenza

Mozilla Public License 2.0, come il repository di origine (vedi `LICENSE`). Questi file sono distribuiti così come
sono, senza garanzie. Mozilla e Firefox sono marchi di Mozilla Foundation: questo repository non è affiliato a Mozilla.
