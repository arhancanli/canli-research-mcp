# Where this code lives

This repository is the standalone home of the `canli-research-mcp` package, published so the server can be
installed, scanned and reviewed on its own. It is imported from the `mcp-research/` directory of
[arhancanli/canlicapital](https://github.com/arhancanli/canlicapital/tree/main/mcp-research), which is
where changes are made and tested; this repository is updated from it.

Imported from canlicapital commit `10121fee41325d6e04a3b17715d1ca619a18bfd6`.

- npm: https://www.npmjs.com/package/canli-research-mcp
- MCP Registry: `io.github.arhancanli/canli-research-mcp`
- Hosted endpoint (no install): https://canlicapital.com/mcp/research

The Claude Desktop bundle attached to each release is built by `.github/workflows/release.yml` from
the files committed at the release tag (`mcp-research/mcpb/build.sh` in canlicapital does the same), with
a signed build provenance attestation:

```bash
gh attestation verify canli-research.mcpb --repo arhancanli/canli-research-mcp
```

Files owned by this repository and kept across syncs: `.github/` (CI, CodeQL, OpenSSF Scorecard,
Dependabot, and the release workflow that builds, signs and attaches the Claude Desktop bundle),
`.gitignore`, `MIRROR.md`, `glama.json`, and the digest-pinned base image in `Dockerfile`.
