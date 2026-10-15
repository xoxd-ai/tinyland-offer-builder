# tinyland-offer-builder (retired)

Retired on 2026-10-14 under rulings RU2/RU7. Nothing here is maintained.

The Schema.org `Offer` builder now lives in
[xoxd-ai/tinyland-activitypub](https://github.com/xoxd-ai/tinyland-activitypub)
as the `./offer-builder` subpath export, from version 1.0.0:

- Bazel: `bazel_dep(name = "tummycrypt_tinyland_activitypub", version = "1.0.0")`
  (or later) from [xoxd-ai/bazel-registry](https://github.com/xoxd-ai/bazel-registry),
  in place of `tummycrypt_tinyland_offer_builder`.
- Imports: `@tummycrypt/tinyland-activitypub/offer-builder` in place of
  `@tummycrypt/tinyland-offer-builder`. The API is unchanged.
- The GNU Taler transaction type is `taler`. The source in this repository
  still spells it `talar`; the registry 0.2.0 entry patched it.

The `tummycrypt_tinyland_offer_builder` 0.2.0 registry entry stays resolvable
and is marked deprecated. Nothing is yanked or unpublished. In-house packages
ship only as Bazel modules (RU6), so no npm release follows.

This repository is archived and read-only.
