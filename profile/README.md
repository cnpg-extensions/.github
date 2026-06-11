![not-cloudnative-pg](./not-cnpg.png)

# not-cloudnative-pg

A home for PostgreSQL extension container images that are compatible with
[CloudNativePG](https://cloudnative-pg.io/) but cannot be accepted into the
official [cloudnative-pg/postgres-extensions-containers](https://github.com/cloudnative-pg/postgres-extensions-containers)
project due to licensing constraints.

## Why does this exist?

The upstream CNPG project requires every component in an extension image to be
covered by a license on the
[CNCF Allowed Third-Party License Policy](https://github.com/cncf/foundation/blob/main/policies-guidance/allowed-third-party-license-policy.md).
Some excellent, widely-used extensions contain source files under licenses that
are not on that list (e.g. Vixie-Cron, GPL). The upstream maintainers will not
file license exceptions for new extensions — which is a reasonable governance
decision, not a criticism.

## Repositories

| Repository | Description |
|---|---|
| [postgres-extensions-containers](https://github.com/not-cloudnative-pg/postgres-extensions-containers) | Container images for PostgreSQL extensions blocked from upstream by licensing |

## Usage

See the
[postgres-extensions-containers README](https://github.com/not-cloudnative-pg/postgres-extensions-containers#readme)
and each extension's directory for `Cluster` and `Database` YAML examples.

## Relationship to upstream

This org tracks the upstream build infrastructure as closely as possible. The
only intentional divergence from
[cloudnative-pg/postgres-extensions-containers](https://github.com/cloudnative-pg/postgres-extensions-containers)
is the removal of upstream-maintained extensions and the addition of
license-blocked ones.
