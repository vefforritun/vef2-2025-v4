# Vefforritun 2, 2025, verkefni 4: React framendi

Verkefnið snýst um að setja upp react framenda fyrir vefþjónustu gerða í verkefni 3.

## Markmið

- Uppsetning og notkun á React með [Next.js](https://nextjs.org/).
- Noktun á React components með props og state.
- Routing í React verkefnum.

## Vefþjónustur og gögn

Þið getið notað þá vefþjónustu sem þið smíðuðuð í verkefni 3 eða notað [sýnilausn á verkefni 3](https://github.com/vefforritun/vef2-2025-v3-synilausn) (gefin út 10. mars).

## Virkni

Setja skal upp a.m.k. þrjár síður:

- Forsíðu sem birtir flokka með hlekk á þann flokk.
- Flokkasíðu sem birtir spurningar í gefnum flokk, ef flokkur er ekki til skal birt 404 síðu.
- Síðu sem leyfir að vinna með gögn, eitt af eftirfarandi:
  - Búa til, breyta og eyða flokk.
  - Búa til spurningu með svörum.
  - Breyta spurningu með svörum.

Setja skal upp gagnvirkni, sjá að neðan.

Nota skal annaðhvort `pages/` möppu eða _app router_ (`app/` mappa) fyrir í Next.js uppsetningu.

### Forsíða

Forsíða með einhverjum titli og flokkar með hlekkjum, t.d. endurnýta viðmót og útlit úr verkefni 2.

### Flokkasíða

Birting á öllum spurningum í flokki. Ef flokkur er ekki til skal birta 404 síðu.

Spurningar skulu birtar með öllum svörum. Hægt að svara spurningu og fá endurgjöf um svar. Hægt að endurnýta viðmót og útlit úr verkefni 2.

### Unnið með gögn

Eitt af eftirfarandi:

- Búa til, breyta og eyða flokk.
- Búa til spurningu með svörum.
- Breyta spurningu með svörum.

Ef villur koma upp frá vefþjónustu skal birta þær, bæði ef upp kemur almenn `500` villa og ef upp koma villur vegna notanda, t.d. `400` villa.

Ekki þarf að útfæra neina auka validation í framendanum fyrir utan að setja viðeigandi attribute á `<input>` ef það er talið nauðsynlegt.

Hægt er að útfæra fleiri en eitt atriði til upphækkunar, hámarkseinkunn 10.

### Components

Setja skal upp a.m.k. fimm componenta sem halda utan um viðeigandi stöðu og taka við gögnum gegnum props. Það er frjálst að útbúa fleiri componenta ef það er nauðsynlegt.

Hugmyndir að componentum:

- `Layout` component sem heldur utan um header, efni og footer á síðu.
- `List` component sem birtir lista af atriðum.
- `Detail` component sem birtir stakt.
- Form componenta: `Form`, `Input` og `Button`. Ekki þarf að útbúa sértæka componenta fyrir lengri texta eða tölur fyrir einingar.

## Tæki, tól og test

Setja skal upp verkefni með NextJS.

Setja skal upp (eða nota uppsettningu með viðeigandi framework) `eslint`. Engar villur skulu vera til staðar.

Ekki er krafa um að skrifa test.

## Annað

Grunnslóð (_base url_) á vefþjónustu skal geyma í env breytu sjá [skjölun fyrir NextJS](https://nextjs.org/docs/pages/building-your-application/configuring/environment-variables#exposing-environment-variables-to-the-browser).

Ef notaðar eru vefþjónustur úr verkefni 3 getur verið gott að hafa vefþjónustur keyrandi _locally_, þá er viðeigandi slóð sett í env breytu, t.d. `NEXT_PUBLIC_API_BASE_URL=http://localhost:5000/`.

## GitHub og hýsing

Setja skal upp vefinn á Vercel.

## Mat

- 10% — Tengt við vefþjónustu.
- 20% — Forsíða sem birtir flokka.
- 20% — Flokkasíða sem birtir spurningar.
- 20% — Unnið með gögn.
  - Aukalega +10% fyrir hvert auka atriði.
- 20% — Components útfærðir, a.m.k. fimm.
- 10% — Tæki, tól og test; GitHub og hýsing.

Hámarkseinkunn er 100% eða 10.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri miðvikudaginn 5. mars 2025.

## Skil

Skila skal í Canvas í seinasta lagi fyrir lok dags fimmtudaginn 20. mars 2025.

Skil skulu innihalda:

- Slóð á verkefni keyrandi.
- Slóð á GitHub repo fyrir verkefni. Dæmatímakennurum skal hafa verið boðið í repo. Notendanöfn þeirra eru:
  - `osk`
  - `ofurtumi`
  - `tomasblaer`

## Einkunn

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ef stórt mállíkan (LLM, „gervigreind“, t.d. ChatGTP) er notað til að skrifa part af lausn skal taka það fram. [Sjá nánar á upplýsingasíða um gervigreind hjá HÍ](https://gervigreind.hi.is/).

Sett verða fyrir ([sjá nánar í kynningu á áfanga](https://github.com/vefforritun/vef2-2025/blob/main/namsefni/01.kynning/1.kynning.md)):

- fimm minni sem gilda 10% hvert, samtals 50% af lokaeinkunn.
- tvö hópverkefni þar sem hvort um sig gildir 20%, samtals 40% af lokaeinkunn.
- einstaklingsverkefni sem gildir 15–25% af lokaeinkunn.

---

> Útgáfa 0.3

| Útgáfa | Breyting      |
| ------ | ------------- |
| 0.1    | Fyrsta útgáfa |
| 0.2    | Taka út að skila þurfi á Netlify |
| 0.3    | Laga hlekk á sýnilausn að v3 |
