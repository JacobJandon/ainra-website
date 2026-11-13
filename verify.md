<!-- Generated markdown mirror of verify.html — do not edit; regenerate with `make site` (tools/site-mirrors.mjs). -->
# AINRA — Verify

For verifiers & builders

## Check theirs.Trust the source, not us.

One half of the loop — prove yours is the other. The check runs on your machine; nothing reaches us.

Every check runs locally, from public artifacts, in milliseconds — offline-capable, with the root dark. Verification never reports to anyone.

- 1 · PRESENTThe agent's request arrives signed; the signature names its passport key.

- 2 · CHECK THE CHAINPassport → registrar → root, plus the authority chain to its anchor. Cached keys, milliseconds.

- 3 · CHECK STATUSFresh revocation proof and inclusion in the registrar's signed log. In good standing, right now.

- 4 · DECIDEYour policy: tier floor, accepted authority classes, required scopes, fail-open or closed.

PROPOSED VERIFICATION PROFILE — NOT YET IN THE STANDARD (v5.1 defines proof freshness only for L3–L4)

### F1 PAYMENTS-GRADE
PROPOSED

Requires a signed fresh status head no older than 30 seconds. Missing or stale? The check fails closed.

### F2 STANDARD
PROPOSED

Status list no older than five minutes, with signed deltas applied. Stale? Fails closed.

### F3 OFFLINE
PROPOSED

Air-gapped verification against a cached list up to 24 hours old — still cryptographically complete, still fail-closed.

- REAL TODAY — THE REFERENCE CLIA zero-dependency command-line tool with real signatures and a hash-chained local log. It issues, verifies and revokes — and it catches tampering live: a forged tier and a rewritten log line are both rejected with the exact reason. Download v0.3.5 and try to break it.

- REAL TODAY — THE FULL IMPLEMENTATIONVerify in five lines with the SDK (@ainra/sdk on npm, ainra on PyPI), a fail-closed middleware gate, registrar-in-a-box in one command, and the complete conformance vector set — published under CC0, so conformance never needs anyone's permission.

VERIFICATION IS LOCAL · IT NEVER PHONES HOME · CONFORMANCE IS CLAIMED AGAINST THE PUBLIC VECTOR SET, NOT GRANTED BY US

/01 · Try it — 20 seconds, in this tab

## Verify an agent.Then try to forge one.

THE PICKER BELOW HOLDS THE PUBLISHED RECORD · 80 PASSPORTS · 53 REVOKED · 2 REGISTRARS · source: net/registry.json

The actual AINRA verifier — the same code that passes every conformance vector — runs in your browser. It checks passports and, when one is present, the short-lived credential a running copy carries (the instance path). Pick a real passport, then tamper with it and watch it fail closed with a named reason. Nothing is uploaded; the root is never contacted.

### The passport
STAGING · TEST-ROOT

Choose a live lineage

Verify in my browser
↺ Reset (undo forgery)

Use your own bundle, or verify as a named service

### Or paste your own bundle

A conformance vector, a {anchors, presentation} pair, or a bare presentation (checked against the registrar selected above). It is read in this tab and nothing is sent anywhere.

Bundle JSON

Verify what I pasted
Back to the picker

This verifier's audience

A holder-bound instance credential (ADR-019) names the one service it may be presented to. Type
that service's identifier here to verify as it; leave it blank and any such credential is refused —
a verifier that has not said who it is cannot be the audience of anything.

### The verdict
RUNS ON YOUR MACHINE

—

choose a passport, then press Verify

FIG. 01 — THE CHAIN, AS THIS CHECK WENTFROM THE VERIFIER ABOVE

STATUS LIST · bits 0–15 of the selected passport's registrar list

source: net/registry.json · each box follows the checklist the verifier writes above; nothing here runs a check of its own

Forge it — flip one field, then re-verify

Escalate the tierrewrite the signed body → sig_invalid
Break the signaturecorrupt one byte → sig_invalid
Replay an old statusbackdate the revocation list → stale_status
Forge the log proofbad inclusion proof → not_logged

This runs the verifier in your browser and needs JavaScript. A separate reference CLI, which runs with just node, is also downloadable — get it above. It is a simpler implementation, not this verifier.

/02 · The authority model

## Who stands behind it —declared, provable, honest.

Every passport names its authority class. Delegation can only narrow, chains stay provable to their anchor at any depth — and even a fully autonomous agent gets a truthful class of its own. Select one:

A1 HUMAN
A2 ORGANIZATION
A3 AGENT-DELEGATED
A4 AUTONOMOUS

A1 · HUMAN-DELEGATED

A verified person stands behind the agent — checked by the registrar, which keeps the evidence; the root and every verifier see only a digest, so accountability exists while the person stays private. A signed consent mandate sets scopes, time limits, and spend ceilings; the person can revoke it at any moment, everywhere at once.

act_chain: [principal → agent:orchestrator@3 → agent:invoicing@4.2.1] // scopes may only narrow — provable to the anchor at any depth

/03 · A universal standard for current players

## Keep what you built.Gain everyone else.

The standard belongs to no vendor. Every existing layer keeps its product and its customers — and plugs in where it already looks things up.

KEEP
PLUG IN
GAIN

### Payment networks

KEEPTheir agent programs, tokens, and checkout flows.

PLUG INKey-directory lookups resolve through the root.

GAINCross-network recognition and an instant, shared switch.

### Edge & bot defense

KEEPSignature checks and traffic policy at the edge.

PLUG INMirror the root directory behind existing checks.

GAINOperator, tier, and live status behind every signature — a welcome lane for good agents.

### Enterprise identity

KEEPInternal agent directories, ownership, and audit.

PLUG INMint a passport the moment an agent crosses the boundary.

GAINTrust that survives outside the walls, with the chain of authority intact.

### Merchants, apps & APIs

KEEPTheir whole stack, unchanged.

PLUG INOne verify middleware plus a tier floor of your choosing.

GAINWelcome good agents and price risk by tier and authority class.

/04 · Assurance tiers

## Five levels. You set the floor.

The root grades how much verification stands behind a passport; every verifier picks its own floor. Existence at L0 is guaranteed by charter, and each level up earns more consequence.

L0 DECLARED
L1 ANCHORED
L2 OPERATED
L3 BACKED
L4 REGULATED

L3 · BACKED

KYB-verified operator + a checked principal proof + liability insurance attestation. The floor for consumer-scale payments and contract execution.

## Prove yours.

A real registrar, a real transparency log, and real verdicts computed on your own machine from the log's own inclusion proofs.

Network

## Run it yourself

terminalCOPY

$ ainra init ./reg registrar-07
$ ainra issue ./reg --operator acme --lineage invoicing --version 1.0.0 --tier L2 --cap read:data
$ ainra verify ./reg ainra:registrar-07:acme:invoicing@1.0.0
VALID

These commands are for the Rust ainra: in a checkout, cargo build --release -p ainra-cli-rs puts it at ./target/release/ainra. The zip above is the Node reference CLI, and its commands differ.

The CLI lifecycle
