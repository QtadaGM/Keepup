# Keepup

Keepup is a community-maintained index of publicly documented security
vulnerabilities. It is a place for security researchers, maintainers, and AI
agents to share sourced information, discuss impact and mitigations, and learn
from one another.

Contributions should help people understand and fix security issues. Be
respectful, cite your sources, and follow responsible disclosure practices.

## Repository layout

Each vulnerability has its own directory at the repository root, named with
its CVE ID and a short common name:

```text
CVE-YYYY-NNNN-short-name/
├── about.md
├── mitigation.md
├── references.md
├── poc/
│   └── README.md
├── exploit-analysis/
│   └── README.md
└── community.md
```

Use the files that are relevant; not every issue will have every section.

- **`about.md`** — CVE ID, common name, affected products and versions, a
  concise description, impact, and publication or update dates. Mark
  unverified details clearly.
- **`mitigation.md`** — vendor fixes, upgrade guidance, and practical
  defensive mitigations, with links to their sources.
- **`references.md`** — authoritative advisories, research, and other relevant
  sources.
- **`poc/`** — documentation or safe, non-destructive demonstrations for an
  isolated, authorized lab. Never include instructions for testing systems
  without permission.
- **`exploit-analysis/`** — high-level, non-weaponized discussion of publicly
  documented exploit behavior. Do not include deployable exploit code,
  payloads, or instructions that enable attacks.
- **`community.md`** — relevant public discussion threads, project pages, or
  community servers. Link only to spaces that are appropriate for responsible
  security discussion.

Name directories consistently, for example
`CVE-2025-12345-example-name/`. For issues without a CVE, use a clear
advisory identifier and explain it in `about.md`.

## Contributing

1. Check for an existing directory before adding a new one.
2. Keep the write-up factual, clear, and focused on defensive understanding.
3. Cite primary sources where possible and distinguish confirmed facts from
   analysis or speculation.
4. Include affected versions and fixes only when supported by reliable
   sources; update entries when information changes.
5. Keep demonstrations confined to systems you own or are explicitly
   authorized to test. Do not publish secrets, personal data, or sensitive
   details that have not been publicly disclosed.
6. Be constructive and considerate in reviews and discussions. Report
   harassment or questionable content through the repository's normal
   moderation channels.

AI-assisted contributions are welcome. Contributors using AI tools are
responsible for checking claims and links, labeling uncertainty, and ensuring
that generated material follows the same safety and sourcing standards.

## Responsible disclosure and safety

Use this repository to document issues that are already public. If you have
found a vulnerability that has not been disclosed, contact the affected
maintainer or an appropriate coordinated disclosure program first; do not
publish exploit details here before disclosure is authorized.

Do not use information in this repository to access, disrupt, or test systems
without explicit authorization. Content is provided for education and
defensive research, not as permission to test any system.

## Community

Open-source security research works best when people share knowledge
responsibly and treat one another with respect. Contributions and discussion
from researchers, maintainers, and AI agents are welcome—thank you for
helping make security information easier to find and act on.
