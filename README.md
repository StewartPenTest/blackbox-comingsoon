# Blackbox Auditor Marketing Site

Static marketing site for [blackboxauditor.com](https://blackboxauditor.com) - an AWS audit evidence tool for auditors and GRC teams.

## Site Structure

```
├── index.html                 # Homepage
├── css/styles.css             # Shared stylesheet
├── product/                   # Product pages
│   ├── aws-iam-audit-evidence.html
│   ├── aws-sso-federated-access-audit.html
│   ├── aws-cross-account-role-trust-audit.html
│   └── aws-external-boundary-scope-audit.html
├── compare/
│   └── manual-vs-blackbox-auditor.html
├── resources/
│   └── sample-reports.html    # Placeholder
├── company/
│   └── contact.html           # Contact form (Formspree)
└── CNAME                      # Domain configuration
```

## Tech Stack

- Pure HTML/CSS (no build tools required)
- Google Fonts (Inter)
- Formspree for contact form handling
- Logo hosted on AWS S3

## Deployment

Static site - deploy directly to GitHub Pages, Netlify, or any static host.

## Contact Form

Uses Formspree. Form ID is configured in `company/contact.html`.

## Adding Sample Reports

When ready, add PDF/image links to `resources/sample-reports.html`.
