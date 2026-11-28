---
title: Feedpoint
summary: Sjáðu hvernig samviðnám í fæðipunkti endafæddra vírloftneta og tvípóla breytist með lengd vírsins og staðsetningu fæðipunktsins, á HF-tíðnisviðunum frá 160 m upp í 6 m.
# Stutt lýsing fyrir forsíðuna. Ein eða tvær stuttar setningar.
tagline: Samviðnám vírloftneta á HF, 160 m til 6 m. Endafædd loftnet og tvípólar.
# Dagurinn sem forritið fór á síðuna. Forsíðan sýnir fjögur nýjustu forritin.
date: 2026-11-13
app_url: https://tf5nn.github.io/HF-Antenna-Impedance-Visualizer/
repo_url: https://github.com/TF5NN/HF-Antenna-Impedance-Visualizer
translated_from: en
translated_by: ai
# Tags work the same as on posts. Write them in English in both languages.
tags: ["HAM radio", "Antennas"]
weight: 10
---

Feedpoint sýnir samviðnám HF-loftneta: gagnvirkt kennslutól í vafranum fyrir radíóamatöra. Það teiknar samviðnámið sem vírloftnet hefur í fæðipunktinum, svo þú sjáir hvers vegna sumar vírlengdir er auðvelt að aðlaga á mörgum tíðnisviðum og aðrar ekki.

Forritið sjálft er á ensku, svo heiti hnappanna eru hér á ensku líka.

## Hvað það gerir

- **Ellefu HF-tíðnisvið**, frá 160 m upp í 6 m, og hægt að kveikja og slökkva á hverju fyrir sig.
- **Tveir hamir.** End-Fed sýnir samviðnám á móti lengd vírsins. Dipole sýnir samviðnám á móti staðsetningu fæðipunktsins, frá miðjufæddum tvípól yfir í utanmiðjufæddan (OCF).
- **Aðlögunarsvæði** skyggð á grafinu: 49:1, 9:1 með loftnetsaðlagara og 1:1 fyrir endafædd loftnet; 1:1, 4:1, 6:1 og eigið hlutfall fyrir tvípóla.
- **Sweet Spots** dregur fram vírlengdir þar sem mörg tíðnisvið lenda innan aðlögunarsvæðis í einu.
- **Loftnetsaðlagari** (tuner): athugun með þremur forstillingum og eigin sviði.
- Stillingar fyrir **mótvægi** (counterpoise) og **hraðastuðul** (velocity factor), og hæð yfir jörðu í Dipole-ham.

## Hvað það nær ekki yfir

Tólið reiknar löng vírloftnet, þar sem standbylgjur ráða samviðnáminu. Það gildir ekki fyrir rafmagnslega stutt loftnet eða stangarloftnet með hleðsluspólum. [README-skráin á GitHub](https://github.com/TF5NN/HF-Antenna-Impedance-Visualizer#readme) útskýrir hvers vegna (á ensku).

## Leyfi

Creative Commons Attribution 4.0 (CC BY 4.0).
