# Security Policy

Thank you for helping keep NSL.SH, Yundera and the people who use them safe.

## Reporting a vulnerability

**Please do not open a public issue for a security problem.** Report it privately, by either:

1. **GitHub private reporting (preferred):** open the repository's **Security** tab and click **Report a vulnerability**.
2. **Email:** contact@yundera.com, with the subject line starting with `[SECURITY]`.

Please include:

- the component and version (or commit) affected
- what an attacker can do, and the conditions needed
- steps to reproduce, or a proof of concept
- any suggested fix, if you have one

You can write in English or French.

## What happens next

| Step | Our target |
| --- | --- |
| We acknowledge your report | within 3 working days |
| We confirm the issue and its severity | within 7 days |
| Fix released, for critical and high severity | within 30 days |
| Fix released, for medium and low severity | in the next regular release |

We keep you informed along the way and agree a disclosure date with you. Once the fix is out, we publish a GitHub security advisory and credit you, unless you prefer to stay anonymous. If no fix is possible within 90 days, we will still disclose the issue together, with the best mitigation available.

## Supported versions

| Component | Receives security fixes |
| --- | --- |
| NSL.SH box template (`mesh-router-template-root`) | the `stable` channel; boxes on automatic updates get fixes with the nightly self-check |
| Maison, Files and other box components | the latest release |
| NSL.SH routing service (gateway, backend, nameserver) | the running service at nsl.sh, patched by us |
| Yundera managed servers | all of them, patched by us without action on your side |

If you disabled automatic updates (`MESH_AUTO_UPDATE=false`), re-run the installer to get a fix.

## Scope

**In scope:** every repository in the [Yundera organization](https://github.com/Yundera), the nsl.sh routing service, and the way our App Store packages and configures apps (for example an app exposed without the login gate, or a default secret shared between boxes).

**Out of scope:**

- vulnerabilities in the apps themselves (Immich, Nextcloud, Jellyfin and others): please report those to their own maintainers. Tell us too if our packaging makes the problem worse.
- denial of service by sheer traffic volume, spam, and social engineering of our team
- reports from automated scanners with no demonstrated impact

## Testing safely

Test only against a box you own, or our demo at demo.nsl.sh. Do not access other users' data, degrade the shared nsl.sh service, or keep any data you come across. If you act in good faith and follow this policy, we will not take legal action against you, and we will treat your research as authorized.
