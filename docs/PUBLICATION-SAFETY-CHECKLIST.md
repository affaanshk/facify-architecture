# Public-release safety checklist

Do not switch this repository to public until the project owner/institution and relevant stakeholders have approved the material being published.

## Before publication

- [ ] Confirm written permission to publish a high-level architecture overview.
- [ ] Confirm whether the institution permits use of the project name and institution name.
- [ ] Confirm whether the patent applicants/stakeholders approve linking the application and describing the project relationship.
- [ ] Review every diagram for confidential implementation details.
- [ ] Review every screenshot manually before upload.
- [ ] Remove student faces, names, IDs, class labels, attendance records and metadata.
- [ ] Remove browser tabs, internal URLs, IP addresses, hostnames, QR codes and notifications.
- [ ] Confirm no credentials, tokens, `.env` files, certificates or private keys are present.
- [ ] Confirm no source code, model weights, private datasets or internal documents are present.
- [ ] Do not add a software license unless the rights holder explicitly authorizes one.

## Safe defaults

- Keep the repository private until approval is obtained.
- Publish only the README and sanitized, conceptual diagrams after approval.
- Do not publish raw screenshots by default; use synthetic/mock UI illustrations if approved.
- Do not publish detailed security architecture, internal endpoints, thresholds, schemas or deployment topology.
- Re-check the repository contents and commit history before changing visibility to public.

## If anything sensitive was accidentally committed

Deleting a file in a later commit does not remove it from Git history. Treat exposed credentials as compromised, rotate/revoke them immediately, and follow the institution's incident-reporting process.
