# Changelog

Tutte le modifiche rilevanti a questo modulo sono documentate in questo file.

Il formato è basato su [Keep a Changelog](https://keepachangelog.com/it/1.1.0/)
e questo progetto aderisce al [Semantic Versioning](https://semver.org/lang/it/).

## 1.0.1

- Sicurezza: il "Link ADV" accetta solo `http`, `https`, `mailto`, `tel` e `//`; altri schemi (`javascript:`, `data:`) ripiegano sull'URL del prodotto.

## [1.0.0] - 2026-10-14

### Added
- Tipo prodotto `adv_product` (Adv Product) con indice prezzi, stock e prezzo a 0.
- Attributi `link_adv` (Link ADV) e `adv_cta_label` (testo pulsante) nel gruppo "Adv" di tutti gli attribute set, tramite data patch.
- Link del prodotto verso la destinazione, redirect 302 della scheda, prezzo nascosto, carrello rifiutato, esclusione dalla sitemap.
- View model `Threecommerce\AdvProduct\ViewModel\AdvProduct` per i temi custom.
- Traduzione italiana.

### Removed
- Vecchio `InstallData`, CSS di layout a righe non usato e configurazione di prezzo non funzionante della bozza iniziale.
