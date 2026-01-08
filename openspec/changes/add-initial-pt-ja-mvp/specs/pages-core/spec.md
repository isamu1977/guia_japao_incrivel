## ADDED Requirements

### Requirement: Home Page (PT and JA)
The system SHALL provide a localized Home page in PT and JA with a headline and call-to-action.

#### Scenario: Home page PT
- **WHEN** a user visits `/pt/`
- **THEN** a localized Home page in Portuguese is rendered with headline and CTA

#### Scenario: Home page JA
- **WHEN** a user visits `/ja/`
- **THEN** a localized Home page in Japanese is rendered with headline and CTA

### Requirement: Contact Page (PT and JA)
The system SHALL provide a localized Contact page in PT and JA including a contact method link.

#### Scenario: Contact page PT
- **WHEN** a user visits `/pt/contato`
- **THEN** a localized Contact page in Portuguese is rendered with a working `mailto:` link

#### Scenario: Contact page JA
- **WHEN** a user visits `/ja/contact`
- **THEN** a localized Contact page in Japanese is rendered with a working `mailto:` link
