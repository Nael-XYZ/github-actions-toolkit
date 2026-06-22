# GitHub Actions Toolkit 🧰

Reusable GitHub Actions workflows and composite actions.

## Actions

- **setup-tools**: Auto-detect + cache dependencies
- **matrix-build**: Parallel builds across OS/arch
- **deploy-gate**: Manual approval + canary
- **secrets-rotate**: Auto-rotate secrets

## Usage

```yaml
- uses: org/actions-toolkit/setup-tools@v2
  with:
    node: true
    python: 3.12
    
- uses: org/actions-toolkit/deploy-gate@v2
  with:
    environment: production
    reviewers: "@team/ops"
```

## License

MIT