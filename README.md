# lennyobez.com

The personal website for Lenny Obez, unifying three identities (developer, photographer, explorer) under a single multilingual domain. The site serves as the canonical online destination for anyone searching "Lenny Obez," replacing a fragmented presence across multiple platforms with a cohesive, professional experience. It is built on the Pulsar Framework and powered by the Pulsar CMS extension.

## What this is

- A personal brand website, not a framework or library
- A real-world showcase of the Pulsar Framework and its CMS extension in production
- A multilingual site serving four languages: English, French, Dutch, and German

## Sections

| Section | Purpose |
|---------|---------|
| Landing | Three-column hub linking to Development, Photography, and Explore |
| Development | Developer portfolio, projects, services, tech stack, open source, uses |
| Photography | Photo gallery, services, behind the scenes |
| Explore | Urban exploration and off-road stories, gear, locations |
| Blog | Technical articles on Pulsar, PHP, and development topics |
| About | Personal bio, background, and /now page |
| Contact | Unified contact form for all audiences |
| Resume | Online CV with downloadable PDF |
| Colophon | How this site was built (Pulsar showcase) |
| Legal | Privacy policy and terms of use (all four languages) |

## Tech stack

- **Framework**: Pulsar Framework (PHP 8.5+)
- **CMS**: Pulsar CMS extension
- **Database**: MariaDB
- **Templating**: Pulsar templates (`.pulsar.php`)
- **i18n**: Pulsar i18n (domain-based catalogs, ICU MessageFormat)
- **Frontend**: Pulsar Design System, CSS custom properties, vanilla JS
- **Hosting**: AWS (Route 53, CloudFront, EC2)
- **Server**: Nginx + PHP-FPM
- **CI/CD**: GitHub Actions

## Project structure

```
lennyobez.com/
├── app/
│   └── Modules/
│       ├── Landing/
│       ├── Development/
│       ├── Photography/
│       ├── Explore/
│       ├── Blog/
│       ├── About/
│       ├── Contact/
│       ├── Resume/
│       ├── Colophon/
│       ├── Legal/
│       └── Shared/
│           ├── Middleware/
│           └── ViewModel/
├── extensions/
│   ├── ext-cms-website/
│   ├── ext-gallery/
│   ├── ext-contact/
│   └── ext-rss/
├── public/
│   ├── index.php
│   ├── assets/
│   └── photos/
├── resources/
│   ├── lang/
│   │   ├── en/
│   │   ├── fr/
│   │   ├── nl/
│   │   └── de/
│   └── views/
│       ├── layouts/
│       ├── components/
│       └── {section}/
├── config/
├── database/
│   └── migrations/
├── storage/
└── tests/
```

## Client extensions

| Extension | Purpose |
|-----------|---------|
| ext-cms-website | Site-specific CMS content types (Project, GallerySet, Article, Service), view templates, seeders |
| ext-gallery | Photo gallery with masonry grid, lightbox, filtering, EXIF display, responsive image generation |
| ext-contact | Contact form definition via Pulsar Form extension, SMTP delivery via Pulsar mail transport |
| ext-rss | RSS/Atom feed generation from CMS content |

## Internationalization

The site supports four languages: English, French, Dutch, and German. This covers international reach plus Belgium's three official languages. All content is stored with per-locale fields in the CMS, and translations use domain-based catalogs with ICU MessageFormat through Pulsar's built-in i18n system.

## Contributing

Bug reports, feature suggestions, and security disclosures are welcome. See [CONTRIBUTING.md](.github/CONTRIBUTING.md).

## Security

If you find a vulnerability, please report it privately. See [SECURITY.md](.github/SECURITY.md).

## License

This project uses a source-available license that allows personal and educational use while restricting commercial use and redistribution. See [LICENSE](LICENSE) for the full terms.
