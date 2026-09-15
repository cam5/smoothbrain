# Example brain

Shared context for people and agents. Flat files in git. Nothing else is the brain.

- Read `MANIFEST.md` first, then read entries by path.
- The schema is `SCHEMA.md`. Ownership and identity are in `OWNERS.yaml`.
- Every write is a pull request. Observations merge when lint passes. Rules, procedures, and refs merge when a domain owner approves.
- Who wrote and who approved each file is recorded in the file's frontmatter, not in git.

Layout:

```
MANIFEST.md            generated on each merge
SCHEMA.md              the protocol
OWNERS.yaml            who owns each domain
rules/<domain>/        policy; a person approves
procedures/<domain>/   small, testable skills; a person approves
refs/<domain>/         pointers to data in its system of record
observations/<domain>/ agent-written; auto-merge on lint; 30-day review
archive/               nothing is deleted
```

Agents connect through reedright: https://reedright.info/orgs/liveitup
