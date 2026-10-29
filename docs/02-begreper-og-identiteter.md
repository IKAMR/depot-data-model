# Begreper og identiteter

**Status: Arbeidsutkast.** Definisjonene må avklares i Issues.

| Begrep | Foreløpig forklaring |
| --- | --- |
| Arkivskaper | Enhet eller organisasjon som skapte arkivet |
| Eier | Organisasjon med eierskap/ansvar på et bestemt tidspunkt |
| Bevaring | Faglig identifisert bevaring, normalt med nummer `FFKK_nnn` |
| Innlevering | Registrert mottak, normalt `E-FFKK-YYYY-nnnn` |
| Leveransepakke | Konkret innlevert pakning eller leveransestruktur |
| Uttrekk | Logisk uttrekk som kan relateres til bevaring og innlevering |
| Innholdsvariant | Representasjon eller bearbeiding av et logisk uttrekk |
| Filforekomst | Observert fil på et lagringssted til et tidspunkt |
| Analyse/evidens | Resultater og kildereferanser fra valideringsverktøy |

## Ulike identifikatorer

- `FFKK_nnn` er i normaltilfellet bevaringsnummer knyttet til **arkivskaper**.
- `E-FFKK-YYYY-nnnn` er i normaltilfellet innleveringsnummer knyttet til **eierkommune**, år og innleveringens løpenummer.
- Arkivskaper og eier kan ha ulike koder, og historiske og spesielle identifikatorer må kunne representeres.
- Faglige identifikatorer skal ikke forveksles med eventuelle interne nøkler i fremtidige databaser.

## Modellbehov

Samme bevaring kan være knyttet til flere innleveringer. En innlevering kan inneholde flere uttrekk, og potensielt uttrekk fra ulike bevaringer. Innholdsvarianter er ikke automatisk nye uttrekk; identiske fysiske kopier er heller ikke nye uttrekk.

**Åpent:** eksakt definisjon av bevaring/uttrekk, relasjonskardinaliteter, historisering, intern identitet og feltkrav.
