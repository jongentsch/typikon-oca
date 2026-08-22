# Experimental OCA tradition pack

This is a runtime resource pack for the sibling `typikon-engine` project. It is
an engineering fixture, not an approved or complete OCA Typikon.

Its two date-free observances are named `*-context` on purpose. They exercise
the two ordinary-Sunday cases stated in the OCA's published Great Vespers
outline without inventing a saint's date or rank classification. A caller must
select the desired context explicitly.

No liturgical text is included. The materials are semantic specifications only.

```console
cd ../typikon-engine
cargo run -p typikon-cli -- validate ../typikon-oca
cargo run -p typikon-cli -- compile-service --pack ../typikon-oca \
  --date 2026-08-22 --service great_vespers --tone tone_3 \
  --observance lesser-saint-context
```

License selection for this tradition pack is pending and independent of the
engine's license.
