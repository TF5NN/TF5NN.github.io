---
title: Sightline
summary: Hæðarsnið fyrir radíósambönd. Settu tvo punkta á kortið og sjáðu hvort landið er fyrir, og hvort radíósamband á milli þeirra myndi líklega ganga.
# Stutt lýsing fyrir forsíðuna. Ein eða tvær stuttar setningar.
tagline: Hæðarsnið. Settu tvo punkta og sjáðu hvort radíósamband á milli þeirra gengur.
# Dagurinn sem forritið fór á síðuna. Forsíðan sýnir fjögur nýjustu forritin.
date: 2026-11-16
app_url: https://tf5nn.github.io/sightline/
app_lang: true
repo_url: https://github.com/TF5NN/sightline
translated_from: en
translated_by: ai
# Tags work the same as on posts. Write them in English in both languages.
tags: ["HAM radio", "LoRa", "Maps"]
weight: 30
---

Sightline teiknar landið eftir beinni línu milli tveggja punkta, og sjónlínuna milli loftnetanna tveggja. Það les 2 m hæðargögn beint úr opna ArcticDEM-safninu, svo það virkar á Íslandi og öðru landi norðan við um 60°N.

## Hvað það gerir

- **Hæðarsnið** milli hvaða tveggja punkta sem er, með sveigju jarðar meðtalinni og land sem er fyrir merkt rautt, bæði á grafinu og á kortinu.
- **Loftnetshæð** á báðum endum, hvort sem það er mastur, þak eða handstöð.
- **Mat á radíósambandi**: veldu tíðnisvið, tæki og loftnet og fáðu móttekið merki, svigrúm og skýra niðurstöðu.
- **Forstillingar** fyrir FM á 2 m og 70 cm og fyrir LoRa-mesh á 868 MHz (MeshCore og Meshtastic), og þínar eigin tölur undir Ítarlegt.
- **Fresnel-svæðið** á sniðinu, og kaflar þar sem landið er of nærri merktir gulir.
- **Stöðvalög**: sýndu fastar stöðvar á kortinu, til að byrja með endurvarpa ÍRA. Smelltu á stöð til að sjá hvernig á að nota hana, eða notaðu hana sem punkt A eða B með afli, loftneti og hæð þegar útfylltum.
- **Stöðvar frá A**: þegar stöðvalag sést og punktur A er settur er hver stöð lituð eftir fyrsta mati á sambandinu: grænt ætti að virka, gult er tæpt, rautt ólíklegt. Aðeins á Íslandi.
- **Útsýni**: sjóndeildarhringurinn séður frá punkti A, með áttum, og stöðvarnar og punktur B merkt þar sem þau standa. Dragðu til að snúa. Aðeins á Íslandi.
- **Virkar í síma**: renndu fingri eftir sniðinu til að lesa hæðirnar.
- **Ljóst eða dökkt**, eftir stillingu tækisins, með hnappi til að skipta. Valið fylgir yfir í hin forritin.
- **Deildu leið**: vefslóðin geymir alla uppsetninguna.

## Gott að vita

Niðurstaðan er mat út frá einföldu líkani. Hún hefur reynst rétt um það hvenær land lokar leið, en verið of bjartsýn á lokaðar leiðir inni í bæ. Taktu svigrúmið sem ±10 dB. [Hvernig það virkar og hve vel má treysta því](https://tf5nn.github.io/sightline/how.html?lang=is) segir nánar frá.

Landgögnin eru yfirborðslíkan: byggingar og tré teljast með landinu, eins og þau stóðu þegar gervitunglamyndirnar voru teknar.

Punktarnir þínir haldast í vafranum þínum og í vefslóðinni.

## Heimildir

Landgögn: ArcticDEM, Polar Geospatial Center (CC BY 4.0). Kort: þátttakendur í OpenStreetMap.
