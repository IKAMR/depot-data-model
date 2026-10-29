# Depot Data Model

**Felles datamodeller, databasestrukturer og integrasjonskontrakter for IKAMRs depotforvaltning.**

[IKAMR](https://github.com/IKAMR) | [Data Workflow Manager](https://github.com/IKAMR/data-workflow-manager)

**Status:** Oppstart / konseptuell modellering. Det finnes foreløpig ingen godkjent databaseimplementasjon i dette repoet.

## Formål

Etablere en felles, teknologiuavhengig modell for kataloginformasjon og analyser knyttet til:

- arkivskaper, eier, bevaring og arkivsystem
- innlevering, leveransepakke, uttrekk og innholdsvarianter
- filinventar, lagringsmedier, fysiske forekomster og duplikater
- validering, evidens og depotvurdering
- handshake og integrasjon mellom selvstendige apper

Modellen skal kunne benyttes av lokal **Depot MasterDb**, fremtidig sentral database, **depotportal**, **Data Workflow Manager (DWM)**, andre valideringsapper og filoversiktsapper for eksterne disker og SAN.

## Kun struktur - ikke operative data

Repoet inneholder kun **datadefinisjoner, relasjoner, dokumentasjon, generiske skjema og fremtidige integrasjonskontrakter**. Ingen arkivdokumenter, uttrekk, operative SQLite-databaser, faktiske katalogdata, analyseresultater, filinventarer, diskoppsett eller lokale konfigurasjoner skal committes. Eksempler skal være syntetiske.

## Arbeidsrekkefølge

1. Avklare begreper, identiteter og avgrensninger.
2. Utarbeide **konseptuell datamodell** og bli enige om relasjoner.
3. Utarbeide **logisk datamodell** med datadefinisjoner.
4. Definere **versjonerte integrasjonskontrakter** (handshake).
5. Først deretter lage SQL, migrasjoner eller referanseimplementasjoner.

**Ingen Excel-import eller oppbygging av operativ database i denne fasen.**

## Dokumentasjon

- [Dokumentasjonsoversikt](docs/README.md)
- [Formål og avgrensning](docs/01-formaal-og-avgrensning.md)
- [Begreper og identiteter](docs/02-begreper-og-identiteter.md)
- [Konseptuell datamodell](docs/03-konseptuell-datamodell.md)
- [Lagring og filoversikt](docs/04-lagring-og-filoversikt.md)
- [Integrasjoner og handshake](docs/05-integrasjoner-og-handshake.md)
- [Arbeidsflyt og versjonering](docs/06-arbeidsflyt-og-versjonering.md)
- [Forslag til Issues og videre arbeid](docs/07-issues-og-veikart.md)
- [Arkitekturbeslutninger](docs/decisions/README.md)

Modelltekst er **arbeidsutkast** der ikke annet er uttrykkelig angitt. Faglige valg avklares i Issues og dokumenteres før implementasjon.

Se [CONTRIBUTING.md](CONTRIBUTING.md) for bidrag og delta-add-prinsippet. Lisens er foreløpig ikke valgt: et offentlig repo er ikke automatisk åpen kildekode med gjenbruksrett.
