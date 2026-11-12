# dpoc-nitroso.carbon

Platform repo for `nitroso` — the notes platform (tin + web). `platform.yaml` holds the platform facts
(landscapes/stages per PLAN §8, maturity). `infra/app` renders a ConfigMap
`nitroso-platform` into namespace `nitroso`; `infra/primordial` is empty-but-valid
(service repos own the dependency records).

TEMPLATE note (argon): not pushed until the drill creates it.

## Release
Push a tag `vX.Y.Z` (needs `DPOC_REG_PASSWORD`): pushes charts
`reg.dpoc.specpenguin.dev/charts/dpoc-nitroso:X.Y.Z` and `.../dpoc-nitroso-primordial:X.Y.Z` (no image).
