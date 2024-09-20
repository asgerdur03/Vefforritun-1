# Vefforritun 1, 2024: Verkefni 5, CSS #3

## Markmið

- Útfæra skalanlegann vef.
- Nota grid til að stýra útliti.
- Útfæra kvikun.

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2024-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2024-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2024-v4) setur upp útlit (e. layout).
- [Verkefni 5](https://github.com/vefforritun/vef1-2024-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2024-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Verkefnið

Verkefnið er framhald af [verkefni 2](https://github.com/vefforritun/vef1-2024-v2), [verkefni 3](https://github.com/vefforritun/vef1-2024-v3) og [verkefni 4](https://github.com/vefforritun/vef1-2024-v4), nýtir það efni sem uppsett er í þeim og fylgir þeim verkefnalýsingum fyrir utan það sem tekið er fram hér. Leyfilegt er að nota [sýnilausn að verkefni 4](https://github.com/vefforritun/vef1-2024-v4-synilausn), sem gefin verður út föstudaginn 20. september.

Nú hafa eigendur Spilabúðarinnar skoðað uppfært útlit og það hefur steingleymst að gera þetta skalanlegt! Það þarf að uppfæra verkefnið þannig að síðan passi og virki vel í öllum stærðum frá og með `320px`.

Einnig hefur komið í ljós að það er ekki jafnvægi í hönnun, til að bæta úr því er búið að aðlaga allt að grind sem er skilgreind í `grid.css` og sjá má hvernig lítur út í uppfærðum fyrirmyndum í `fyrirmynd/`.

Að lokum skal bæta við kvikun (e. animation) sem gerir síðuna líflegri.

Sjá uppfært skjal með grunnstílum og breytum í `styles.css`.

Allt útlitið skal vera í `./styles.css` og **allar** HTML skrár skulu vísa í nákvæmlega þá skrá.

## Útlit

Fyrirmynd að útliti er í `fyrirmynd/` möppu. Öll skjáskot eru tekin í `1500px`, `750px` og `320px` breiðum Firefox vafra. Athugið að fyrirmyndir eru uppfærðar frá verkefni 3 og 4.

Bæta þarf við auka elementum við lausn/sýnilausn til að geta náð fram útliti.

Þar sem allt útlit skal útfæra í einni CSS skrá, skal huga að cascade og erfðum, þó er fullkomlega eðlilegt að endurtaka eigindi, en t.d. fyrir málsgreinar (`<p>`) þarf aðeins að taka fram einu sinni hvert margin þeirra er.

### Almennt

Gefið er `styles.css` skjal með grunn að lausn og athugasemdum.

Gefið er `grid.css` skjal með „grid overlay“ sem er vísað í í HTML skrám og sést á fyrirmyndum.

Allt sem gildir í verkefni 2, verkefni 3 og verkefni 4 gildir áfram í þessu verkefni.

Nota skal skilgreind CSS custom properties sem gefin eru í `styles.css`, búið er að bæta við skilgreiningum frá verkefni 4.

### Skalanleiki

Gera þarf síðuna skalanlega og hugsa um að hún virki vel í öllum stærðum frá og með `320px`. Í sýnilausn og fyrirmynd eru brotpunktar:

- Frá og með `320px`
- Frá og með `500px`
- Frá og með `700px`
- Frá og með `800px`

### Grind

Útfæra skal grind skv. CSS custom properties og fyrirmyndum.

### Kvikun

Setja skal upp kvikun:

- Þegar síða opnast skal fara úr `opacity: 0` í `opacity: 1`.
- Þegar sveimað er yfir takka skal snúa við litum.

Nota skal CSS custom properties sem eiga við kvikun og hafa forskeytið `--transition-`.

Sjá hvernig kvikun hegðar sér í myndbandi í `./fyrirmynd/v5.mp4`.

### Takmarkanir

Leyfilegt er að nota allt CSS.

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo.

## Mat

- 20% – Snyrtilega uppsett og gilt CSS.
- 30% – Skalanleg lausn sett upp skv. forskrift.
- 30% – Grind sett upp skv. forskrift.
- 20% – Kvikun útfærð skv. forskrift.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 16. september 2024.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 26. september 2024.

Skilaboð skulu innihalda:

- zip skrá með öllum skrám _eða_ hlekkur á almennt (e. public) GitHub.
- slóð á verkefni keyrandi á Netlify sem athugasemd („Add comment“ eða „Bæta við athugasemd“ á skilaskjá í Canvas).

Skila má eins oft og þið viljið þar til skilafrestur rennur út.

## Einkunn

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ef stórt mállíkan (LLM, „gervigreind“, t.d. ChatGTP) er notað til að skrifa part af lausn skal taka það fram. [Sjá nánar á upplýsingasíða um gervigreind hjá HÍ](https://gervigreind.hi.is/).

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.1

---

| Útgáfa | Lýsing        |
| ------ | ------------- |
| 0.1    | Fyrsta útgáfa |
