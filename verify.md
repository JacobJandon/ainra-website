<!-- Generated markdown mirror of verify.html — do not edit; regenerate with `make site` (tools/site-mirrors.mjs). -->
# AINRA — Verify

For verifiers & builders

# Check theirs.Trust the source, not us.

One half of the loop — prove yours is the other. The check runs on your machine; nothing reaches us.

Every check runs locally, from public artifacts, in milliseconds — offline-capable, with the root dark. Verification never reports to anyone.

1 · PRESENT

The agent's request arrives signed; the signature names its passport key.

→

2 · CHECK THE CHAIN

Passport → registrar → root, plus the authority chain to its anchor. Cached keys, milliseconds.

→

3 · CHECK STATUS

Fresh revocation proof and witness-cosigned log inclusion. In good standing, right now.

→

4 · DECIDE

Your policy: tier floor, accepted authority classes, required scopes, fail-open or closed.

PROPOSED VERIFICATION PROFILE — NOT YET IN THE STANDARD (v5.1 defines proof freshness only for L3–L4)

### F1 PAYMENTS-GRADE

Requires a signed fresh status head no older than 30 seconds. Missing or stale? The check fails closed.

### F2 STANDARD

Status list no older than five minutes, with signed deltas applied. Stale? Fails closed.

### F3 OFFLINE

Air-gapped verification against a cached list up to 24 hours old — still cryptographically complete, still fail-closed.

REAL TODAY — THE REFERENCE CLI

A zero-dependency command-line tool with real signatures and a hash-chained local log. It issues, verifies, and revokes — and it catches tampering live: a forged tier and a rewritten log line are both rejected with the exact reason. Download v0.3.0 and try to break it.

→

AT FIRST PUBLIC RELEASE — AHEAD

The full reference implementation: verify in five lines with the SDK, a fail-closed middleware gate, registrar-in-a-box in one command, and the complete conformance vector set — published under CC0, so conformance never needs anyone's permission.

VERIFICATION IS LOCAL · IT NEVER PHONES HOME · CONFORMANCE IS CLAIMED AGAINST THE VECTOR SET THAT SHIPS AT FIRST PUBLIC RELEASE, NOT GRANTED BY US
