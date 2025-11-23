# opengov-privacy-data
**Produktive Daten**: RoPA-Struktur (aus Aktenplan), ein SSP pro Verfahren, optionale POA&M/Assessment-Artefakte, Evidence-Metadaten (nur RLinks + Hashes).
**Strenge Rechte** (nur Data-Maintainer).

**Versionierung/Audit** via Git History & PR-Reviews.

## Verzeichnisse

``` bash
opengov-privacy-data/
├─ tenants/
│  └─ <org-slug>/
│     ├─ ropa/
│     │  ├─ ropa.json                       # RoPA-Struktur (Prozesshandbuch)
│     │  └─ index.json                      # optionale Übersicht/Inventar
│     ├─ procedures/
│     │  └─ <procedure-id>/
│     │     ├─ ssp.json                     # SSP der Verarbeitungstätigkeit
│     │     ├─ poam.json                    # Findings/Measures (optional)
│     │     ├─ assessment/
│     │     │  ├─ plan.json                 # AP (optional)
│     │     │  └─ results.json              # AR (optional)
│     │     └─ evidence/
│     │        ├─ registry.json             # nur Metadaten+RLinks+Hashes
│     │        └─ (keine Binärfiles hier, s.u.)
│     └─ profiles/
│        └─ resolved/…                      # optional, wenn tenant-spezifisch
└─ README.md

```