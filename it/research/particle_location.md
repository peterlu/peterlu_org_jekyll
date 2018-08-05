---
layout: researchtopic
title:  "Posizione delle particelle rapida e accurata"
lang: it
id: particle_location
permalink: /research/particle_location

description: Software e metodi di imaging ad alte prestazioni per determinare rapidamente e con precisione le posizioni 3D di molte particelle colloidali nelle immagini del microscopio.

thumbnail: PLuTARC_Cluster_480_thumbn.jpg

youtube_single: mZm6I5j_bq0
youtube_playlist: 

publications:
- OpEx_07
- OpEx_13
- PhDThesis_08
- Confocal_05
---
Presentiamo una serie di metodi per localizzare, rapidamente e accuratamente, le particelle fluorescenti riprese con fluorescenza e microscopia confocale.

Abbiamo implementato la tradizionale metodologia Crocker e Grier per localizzare le particelle, con le librerie CPU e GPU accelerate. Di conseguenza, il rilevamento delle particelle è sufficientemente rapido e accurato per essere reimmesso nel controllo meccanico di uno stadio di microscopio, consentendo il blocco in tempo reale dei cluster colloidali, come mostrato nel video. Poiché possiamo seguire un cluster colloidale crescente mentre si allontana dal campo visivo fisso originale, possiamo estendere significativamente il tempo di osservazione di questi processi, oltre i limiti che la diffusione tipicamente impone. Siamo anche stati in grado di osservare i punti quantici (QD) trasportati attivamente in cellule vive libere di muoversi in tre dimensioni, per diverse ore.

Abbiamo anche esaminato attentamente tutte le fasi di questi algoritmi e dimostrato che localizzare accuratamente le particelle in 3D richiede kernel di convoluzione circolari, non i kernel quadrati scelti nelle precedenti implementazioni per motivi di prestazioni. Sebbene apparentemente un dettaglio banale, infatti, l'uso di kernel non circolari può portare alla rivelazione artefatta della cristallinità in sospensioni di particelle dense e disordinate che in realtà non hanno un ordine cristallino significativo.
