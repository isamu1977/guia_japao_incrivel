## ADDED Requirements

### Requirement: Global Layout
The system SHALL provide a shared layout with header and footer applied to all pages.

#### Scenario: Layout wraps page content
- **WHEN** a localized page is rendered
- **THEN** the shared header and footer are visible around the page content

### Requirement: HTML Language Attribute
The system SHALL set the `<html lang>` attribute to the current locale.

#### Scenario: Lang attribute in PT
- **WHEN** visiting a PT page under `/pt/*`
- **THEN** the HTML root element has `lang="pt"`

#### Scenario: Lang attribute in JA
- **WHEN** visiting a JA page under `/ja/*`
- **THEN** the HTML root element has `lang="ja"`
