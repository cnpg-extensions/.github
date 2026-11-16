[![CNPG Extensions](./cnpg-extensions.png)](https://cnpg-extensions.github.io/)

# CNPG Extensions

**The COMPLETE and SECURE Way to run Postgres on Kubernetes**

CloudNativePG with over 100 extensions, clear licensing, deep vulnerability
tracking, and rapid package updates.

**[Explore extensions](https://cnpg-extensions.github.io/extensions/)** ·
[Get started](https://cnpg-extensions.github.io/getting-started/) ·
[Security and image verification](https://cnpg-extensions.github.io/security/)

## More of the Postgres ecosystem, available for CloudNativePG

CNPG Extensions welcomes any OSI-approved license, including outside CNCF’s
permitted set. That broader licensing scope brings more of the Postgres ecosystem
into the catalog.

The upstream CloudNativePG project follows the
[CNCF Allowed Third-Party License Policy](https://github.com/cncf/foundation/blob/main/policies-guidance/allowed-third-party-license-policy.md).
This project complements that scope with additional extensions, including ones
whose shipped components use licenses outside that policy. The catalog also
includes extensions with CNCF-compatible licenses; it is not limited to
license-blocked extensions.

We prefer Debian packages from PGDG for their community, licensing, and
dependency-management foundations. PGRX and Universe build paths support
additional source-built extensions under the project's
[inclusion and licensing policies](https://github.com/cnpg-extensions/postgres-extensions-containers/blob/main/source-build/README.md).

## Repositories

| Repository | Description |
|---|---|
| [postgres-extensions-containers](https://github.com/cnpg-extensions/postgres-extensions-containers) | Debian, PGRX, and Universe extension recipes, build and release workflows, usage examples, and contribution guides |
| [artifacts](https://github.com/cnpg-extensions/artifacts) | Generated `ClusterImageCatalog` manifests combining upstream CloudNativePG extensions with extensions maintained here |
| [cnpg-sbom-generator](https://github.com/cnpg-extensions/cnpg-sbom-generator) | BuildKit SBOM generator that identifies shipped packages, dependency versions, checksums, and license evidence |
| [cnpg-extensions.github.io](https://github.com/cnpg-extensions/cnpg-extensions.github.io) | Website, searchable extension directory, and generated image evidence |
| [.github](https://github.com/cnpg-extensions/.github) | This organization's GitHub profile |

## Get started

Follow the [getting started guide](https://cnpg-extensions.github.io/getting-started/)
to configure update alerts, schedule catalog maintenance, and enable extensions
in your clusters and databases. Browse the
[extension directory](https://cnpg-extensions.github.io/extensions/) for individual
READMEs, available versions, licenses, and image evidence.

For images built here, signatures, provenance, and platform-specific SBOMs help
you verify the publisher and inspect shipped dependencies and licenses. The
[security guide](https://cnpg-extensions.github.io/security/) explains the Cosign,
Docker Buildx, Grype, and Grant commands. Evidence availability varies for images
published by upstream CloudNativePG.

## Relationship to upstream

We track the [CloudNativePG extension build infrastructure](https://github.com/cloudnative-pg/postgres-extensions-containers)
as closely as possible. Upstream-maintained extension recipes stay upstream;
our catalogs automatically incorporate their published entries. For the same
extension, Debian distribution, and PostgreSQL major version, the upstream
catalog entry takes precedence.

Additional work here includes a broader extension selection, source-build paths,
and dependency and license evidence for shipped files. Our SBOM generator
preserves CloudNativePG's inspection formats and tools. See the
[compatibility guide](https://github.com/cnpg-extensions/cnpg-sbom-generator#compatibility)
and [upstream workaround register](https://github.com/cnpg-extensions/postgres-extensions-containers/blob/main/WORKAROUNDS.md)
for technical details.

## Contribute

[Request a new extension](https://github.com/cnpg-extensions/postgres-extensions-containers/blob/main/CONTRIBUTING_NEW_EXTENSION.md)
or help improve packaging, documentation, and tests. A pull request is not
required to propose an extension.

For security issues in our packaging or build infrastructure, follow the
[private reporting policy](https://github.com/cnpg-extensions/postgres-extensions-containers/blob/main/security.md).
Report vulnerabilities in an extension itself directly to that extension's
project owners.
