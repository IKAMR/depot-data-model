# Issues-oppsett og første arbeidsoppgaver

**Status:** Forslag. Ingen Issues er opprettet på GitHub av utviklingsassistenten.

## Issue-maler

GitHub vil tilby disse malene etter første commit:

- `Datamodell og begreper`
- `Integrasjon og handshake`
- `Forslag og dokumentasjon`

De ligger i `.github/ISSUE_TEMPLATE/`. Bruk gjerne dem når du oppretter Issues manuelt.

## Anbefalte labels (opprettes manuelt)

| Label | Formål |
| --- | --- |
| `domain:catalog` | Bevaring, system, arkivskaper og eier |
| `domain:delivery` | Innlevering, pakke, uttrekk, variant |
| `domain:storage` | Disker, SAN, filer, duplikater |
| `domain:validation` | Evidens, validering, vurdering |
| `domain:integration` | Handshake, kontrakt, API |
| `type:model` | Begreper, felter og relasjoner |
| `type:decision` | Viktige modellbeslutninger |
| `type:documentation` | Struktur og veiledninger |
| `status:discussion` | Under avklaring |
| `status:ready` | Klar for gjennomføring |

Maler og labels er to ulike GitHub-funksjoner: ZIP-en inneholder malene, men labels må opprettes i repoets innstillinger dersom du vil ha disse navnene.

## Forslag til de første 8 Issues

### 1. [Modell] Definere bevaring og bevaringsnummer

Avklare hva en bevaring representerer, normalformatet `FFKK_nnn`, historiske/spesielle identifikatorer og koblingen til arkivskaper og system.

**Ferdig når:** En faglig definisjon med eksempler, unntak og identitetsregler er godkjent i `02-begreper-og-identiteter.md`.

### 2. [Modell] Relasjoner mellom innlevering, leveransepakke og uttrekk

Håndtere flere uttrekk per innlevering, flere innleveringer per bevaring og flere bevaringer i samme innlevering.

**Ferdig når:** Konseptuelle relasjoner og kardinaliteter er dokumentert med syntetiske testtilfeller.

### 3. [Modell] Avklare uttrekk, representasjon, variant og kopi

Skille nytt uttrekk fra kryptert arkiv, TAR, DIAS SIP, utpakket arbeidsvariant og eksakt fysisk kopi.

**Ferdig når:** Kriterier og eksempler er dokumentert for hvert tilfelle.

### 4. [Modell] Arkivskaper, eier og tidsavhengige relasjoner

Avklare endring av eierkommune, historiske arkivskapere og forskjellen mellom arkivskaperkode og eierkode.

**Ferdig når:** Rolle- og historikkmodell er beskrevet uten å endre eksisterende identiteter.

### 5. [Modell] Lagringsressurs, volum, plassering og filforekomst

Definere lagringsmedier uavhengig av Windows-stasjonsbokstav, og dekke både eksterne disker og SAN.

**Ferdig når:** Modell for ressursidentitet, plassering og observasjon er avklart.

### 6. [Modell] Filinventar og duplikatklassifisering

Definere nødvendige metadata, kontrollsummer, mulige duplikater og bit-identiske duplikater, samt hvordan kopier og varianter skilles.

**Ferdig når:** Modellen dekker også generelle bilder/dokumenter uten kobling til bevaring.

### 7. [Integrasjon] Dataeierskap og DWM-handshake

Avklare felles referanser, kildeevidens, idempotent hendelsesutveksling og offline-klienter mellom DWM og MasterDb.

**Ferdig når:** Systemansvar, inngående/utgående opplysninger og minimumskontrakt er beskrevet.

### 8. [Modell] Kartlegge Excel-masterark mot felles fagmodell

Bruke Excel-kolonnenes betydning til å kontrollere om modellen dekker behovene. **Ingen dataimport, ingen reelle eksempler i repoet.**

**Ferdig når:** Et generisk feltkart og identifiserte modellhull er dokumentert.

## Foreslått rekkefølge

Start med 1-4 (identitet og innlevering). Deretter 5-6 (lagring og filinventar), fulgt av 7-8 (integrasjon og kildekartlegging). Hold Issues åpne inntil faglig gjennomgang er gjennomført.
