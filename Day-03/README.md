# Your First Security Audit

**Day 3 of 90 · Understanding the Digital World**

## Objective

Conduct a structured personal security audit to identify gaps between current security and the level of protection desired.

The audit followed five steps:

1. **Scope** — define the systems and accounts being assessed.
2. **Intelligence** — gather information about existing exposure.
3. **Exposure** — review current account-security weaknesses.
4. **Severity** — assess the significance of findings.
5. **Remediation** — take at least one corrective action and document remaining work.

## 1. Scope

The assessment covered:

- **Primary email:** personal Gmail account (address intentionally omitted from this public report).
- **Key accounts:** Google, Apple ID, Instagram, Snapchat, and LinkedIn.
- **Devices:** iPhone and Windows laptop.
- **Network:** personal network (identifier omitted).

## 2. Intelligence gathering

### Have I Been Pwned

- Breaches reported for the primary email: **0**
- Worst breach: **None reported**

### Epieos OSINT check

The email lookup displayed services labelled:

- Google Calendar
- Google Maps
- Archive

These are recorded as tool observations, not proof that an account is currently active or that its contents are publicly accessible.

## 3. Current exposure assessment

### Active sessions

- Unrecognised active sessions reported: **None**

### Two-factor authentication

Across the five key accounts, the initial review found a mixture of:

- SMS-only two-factor authentication.
- Accounts with two-factor authentication disabled.

The exact account-by-account breakdown was not recorded in the notes, so this report does not assign individual statuses.

### Email recovery exposure

- Assessment: **Most accounts may be recoverable through the primary email's “Forgot password” flow.**
- Risk: compromise of the primary email could make other accounts easier to take over.

This is the auditor's reported assessment; individual recovery flows were not documented as tested.

## 4. Severity assessment

The overall self-assessment was **mostly Critical and Medium**.

Key risk themes:

- **Authentication weakness:** some important accounts had no 2FA or relied on SMS-only 2FA.
- **Email as a recovery hub:** access to the primary email could affect many connected accounts.
- **OSINT visibility:** the email lookup associated the address with several services.

No unrecognised sessions were found. Specific severity labels for each individual account or service were not recorded, so they are not invented here.

## 5. Remediation completed

- Enabled **authenticator-app-based 2FA on the primary Gmail account**.
- Recorded password information in physical form. The record must be kept securely and never uploaded to this repository.

## 6. Remediation plan

### Next steps

- Enable strong 2FA on the remaining key accounts where it is missing.
- Replace SMS-only 2FA with an authenticator app or passkey where supported.
- Review account-recovery options and remove recovery methods that are no longer valid.
- Review third-party app access and revoke anything unrecognised or no longer needed.
- Move toward using a reputable password manager and unique passwords for every account.
- Keep any physical password backup secured against unauthorised access.

## Key takeaway

A personal security audit turns vague concerns into specific findings and actions. The most important improvement from this assessment was enabling authenticator-app-based 2FA on the primary Gmail account, which is also a recovery point for many other services.

## Progress checklist

- [x] Defined the audit scope.
- [x] Checked the primary email with Have I Been Pwned.
- [x] Ran an Epieos email OSINT lookup.
- [x] Reviewed active sessions and 2FA coverage.
- [x] Assessed overall severity.
- [x] Enabled authenticator-app-based 2FA on primary Gmail.
- [ ] Complete and securely save the full private audit report.
- [ ] Capture a redacted findings screenshot for the course/LinkedIn task.
- [ ] Strengthen 2FA on the remaining key accounts.

---

**Privacy note:** This public learning log intentionally excludes email addresses, passwords, recovery codes, exact device identifiers, network names, and screenshots containing personal account information.
