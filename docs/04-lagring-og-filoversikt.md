# Lagring og filoversikt

**Status: Arbeidsutkast.**

## To bruksområder

**Uttrekk / bevaringspakker:** Hva er innlevert, hvilken innholdsvariant er lagret hvor, og hvilken kontroll/validering er utført?

**Generelt filinventar:** Hvilke bilder, skannede arkivbilder og dokumenter finnes på eksterne disker, servere og SAN? Hvilke er identiske, og hvilke er ulike versjoner?

## Foreløpige begreper

- **Lagringsressurs:** fysisk ekstern disk, server- eller SAN-ressurs.
- **Volum / monteringspunkt:** hvordan ressursen er tilgjengelig på en klient. Stasjonsbokstav alene er ikke stabil identitet.
- **Plassering:** filsti innenfor en bestemt ressurs, lagret i operative systemer.
- **Filforekomst:** observasjon av en fil ved et tidspunkt og en plassering.
- **Filidentifikasjon:** størrelse, kryptografisk kontrollsum og andre metadata.
- **Duplikatvurdering:** mulig treff, bit-identisk innhold eller relatert/transformert variant.

## Avklaringer

Hvordan identifisere ressurser på tvers av maskiner? Hvordan skille en observert fil fra en bekreftet eksisterende kopi? Hvordan dokumentere flytting, fravær og ny skanning? Hvordan unngå hashing av store mengder filer uten behov?

Skanning, duplikatdeteksjon og drift av disker/SAN implementeres **ikke** i dette repoet i oppstartsfasen.
