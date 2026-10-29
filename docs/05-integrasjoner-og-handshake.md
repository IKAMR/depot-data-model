# Integrasjoner og handshake

**Status: Prinsipputkast, ingen implementert API.**

## Mål

La Depot MasterDb, depotportalen, DWM, andre valideringsapper og filoversiktsapper bruke felles identiteter og utveksle metadata uten at de skriver direkte i hverandres databaser.

## Prinsipper som skal vurderes

- Kildeapp eier egne kjøringer, analyser og opprinnelig evidens.
- Felles modell definerer referanser til bevaring, innlevering, uttrekk, variant og filforekomst.
- Depotportalen viser bare informasjon som er egnet for aktuell publisering.
- Klientene kan være offline; mottak må håndtere repetisjoner og gjenopptak.
- Hendelser/kontrakter skal være sporbare og versjonerte.

## Spørsmål til første kontrakt

Hvem er avsender/dataeier? Hvilken hendelses-ID og referanse benyttes? Hvordan skilles hendelsestid fra mottakstid? Hva er reglene for idempotens, konflikt og omkjøring? Hvordan refereres evidens uten å flytte arkivinnhold?

**Forslag til første brukstilfelle:** DWM rapporterer et valideringsresultat for ett definert uttrekk. Endelig JSON-struktur avventer godkjent identitetsmodell.
