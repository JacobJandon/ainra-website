<!-- Generated markdown mirror of foundation.html — do not edit; regenerate with `make site` (tools/site-mirrors.mjs). -->
# AINRA — Foundation & status

/01 · REAL TODAY

## Honest status.

THE MARKS ON THIS PAGE

- DONE · SIGNED · WILL NOT CHANGE

- IN FORCE · RUNNING

- PENDING · INVITED · NOT YET SETTLED

- ZERO · NOTHING THERE YET

Each mark is a Game-of-Life pattern running on a 5×5 grid (B3/S23): a still block, a travelling glider, an oscillating blinker, an empty grid.

NOTHING ON THIS SITE IS SIMULATED WITHOUT SAYING SO · NUMBERS ARE MEASURED OR THEY ARE ABSENT

This page states exactly what exists — nothing more. It changes only when reality does. If anything here ever disagrees with reality, that is a bug: tell us.

UPDATED 2026-11-04 · THE NUMBERS BELOW THE REGISTER COME FROM THE PUBLISHED RECORD 2026-11-04 · AGE ·

### STANDARD v5.1 — PUBLIC ✓

The complete normative specification. Read it or take the canonical file.

### REFERENCE CLI v0.3.3 — WORKING ✓

Zero-dependency, real signatures, hash-chained log; catches forged tiers and rewritten history live. Download.

### REFERENCE IMPLEMENTATION PUBLIC · TEN SIGNED RELEASES

The full stack — issuance, transparency log, witness quorum, revocation, verifier SDK — is public with ten signed, board-proven releases — the current one is v0.7.0. A stranger's cold clone passes every gate: the repository.

### GENESIS ROOT MINTED · OPERATOR-RUN

A FROST 5-of-9 + SLH-DSA dual-root exists; the network runs under it and passports verify root-dark, trusting only the root (make genesis-verify). The distributed public ceremony across independent custodians — plus the external verifiers and soak — is the remaining real-world milestone.

### WITNESSES 0 OPERATORS — GAP

This control has no operators, so the guarantee it provides is not in force today. Witness cosignatures are what would stop the root showing one history to one party and a different one to another. The machinery is built, rehearsed and drilled on every board — an injected fork is refused by a quorum — but a quorum of zero certifies nothing, so for now you are trusting us not to equivocate rather than being able to check. Being the first takes one command: bash kits/witness/be-a-witness.sh. Take the seat.

### EXTERNAL VERIFIERS INVITED

The drop-in verifier kit and the self-serve conformance programme are published; third parties verify — and attest — on their own infrastructure. Attestations so far: 0 of the 3 needed. Want a seat? Join the founding table.

### CONFORMANCE 1169/1169 ✓

Three implementations — Rust, TypeScript and Python — agree on all 1169 CC0 conformance vectors, byte-for-byte, on verdict and reason; a fourth, the reference CLI, agrees on canonical encoding. Reproduced with one command (make diff) in the reference repository; the vector corpus is published alongside it.

### REVOCATION <60s [MEASURED]

Revocation propagation measured under 60 seconds, fail-closed, in networked drills of the reference stack (make soak-smoke). The 14-day multi-region soak runs at genesis.

registrars—

passports issued—

revoked—

checkpoint height—

PRODUCTION LOGS SEALED—UNTIL GENESIS

STAGING NETWORK · TEST-ROOT · published record

RECORD PUBLISHED —

The same read contract AINRAscan and any mirror use — a staging TEST-ROOT, not production. Point it at a network you run with ?net=<url> and these numbers go live. Production logs sealed: 0 until genesis.

The contract at — did not answer, so
nothing above is live right now. Everything else on this site still proves what it proves — the verifier, the
vectors and the signatures are checked on your machine, not on ours. To run the network yourself:
make stage-install (or make genesis-local for a one-shot local world).

/02

## The organization.

A member-governed, non-profit federation — neutral ground where competing issuers become one system without becoming one company. Legitimacy flows from members; the federation never competes with them.

Members

### Every seat is a class.

Issuers, attestors, verifiers, resolution & data providers, witnesses, and public-interest members — each class a constituency in the assembly, which elects the board under charter constraints.

Separation

### Keys and logs stand apart.

Custodians (who hold key shares) and witnesses (who cosign the log) are structurally separate from board and assembly alike. No single person or institution can act alone.

Transparency

### Everything material is public.

Statutes, minutes, budgets, audits, fee schedules, and ceremonies. The root records facts — never money, personal data, reputation, or judgment.

AINRA is a proposal for that neutral root — one open standard anyone can run, own, or fork. You are not asked to trust its founders; everything is public.

/03

## Genesis: how the root is born.

The production root does not exist until it is born in public — on camera, across independent custodians, with no single point of trust. Until then, everything runs on a labeled TEST-ROOT and says so.

-

### The ceremony, rehearsed
A FROST 5-of-9 threshold ceremony — any five of nine custodians can act together, no one alone, four compromised shares are useless. Rehearsed end-to-end across nine isolated processes with a reproducible transcript; an independent checker re-verifies every custodian.DONE · REPRODUCIBLEmake ceremony-rehearsal-multi · runbook: docs/genesis-day/RUNBOOK.md

-

### The recorded public ceremony
Ceremony day is scripted from T−30 days to T+14: sealed hardware shown on camera, air-gapped ephemeral machines, shares generated that never leave them, commitments cross-read aloud. Any failed check aborts the day — publicly.PENDING · REAL-WORLD EVENTgo/no-go checklist · abort playbook · cutover plan — all published in the repo

-

### Independent verifiers
Three or more unaffiliated people each receive a fresh challenge no one can precompute, verify it on their own machines with the published tooling, and sign what they saw. Their attestations become permanent public evidence.RECRUITING · ≥3 STRANGERSchallenge kits minted · outreach ready · the ask is ~10 minutes

-

### The soak
Fourteen days of measured revocation propagation across three regions, each region writing signed reports. The founding declaration refuses to render unless every claim resolves to real evidence.PENDING · 14 DAYS · 3 REGIONSplatform built and smoke-proven · the clock is the operator's button

Honesty rule: these three rows are real-world events, not code. Nothing on this site counts them done before they happen — production logs sealed today: 0.

/04

## Economics: position, not profit.

Revenue is capped per-lineage-year fees at cents scale, flat accreditation, and grants. Verification is free forever — the design goal is a root cheap enough that removing it costs more than keeping it. At scale, the charter's falling cap reduces the fee toward archival cost.

/05

## The road, planned to the end.

- NOW

### Prove
External verifier trials against pre-registered gates; the standard filed in the open with the reference stack as its conformance suite. Three implementations already agree on all 1169 vectors on verdict and reason, and a fourth agrees on canonical encoding; a stranger can clone the repo and every gate passes.

- NEXT

### Anchor
Institutional co-conveners; charter ratification; the first public ceremony sealing log #1; two registrar classes issuing live; one revocation propagated worldwide, watchably.

- THE LONG MIDDLE

### Endure
Adoption plateaus and pressure met with pre-decided responses. Principles fixed, pace flexible.

- THE GOAL

### Disappear
Disappear means become unnecessary, not vanish. The goal isn't an ecosystem that depends on us; it's one that no longer needs us — a relay race, not a solo marathon. From outside it looks like verification as boring as the clock. Beyond that: generational key-succession ceremonies, fork-readiness drills, and a managed-migration clause — if a legitimately adopted successor emerges, the root's final duty is an orderly migration into it. The standard outlives whoever carries it; that is planned, not feared.

Take a founding seat →
What exists today

/06 · INTERNET FREEDOM

## Proof for the people under pressure — without being watched.

Newsrooms, human-rights groups and activists face impersonation and surveillance first. AINRA gives them certainty about the software they deal with, and the check itself tells no one anything.

/01

### A real tool, not a decoy.

Check that an agent belongs to the organisation it names, and not to an impersonator or a spoofed bot: the passport carries its operator, proven to an accredited registrar.

/02

### A check that calls no one.

Signatures and revocation are checked on the verifier’s own machine, from public files. No request goes to us or anyone during a check, so there is no log of who checked whom.

/03

### A seized key, switched off.

If a device or an agent’s key is taken, one bit set in the signed status list (an IETF Token Status List) makes every verifier that checks refuse it — within its freshness class: 30 seconds at F1, five minutes by default.

/04

### No single owner, two signatures.

Every passport is signed twice, Ed25519 and ML-DSA-65, so it holds even if one scheme falls — including to a future quantum computer. The root is built to be held 5-of-9 by independent custodians; today it is pre-ceremony, with no witnesses yet.

/07

## Take a founding seat.

Join now and you help write the rules everyone inherits — you get the standard, the founding brief, and a direct line.

IssuerLicense & issue passports
VerifierGate decisions on the record
AttestorProve identity claims
WitnessCosign the public log
BuilderRun agents that carry passports
OtherSomething else entirely

Pick your seat, then open your founding request.

Take a seat →

Opens a public founding request on the source repository — in the open, like everything else here; nothing is stored on any server we run.

READ THE STANDARD FIRST →

/08 · RELEASE INTEGRITY

## Verify what you download.

Every release is signed, and — the stronger check — reproducible: you rebuild the conformance corpus byte-for-byte from the tagged source and trust the bytes, not us.

### Signing key

SHA256:V1ZbCNdPDEe5plpYq07dGCsoensF4Q+MPPQQkcj5pi4

SSH Ed25519 · public key pinned in-repo (release/ainra-release.pub) · private key offline.

### How to verify

Check the signature, then rebuild from source (make repro) and diff the manifest — no key needed for the strong proof.

The full guide — RELEASE-VERIFY.md →
