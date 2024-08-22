# Vefforritun 1, 2024: Verkefni 2, HTML #2

## Markmið

- Vinna með og velja HTML element.
- Nota HTML validator og huga að því hvernig HTML er skrifað.
- Huga að aðgengi og nota aXe tólið.

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2024-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2024-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2024-v4) setur upp útlit (e. layout).
- [Verkefni 5](https://github.com/vefforritun/vef1-2024-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2024-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Lýsing

Setja skal upp fjórar síður fyrir spilabúð, aðgengilegar af internetinu (gegnum Netlify):

- Forsíða Spilabúðarinnar.
- Spilasíðu.
- Viðburðasíðu.
- Skráning á viðburð.

## Síður

### Efni og möppur

Gefið efni er í textaskrám undir `gogn/` og er Markdown formi. Ekki á að birta nákvæmlega það efni sem kemur fram heldur fylgja leiðbeiningum í hverri skrá fyrir sig.

Gefnar myndir eru í `myndir/` og skal vísa í þær þar (nota þarf relative vísun úr `sidur/` yfir í `myndir/` þar sem við á.)

Gefin er tóm mappa `sidur/` sem skal innihalda allar síður _fyrir utan_ forsíðuna.

### Sameiginlegt

Allar síður skulu innihalda valmynd sem vísar á allar aðrar síður og merkja valda síðu á einhvern hátt, sjá `gogn/valmynd.md`.
Athugið að allar síður fyrir utan forsíðu verða að vera undir `sidur/` möppu.

Allar síður skulu hafa fót (gögn neðst á síðunni) með upplýsingum um opnunartíma, staðsetningu og samfélagsmiðla (notum HÍ samfélagsmiðla sem hlekki), sjá `gogn/fotur.md`.

Allar síður skulu hafa lýsigögn skilgreind fyrir `description`, `og:title`, `og:description` og `og:image` (alltaf `myndir/sharing.jpg`). Prófið með [Facebook Debugger](https://developers.facebook.com/tools/debug/) eða [OpenGraph Social Previewer](https://www.opengraph.xyz/) til að sjá hvort gögn séu rétt eftir að síða er sett upp á Netlify.

Allar síður nema forsíða skulu hafa tengil neðst í efni með textanum „Aftur á forsíðu“.

Allar síður skulu hafa fyrisögn og „beint í efni“ hlekk á eftir fyrirsögn, en á undan valmynd. Hlekkur sem leyfir þeim sem nota skjálesara að sleppa við að hlusta á valmynd.

### Forsíða

`index.html`, forsíða með texta tilgreindum í `gogn/index.md`.

Inniheldur inngangstexta og yfirlit með vísunum í aðrar síður.

### Spilasíða

Síðan skal eiga heima undir `sidur/spil.html`, með lista af spilum, texta í `gogn/spil.md` og lista af spilum (og tengdum myndum) í `gogn/spil.csv`.

Spilamyndir og gögn frá [BoardGameGeek](https://boardgamegeek.com/browse/boardgame).

### Viðburðir

Listi af viðburðum með efni í `gogn/vidburdir.md`. Hver og einn viðburður ætti að tengja á skráningarsíðuna, ekkert þarf að tilgreina hvaða viðburð er komið frá.

### Skráning á viðburði

Síða með formi til að skrá sig á viðburð, svæði og reitir skilgreindir í `gogn/form.md`.

Aðeins á að setja upp formið, **engin** forritun fyrir virkni í formi með JavaScript eða í bakenda.

### Myndir

Vísað er í myndir á viðeigandi stöðum í efni. Myndir eru í `myndir/` möppu og skulu ekki færðar. Leyfilegt er að minnka myndir eða setja `width` eigindi á mynd til að takmarka breidd þeirra.

Myndir frá Unsplash eftir:

- [Tem Rysh](https://unsplash.com/photos/black-trike-parked-near-soter-F6-U5fGAOik)
- [Ross Sneddon](https://unsplash.com/photos/person-holding-jigsaw-puzzle-piece-sWlDOWk0Jp8)
- [Dave Photoz](https://unsplash.com/photos/blue-yellow-and-green-plastic-blocks-FdTmaUlEr4A)

## Útlit

Ekki er gefin forskrift að útliti, þar sem verkefnið snýst um að setja upp merkingarfræðilegt HTML sem snýst um að huga að merkingarfræði _ekki_ útliti.

Ekki þarf eða ætti að gera neitt með CSS. Ef þið viljið fara lengra og byrja á CSS skulið þið passa ykkur á að vanda til verka og helst bera undir kennara eða dæmatímakennara.

## Almennt

- **Nýta skal merkingarfræðilega viðeigandi element**.
- Valmynd skal útfæra með því að afrita og breyta milli síðna, ekki er krafa um neina „forritun“ til að útbúa valmynd.
- Síður skulu nota `utf-8` stafasett.
- Passa skal upp á að hafa snyrtilega uppsettan kóða þar sem inndráttur er samræmdur.
- Allar síður skulu vera villulausar ef prófaðar með [HTML validator](https://validator.w3.org/).
- Allar síður skulu vera án aðgengisvillna ef prófaðar með [aXe](https://www.deque.com/axe/), setjið upp viðbót í vafra.

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo.

## Mat

- 20% – Merkingarfræðileg element og síður án villna frá HTML validator og aXe validator.
- 10% – Haus, valmynd og fótur eftir forskrift.
- 10% – Forsíða uppsett eftir forskrift.
- 30% – Spilasíða uppsett eftir forskrift.
- 15% – Viðburðasíða uppsett eftir forskrift.
- 15% – Skráning á viðburði síða uppsett eftir forskrift.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 26. ágúst 2024.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 5. september 2024.

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
