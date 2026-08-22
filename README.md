# Experimental OCA tradition pack

[![CI](https://github.com/jongentsch/typikon-oca/actions/workflows/ci.yml/badge.svg)](https://github.com/jongentsch/typikon-oca/actions/workflows/ci.yml)

This is a runtime resource pack for the sibling `typikon-engine` project. It is
an engineering fixture, not an approved or complete OCA Typikon.

Its two dated observances exercise the ordinary-Sunday cases stated in the
OCA's published Great Vespers outline. Official service orders instantiate the
lesser-saint branch with Ven. Pimen the Great on 2023-08-27 and the
six-stichera branch with the Miracle of the Archangel Michael at Colossae on
2026-09-06.

The outline is represented as a `source`; the reusable 7+3 and 6+4
interpretation is a `scoped_claim` citing that source; and each official dated
service order is a `dated_witness`. This keeps a date-specific resolved result
distinct from the general rule it confirms.

No liturgical text is included. The materials are semantic specifications only.

```console
cd ../typikon-engine
cargo run -p typikon-cli -- validate ../typikon-oca
cargo run -p typikon-cli -- compile-service --pack ../typikon-oca \
  --date 2023-08-26 --service great_vespers
```

This fixture pack uses Revised Julian fixed dates. The generic engine also
supports Julian fixed-date projection for a future Old Calendar pack or OCA
calendar profile. The caller does not supply the calculated weekly tone.

License selection for this tradition pack is pending and independent of the
engine's license.

GitHub Actions validates the pack with the sibling engine's CLI and compiles
both dated cases on every push and pull request.
