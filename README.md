# TFLint + Renovate Example 2

## Setup

- Each module lists only the providers which are being required for this module using exact version constraints

## Observation

- ✅ TFLint is happy
- ❌ Renovate upgrades providers versions in `.tf` files of child modules but does not update the lock file -> `terraform init` fails with _"locked provider xyz does not match configured version constraint"_

## Workarounds

- manually updating the lock file
