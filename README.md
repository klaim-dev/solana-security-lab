# solana-security-lab

Solana vulnerabilities: vulnerable/fixed pairs with exploit tests + audit reports.

**Stack:** Rust · Anchor · TypeScript · Security reports

**Status:** work in progress - updated daily.

## Goal

Create a hands-on Solana security lab with intentionally vulnerable programs, exploit tests, fixed implementations, and concise audit-style reports.

This repository is designed to show security judgment, not just syntax. Each module should explain the bug, demonstrate the exploit, apply the fix, and document the invariant that prevents regression.

## Planned Vulnerability Tracks

- Missing signer checks
- Incorrect account owner validation
- PDA seed confusion
- Wrong token mint validation
- Token account authority mistakes
- Unsafe account close flows
- Arithmetic and reward accounting bugs
- CPI trust boundary mistakes

## Layout

```text
vulnerable/  Broken examples
fixed/       Corrected versions
tests/       Exploit and regression tests
reports/     Short audit notes and findings
```

## Report Format

Each issue should include:

- Impact
- Root cause
- Exploit path
- Fix
- Regression test

## Local Development

```bash
anchor build
anchor test
```

## Keywords

Solana, Anchor, Rust, smart contract security, audit, exploit tests, DeFi security, PDA, SPL Token.
