# Arbeidsflyt og versjonering

**Status: Foreslått arbeidspraksis.**

1. Opprett Issue med faglig behov, eksempel og avgrensning.
2. Drøft begreper og relasjoner; beskriv alternativer.
3. Registrer vesentlig beslutning som ADR i `docs/decisions/`.
4. Oppdater konseptuell og deretter logisk datamodell.
5. Definer og test fremtidige maskinlesbare skjema/kontrakter først når definisjonene er godkjent.
6. Implementer senere SQL, migrasjoner, importer og apper.

## Delta-add

Endringer leveres med relative stier i delta-ZIP. Prosjektansvarlig legger dem til lokalt og står selv for test, commit og push. Ingen automatiske GitHub-endringer.

## Dokumentstatus

Bruk **Arbeidsutkast**, **Til vurdering**, **Godkjent** eller **Utgått**. Første commit er prosjektetablering, ikke en godkjent datamodellrelease.

## Versjonering og kompatibilitet

Versjonering av skjemafiler og API-kontrakter velges før første maskinlesbare release. Inkompatible endringer må ha dokumenterte migrerings- og kompatibilitetsregler.
