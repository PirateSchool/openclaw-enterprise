# Shared release disposition

The canonical configuration is [release-publication.json](release-publication.json). It is validated by the shared provider; it does not grant release, registry, cloud or deployment authority.

Shared publication is explicitly disabled. Shared publication is disabled: imported CLI, OCI and chart publishers admit only openclaw/openclaw-enterprise; this fork has no native publication authority.

## Existing native owner

`.github/workflows/container-publish.yml` remains the native operation boundary. The imported native publisher admits the upstream repository and protected environment. This fork remains an upstream-derived source project; its imported publisher does not establish fork publication authority.

## Remaining qualification

- Establish reviewed native fork ownership before enabling CLI, OCI or chart publication.
- Qualify upstream/private-provider access, both native architectures, exact prepared bytes and actual destination readback.

The configured notes directory is reserved for future exact-source reviewed product content. No product version, tag, artifact, notes bundle or publication receipt is fabricated here. Source configuration validation is separate from native runtime and destination qualification.

The shared implementation belongs to `agencyftw/.github`. Do not add local formatters, validators, publication engines or retry loops to close these gaps. Native adapters must call its pinned APIs after their existing admission gates pass.

This public fork has no qualified access path to the private canonical provider. Its workflows remain unchanged. The configuration was validated against the exact shared core during preparation; hosted provider resolution and native adapter integration remain unqualified. Do not hand-copy the generic implementation to bypass access policy.
