## ADDED Requirements

### Requirement: Localized Metadata
The system SHALL provide per-locale `<title>` and `<meta name="description">` for all localized pages.

#### Scenario: Metadata PT
- **WHEN** a PT page is rendered
- **THEN** the page has a localized `<title>` and description in Portuguese

#### Scenario: Metadata JA
- **WHEN** a JA page is rendered
- **THEN** the page has a localized `<title>` and description in Japanese

### Requirement: Robots and Sitemap
The system SHALL provide `robots.txt` and `sitemap.xml` that include both locale paths.

#### Scenario: Robots present
- **WHEN** the site is built
- **THEN** a `robots.txt` is available under the site root

#### Scenario: Sitemap includes locales
- **WHEN** the site is built
- **THEN** a `sitemap.xml` is available that lists PT and JA page URLs

### Requirement: Hreflang Alternates
The system SHALL include minimal `rel="alternate" hreflang` links for `pt`, `ja`, and `x-default` on localized pages.

#### Scenario: Hreflang alternates present
- **WHEN** a localized page is rendered
- **THEN** the document head includes `link[rel="alternate"][hreflang="pt"]`, `link[rel="alternate"][hreflang="ja"]`, and `link[rel="alternate"][hreflang="x-default"]` with correct URLs
