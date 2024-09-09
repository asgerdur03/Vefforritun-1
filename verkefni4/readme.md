# Vefforritun 1, 2024: Verkefni 4, CSS #2

## Markmið

- Nota CSS custom properties (variables, breytur)
- Nota flexbox til að stýra útliti
- Útfæra „card“ viðmót

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2024-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2024-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2024-v4) setur upp útlit (e. layout).
- [Verkefni 5](https://github.com/vefforritun/vef1-2024-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2024-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Verkefnið

Verkefnið er framhald af [verkefni 2](https://github.com/vefforritun/vef1-2024-v2) og [verkefni 3](https://github.com/vefforritun/vef1-2024-v23), nýtir það efni sem uppsett er í þeim og fylgir þeim verkefnalýsingum fyrir utan það sem tekið er fram hér. Leyfilegt er að nota [sýnilausn að verkefni 3](https://github.com/vefforritun/vef1-2024-v3-synilausn), sem gefin verður út föstudaginn 13. september.

Nú hafa eigendur Spilabúðarinnar skoðað fyrstu útgáfu af útliti en vilja gera nokkrar breytingar:

- Breyta valmynd þannig að hún sé lóðrétt og vinstra megin við efni.
- Breyta og samræma hvernig efni er birt og nýta svokallað korta („card“) viðmót.
- Bæta við efni á forsíðu.
- Stækka efnið í stærri skjám upp í `1200px` breitt.

Þessar breytingar sjást í uppfærðri fyrirmynd í `fyrirmynd/` möppu. Að auki nánari lýsing að neðan.

Aukalega skal laga kóða þannig að:

- Flexbox sé notað til að stýra útliti og með því fjarlægja notkun á `float`, `clear` og `display: inline-block` aðferðum til að stýra útliti.
- Nota CSS Custom properties (variables) til að stýra litum og öðrum stílum.

Sjá uppfært skjal með grunnstílum og breytum í `styles.css`.

Allt útlitið skal vera í `./styles.css` og **allar** HTML skrár skulu vísa í nákvæmlega þá skrá.

## Útlit

Fyrirmynd að útliti er í `fyrirmynd/` möppu. Öll skjáskot eru tekin í `1500px` breiðum Firefox vafra. Athugið að fyrirmyndir eru uppfærðar frá verkefni 3.

Bæta þarf við auka elementum við lausn/sýnilausn til að geta náð fram útliti.

Þar sem allt útlit skal útfæra í einni CSS skrá, skal huga að cascade og erfðum, þó er fullkomlega eðlilegt að endurtaka eigindi, en t.d. fyrir málsgreinar (`<p>`) þarf aðeins að taka fram einu sinni hvert margin þeirra er.

### Almennt

Gefið er `styles.css` skjal með grunn að lausn og athugasemdum.

Allt sem gildir í verkefni 2 og verkefni 3 gildir áfram í þessu verkefni.

### CSS Custom properties

Nota skal þau gildi sem eru gefin í `:root` reglunni í `styles.css` til að stýra gildum, þar með talið litum, leturstærðum og öðru sem gefið er.

Í CSS reglum sem notuð eru (hvort sem það er sýnilausn á verkefni 3 eða ykkar eigin) skal nota þessi gildi, það er að segja, ekki nota nota gildið úr `:root` reglunni með `var()` fallinu.

### Flexbox

Allstaðar þar sem `float`, `clear` og `display: inline-block` eru notað til að stýra útliti skal nota flexbox. Það getur verið eitthvað eða allt af þessu:

- Meginviðmót (haus, meginmál og fótur)
- Valmynd (en samt sjá að neðan)
- Kortaviðmót (en samt sjá að neðan)
- Fótur
- Efni á síðum (fyrir utan töflu)

Athugið að til að ná fram öllu því sem gefið er í fyrirmynd þarf að nota flexbox innan í flexbox, innan í flexbox, innan í flexbox og svo framvegis.

### Uppfærð valmynd

Færa skal valmynd úr því að vera fyrir neðan haus yfir í að vera lóðrétt og við hliðina á meginmáli. Að auki þarf að stækka pláss á meginmála og hækka upp í `1200px` hámarksbreidd.

### Kortaviðmót

Útfæra skal kortaviðmót fyrir efni á vefnum:

- Efni á forsíðu
- Efni á viðburðasíðu
- Form á bóka viðburð síðu

Þetta skal útfæra einu sinni og nota síðan rétta class selectora til að nýta. Sjá athugasemdir í `styles.css`.

### Nýtt efni á forsíðu

Nota skal kortaviðmót og það sem uppfært er í fyrirmynd til að bæta við eftirfarandi efni á forsíðu fyrir tvö spil:

- Brass: Birmingham. Ný komið aftur! Klassískt spil sem fær 8,41 í einkunn hjá BoardGameGeek. Skoða spil. Setja í körfu.
- Pandemic Legacy. Getið þið unnið saman til að stöðva heimsfaraldur? Spil sem fær 8,37 í einkunn hjá BoardGameGeek.. Skoða spil. Setja í körfu.

### Takmarkanir

Aðeins skal nota eftirfarandi eigindi, og ef tekið fram, viðeigandi gildi:

- `background-color`
- `border` og nánari skilgreiningar
- `box-sizing`
- `color`
- `display: flex;`
  - önnur flex eigindi og `gap`
  - ekki ætti að nota önnur gildi fyrir `display`, sjá að neðan
- `font-display`
- `font-family`
- `font-style`
- `font-weight`
- `list-style: none;`
- `margin-bottom` og `margin-top`
  - _ekki_ ætti að nota `margin-left` og `margin-right` heldur flexbox
- `padding` eigindi
- `src`
- `width`, `max-width`, `max-height`
- Þau eigindi notuð í `.sr-only` og ekki tiltekin hér ætti ekki að nota í annað.
- Ekki ætti að nota `vertical-align` og `float` til að stýra útliti.

Ekki skal nota önnur `display` gildi en `display: flex;` og ekki nota `text-align` til að miðja efni. `display: block` og `display: inline-block` má nota í sértækum tilfellum, sýnilausn notar fyrir mynd í kortum og formi.

Ekki þarf að huga að skalanleika (síðan þarf ekki að líta vel út í undir `1000px` skjá).

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo.

## Mat

- 20% – Snyrtilega uppsett og gilt CSS.
- 10% – Aðeins leyfileg eigindi og gildi notuð.
- 10% – CSS Custom properties fyrir gildi.
- 20% – Flexbox notað fyrir útlit.
- 10% – Uppfærð valmynd.
- 20% – Kortaviðmót.
- 10% – Nýtt efni á forsíðu.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 9. september 2024.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 19. september 2024.

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
