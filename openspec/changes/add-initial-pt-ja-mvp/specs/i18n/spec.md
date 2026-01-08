## ADDED Requirements

### Requirement: Locale Routing
The system SHALL serve localized pages at path prefixes `/pt/` and `/ja/`.

#### Scenario: PT localized path
- **WHEN** a user visits a path under `/pt/`
- **THEN** the PT (Portuguese) localized page content is rendered

#### Scenario: JA localized path
- **WHEN** a user visits a path under `/ja/`
- **THEN** the JA (Japanese) localized page content is rendered

### Requirement: Root Redirect to PT
The system SHALL redirect the root path `/` to the Portuguese locale path `/pt/`.

#### Scenario: Root redirects to PT
- **WHEN** a user visits `/`
- **THEN** they are redirected to `/pt/`

### Requirement: Language Switcher
The system SHALL provide a language switcher that links to the equivalent path in the other locale.

#### Scenario: Switch equivalent route
- **WHEN** a user clicks the language switcher on a localized page
- **THEN** they navigate to the same page path under the other locale prefix
