# CR-DE-CAT-02: Initial Population

| Field | Value |
|---|---|
| **CR** | CR-DE-CAT-02 |
| **Title** | Initial population: the org's verifiable persistent data structures |
| **Status** | Landed |
| **Layer** | Catalogue (L4 Data Foundation) |
| **Programme** | Org-wide catalog advancement (Wave 1) |
| **Repository** | `technehub-labs/dea-catalog-data-entities` |
| **Author** | Emmanuel A. Otchere |
| **Date** | 2026-11-02 |
| **Depends on** | CR-DE-CAT-01 (kit); CR-CATALOG-STRUCT-10/10A (generator) |
| **Trigger** | Wave 1 of the org-wide catalog advancement programme. DataEntity is the highest-centrality unpopulated entity (18 relationship endpoint lists); information-asset records name `derived-from` lineage into Data Entities as their deferred posture until canonical data-entity ids exist. |

## 1. Executive summary

Nine canonical Data Entity records are admitted, each an org-verifiable persistent data structure: the metamodel's SQLite schema (the org's canonical relational schema) and the record stores of the eight populated catalogs (processes 3,722; capabilities; business-objects 74; value-streams 111; information-classes 8; information-assets 7; roles; actors). Business-object realization (`dea:represents`) is deferred: the business-objects catalogue holds real-world entities (Customer, Invoice, Order), none of which these stores realize; no local substitute targets are invented.

## 2. Seed selection (FOUNDATIONS D-5)

Every seed cites a committed repository path corroborated at admission. No hypothetical or planned structures. The metamodel SQLite schema's companion per-table records are NOT admitted as separate seeds (137 tables would be a bulk derivation, not an evidence tranche); the schema record is the entry point and per-table records await a per-structure evidence CR.

## 3. Unblocked downstream (named, not landed here)

- Information-asset `derived-from` lineage: the IA records' deferred posture can now assert targets (e.g., the integrity report derived from the capabilities store). Owned by a future information-assets CR.
- The metamodel's `dea:derived-from`, `dea:exposes`, `dea:trained-on`, `dea:curates`, `dea:evidenced-by` endpoint lists that name DataEntity now have canonical target ids available.

## 4. Scope

In scope: 9 record subtrees (record + README), CATALOG.yaml regeneration, register row, CHANGELOG.

Out of scope: any represents assertion; per-table seeds; sibling catalogues; metamodel lifecycle backfill (wave-boundary CR).

## 5. Acceptance criteria

1. Gates 1-6 all `Findings: 0` with 9 canonical records.
2. `CATALOG.yaml` counts: entities 9, canonical 9, open_change_requests 0.
3. Authorship gate conformant.

## 6. NOT-list

1. No `dea:represents` assertions (deferred; no matching canonical business objects).
2. No per-SQLite-table records.
3. No schema or vocabulary changes.
