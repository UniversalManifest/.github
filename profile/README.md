<div align="center">
  <img src="https://raw.githubusercontent.com/UniversalManifest/.github/main/profile/assets/um-color-logo-500.png" alt="Universal Manifest logo" width="200">
</div>

<h1 align="center">Universal Manifest</h1>

<p align="center">A portable, signed context envelope for systems that don't share a backend.</p>

---

## The problem

Most trust on a network is brokered by something both sides already share. Two parties can rely on each other because they authenticate against the same service, resolve against the same directory, or sit behind the same operator.

That assumption breaks the moment there is no shared backend. A person arrives at a venue. A client connects to a service it has never seen. One device meets another. Each side needs to know who it is dealing with, what it is permitted to do, and what was consented to — and there is no common server to ask.

## What Universal Manifest is

Universal Manifest is a JSON-LD document format that lets two parties exchange verified identity, trust, consent, and capability information in a single handshake.

Each side presents a manifest. Each side evaluates what the other presented. Each side produces a receipt: a machine-readable record of what it checked, what it accepted, and what it could not read. The document carries its own proof, so the exchange stands on its own. No central server is required.

## Repositories

- **[universal-manifest](https://github.com/UniversalManifest/universal-manifest)** — the specification itself: the manifest document format, the evaluation model a conforming implementation follows, the signature and identity-binding profiles, and the receipt structure. It also holds the conformance suite and the reference runner. Start here, and open specification issues here. The latest release is [v0.5.0](https://github.com/UniversalManifest/universal-manifest/releases/tag/v0.5.0).
- **[use-cases](https://github.com/UniversalManifest/use-cases)** — applied write-ups and figures that walk the format through concrete scenarios, such as permissions and handshaking between two parties. It shows the specification in use rather than restating it.

Both repositories are mirrored, with identical commits, at [oma3dao/universal-manifest-spec](https://github.com/oma3dao/universal-manifest-spec) and [oma3dao/universal-manifest-use-cases](https://github.com/oma3dao/universal-manifest-use-cases).

## Standards composition

Universal Manifest is built to compose with existing work rather than replace it.

- **JSON-LD** — a manifest is a JSON-LD document, so the terms it carries have unambiguous meaning across parties.
- **Decentralized Identifiers (DIDs)** — identity is expressed with DIDs, so a subject is resolvable without a shared account system.
- **Verifiable Credentials** — credential-shaped claims travel inside a manifest and are verified on their own terms.
- **JSON Canonicalization Scheme (RFC 8785)** — provides the deterministic serialization that signatures are computed over.

The specification follows W3C document conventions. Earlier versions were reviewed in the OMA3 Technical Working Group, and publication asserts no OMA3 ratification.

## Authorship and provenance

Universal Manifest was created by **Grig Bilham** of **[Sumset Tech LLC](https://sumset.tech)**, who serves as project lead, inventor, and editor.

The specification was authored as independent work. Its maintainers accept changes through issues and pull requests on the specification repository. Contributions from others are credited by name in the specification's attribution record.

## Licensing

- **Specification v0.5 and later, and all code and tooling:** the Apache License, Version 2.0.
- **Earlier published versions, v0.1 to v0.4:** each keeps the notices and terms it carried when published.

The full licence texts are in the specification repository.

## Security

Report suspected vulnerabilities privately to **security@universalmanifest.net**. Please do not disclose a suspected vulnerability in a public issue.

---

<p align="center"><a href="https://universalmanifest.net">universalmanifest.net</a></p>
