# Security follow-up — 19 October 2026

The repository uses the legacy Gatsby 2 / React 16 ecosystem and an existing CircleCI pipeline. Keep its current application behavior while planning a staged supported-stack migration. Renovate automerge is disabled so dependency proposals require review. A modern production build and exhaustive legacy dependency remediation are still pending.

The new baseline scans the current checked-out tree, not historical commits. Do not interpret a green check as proof that historical credentials were revoked. No production deployment or provider credential test was performed.

Repository rulesets, required PR checks, secret scanning/push protection, Dependabot alerts, account 2FA, and token/SSH-key hygiene require verification in GitHub settings. These settings were not mutated by this PR. Apply required checks only after their first verified successful run, so existing deployments are not unexpectedly blocked.
