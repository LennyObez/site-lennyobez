# Contributing

Thanks for your interest in contributing to lennyobez.com.

This is a personal website built on the Pulsar Framework with the Pulsar CMS extension. The source code is publicly available for reference and learning, but the license does not permit cloning, forking, or redistributing the repository. Contributions are welcome through bug reports, feature suggestions, and security disclosures.

## How to contribute

- **Bug reports**: open an issue using the bug report template
- **Feature suggestions**: open an issue using the feature request template
- **Security vulnerabilities**: report privately via [SECURITY.md](SECURITY.md)

## Coding standards

The following standards apply to all code in the repository. If you're referencing this project for your own Pulsar-based site, these conventions are worth adopting.

### PHP

- Every PHP file must start with `<?php` followed by `declare(strict_types=1);`.
- Prefer explicit dependencies (constructor injection).
- Follow PER-CS2.0 coding style.
- Public APIs must be typed and documented.
- Exceptions must be typed; no silent failures.

### TypeScript / JavaScript

- Prefer TypeScript for all new JS code.
- Typed linting is preferred; avoid `any`.
- Keep Node tooling optional for runtime.

### HTML / UI

- HTML5 semantic markup only.
- Accessibility is mandatory: keyboard support, correct labels and focus behavior, minimal and correct ARIA usage.
- All text-dominant pages must achieve Lighthouse 100/100.

## Commit convention

This project uses [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <imperative summary>
```

**Types:** `feat`, `fix`, `docs`, `perf`, `refactor`, `test`, `ci`, `build`, `chore`, `security`

**Scopes:** `app`, `cms`, `i18n`, `gallery`, `contact`, `rss`, `infra`, `ci`, `docs`

## Security issues

Don't open public issues for vulnerabilities. Report them privately. See [SECURITY.md](SECURITY.md).

Thanks for your interest in lennyobez.com.
