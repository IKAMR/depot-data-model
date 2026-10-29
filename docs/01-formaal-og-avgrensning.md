# Formål og avgrensning

**Status: Utgangspunkt for modelleringen.**

## Formål

Definere en felles, teknologiuavhengig informasjonsmodell for IKAMRs depotkatalog, innleveringer, uttrekk, validering, lagringsforekomster og filinventar. Modellen skal senere kunne implementeres i lokal SQLite eller en sentral database og brukes av flere selvstendige applikasjoner.

## Fire sentrale skiller

1. **Repo og operativ database:** GitHub inneholder kun struktur og generiske kontrakter, aldri de lokale datafilene.
2. **Kataloginformasjon og arkivinnhold:** Operative databaser kan inneholde katalogopplysninger og analyser, men ikke selve arkivdokumentene.
3. **Logisk objekt og fysisk forekomst:** Ett uttrekk kan ha flere representasjoner og kopier på flere medier.
4. **Felles modell og lokal installasjon:** Diskoppsett, servernavn, stier og tilkoblinger er lokale forhold.

## Aktuelle systemer

- Depot MasterDb og en fremtidig sentral masterdatabase.
- Depotportal/frontend.
- Data Workflow Manager (DWM), Arkade 5, KDRS Query og andre analyse-/valideringsapper.
- Filoversiktsapper for eksterne disker og SAN, inklusive generelle dokument- og bildesamlinger.

## Utenfor oppstartsfasen

Databaseimplementasjon, importer fra Excel, scripts, filskanning, hashing og apper. Vi beskriver **hva** informasjonen er og **hvordan** den henger sammen før vi bestemmer teknisk lagring.
