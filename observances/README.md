# Observance organization

The engine recursively loads YAML beneath this directory.

- `feasts/major/` contains major feasts.
- `feasts/minor/` is reserved for minor feasts.
- `saints/<type>/` groups saints by a practical subtype such as `martyrs/`,
  `monastics/`, or `hierarchs/`.
- Non-human commemorations use their own general type, such as
  `angels/archangels/`.

These paths are a maintenance taxonomy only. A document's stable `id` is its
reference key and its YAML fields determine liturgical behavior.
