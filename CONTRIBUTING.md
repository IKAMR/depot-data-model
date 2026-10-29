# Bidrag til depot-data-model

Vi utvikler **fagmodell før implementasjon**. Beskriv forslag som GitHub Issues og avklar relasjoner, identiteter, ansvar og konsekvenser før skjema eller kode lages.

## Delta-add og Git

Prosjektansvarlig legger selv til leverte deltaer, tester, committer og pusher. Utviklingsassistenten gjør ikke direkte endringer på GitHub.

Ved endringer: oppdater berørt dokumentasjon; registrer vesentlige valg som ADR i `docs/decisions/`; dokumenter fremtidige inkompatible endringer i kontrakter.

## Avgrensning

Kun generiske strukturer og syntetiske eksempler hører hjemme her. Ikke legg inn operative databaser, reelle depotregistre, uttrekk, analyser, disk-/SAN-konfigurasjoner, faktiske filinventarer eller hemmeligheter.

`.gitignore` alene er ikke en garanti. Gjennomgå `git status` og `git diff --cached` før hver commit.

Faglig dokumentasjon skrives primært på norsk. Maskinlesbare felt- og skjemanavn avtales ved modellgodkjenning.
