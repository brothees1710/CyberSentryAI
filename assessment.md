# CyberSentryAI — Security Assessment Report

Generated (UTC): 2026-11-11 02:55

## Scope and method
Reviewed 300 exported Windows Security event records (maximum 300).
Offline RULE-BASED analysis because the UTSA VPN/Qwen connection was unavailable.
No AI model was queried. These labels are preliminary and require human verification.

## Classification summary
- BENIGN: 285
- SUSPICIOUS: 15
- MALICIOUS: 0

## Observed event categories (event IDs only)
- Windows Event ID 4798: 136 record(s)
- Windows Event ID 5379: 126 record(s)
- Windows Event ID 4624: 15 record(s)
- Windows Event ID 4672: 13 record(s)
- Windows Event ID 4634: 4 record(s)
- Windows Event ID 4799: 2 record(s)
- Windows Event ID 4648: 2 record(s)
- Windows Event ID 4738: 2 record(s)

## Findings requiring manual review
- SUSPICIOUS / Event ID 4672 (13): Special privileges assigned; check account and session context.
- SUSPICIOUS / Event ID 4648 (2): Explicit credentials were used; verify this was expected.

## Recommendations
1. Confirm the context of flagged event IDs in the original Event Viewer log.
2. Investigate repeated authentication failures and unexpected account/privilege changes.
3. Correlate with endpoint logs and the relevant system owner before declaring an attack.
4. Re-run the assignment's Qwen model workflow after VPN access is restored.

## Limitations and privacy
This output is from deterministic triage rules, not UTSA Qwen Coder. Event IDs alone do not prove malicious activity.
Raw logs were deliberately excluded from this report; do not publish the original CSV.
