# ninogentile.archimedix.net

Archivio statico del sito personale di **Nino Gentile**, che fino a novembre 2026 era online su
ninogentile.com (WordPress su OVH, dominio registrato il 2024-11-14 e non rinnovato).

Il sito è stato regalato da Archimedix a Nino in occasione dell'uscita del suo libro
*"Appunti di un viaggio introspettivo"* (Edizioni Mille). Tutti i contenuti sono di Nino Gentile.

## Com'è fatto

- **Dump HTML** del sito pubblico, fatto il 2026-11-10 con `wget --mirror --convert-links`.
- **Pulizia**: tolti i residui dinamici di WordPress (feed, REST API, oEmbed, emoji loader,
  speculation rules) e riscritti i link assoluti verso `https://ninogentile.archimedix.net`.
- Commenti, ricerca e widget social (Facebook e Instagram feed) non funzionano più: il sito è statico.
- Pubblicato con **GitHub Pages**; il file `CNAME` contiene il dominio personalizzato
  (record DNS `ninogentile CNAME archimedix.github.io.` nella zona archimedix.net).

## Non versionato

`_archivio/` (in `.gitignore`) contiene l'export WordPress (WXR) e i 251 allegati originali non
usati dalle pagine pubblicate. Resta fuori dalla repo perché l'export contiene bozze non
pubblicate, email e IP degli utenti.
