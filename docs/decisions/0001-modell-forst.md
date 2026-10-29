# ADR 0001: Modell før implementasjon

**Status:** Godkjent arbeidsprinsipp  
**Dato:** 2026-10-29

## Bakgrunn

Flere IKAMR-apper skal samarbeide om felles katalog, innleveringer, uttrekk, lagringsoversikt og analyser. Direkte implementering fra dagens Excel kan låse modellen til regnearkets struktur.

## Beslutning

Først dokumenteres og godkjennes begreper, konseptuell og logisk datamodell og integrasjonsprinsipper. Deretter utvikles SQL, importer, migrasjoner og apper. Offentlig GitHub-repo inneholder bare struktur og generiske kontrakter, aldri operative depotdata eller lokal installasjonskonfigurasjon. Arbeidsflyten er delta-add, og prosjektansvarlig styrer Git.

## Konsekvens

Prosjektet begynner med dokumentasjon og Issues. Operativ database og kode utvikles senere, basert på godkjent modell.
