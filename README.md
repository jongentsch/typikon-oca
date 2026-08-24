# Experimental OCA tradition pack

[![CI](https://github.com/jongentsch/typikon-oca/actions/workflows/ci.yml/badge.svg)](https://github.com/jongentsch/typikon-oca/actions/workflows/ci.yml)

This is an engineering fixture for `typikon-engine`, not an approved or
complete OCA Typikon.

The pack defines complete ordered structures for Vespers, Great Vespers,
Matins, and Divine Liturgy, including fixed/changeable components and the
Chrysostom/Basil forms. Rank profiles express major-feast, six-stichera, and
lesser-commemoration requirements.

The official OCA Great Vespers outline and dated orders ground the Ven. Pimen
7+3 and Archangel Michael 6+4 Lord-I-Call witnesses. Their saint material now
lives directly in each observance document. Rules supply Octoechos material
and admit the observance's contribution; they do not manufacture a synthetic
saint resource ID.

Twelve major feasts are discovered from the date alone. Official OCA feast
pages and service sources remain authority evidence, while missing
component-level perennial propers compile as explicit `unresolved` entries.
This prevents a dated order from being reused silently in another year.

The former bundle wrappers are preserved only under
`archive/legacy-resource-bundles/` for migration history and are not loaded.

```console
cd ../typikon-engine
cargo run -p typikon-cli -- validate ../typikon-oca
cargo run -p typikon-cli -- compile-date --pack ../typikon-oca --date 2026-12-25
```

License selection is pending.
