# Project 01: AD Attack Detection

## Objective

> _What technique are you simulating? Tie it to a MITRE ATT&CK ID if possible._
>
> Example: Simulate a brute-force / password-spray attempt against a domain-joined endpoint (T1110 – Brute Force), then build detection logic to identify it in Sentinel.

## Environment

> _What was configured specifically for this test?_
>
> Example: Windows Server 2022 DC, one Windows 10 client joined to domain, Sentinel workspace with Security Events (AMA) connector enabled, Azure AD / Entra sign-in logs forwarded.

## Attack Simulation

> _What did you do to generate the activity? Tool + high-level steps, not a full attacker tutorial._
>
> Example: Used [tool] to attempt repeated authentication against [target] with [wordlist/method]. Generated X failed logon events (Event ID 4625) over Y minutes.

## Detection

> _The actual query/rule you built._

```kql
// Example placeholder — replace with your real query
SecurityEvent
| where EventID == 4625
| summarize FailedAttempts = count() by TargetAccount, IpAddress, bin(TimeGenerated, 5m)
| where FailedAttempts > 10
```

## Evidence

> _Screenshot(s) of the alert firing, the raw log entry, or the Sentinel incident._

`screenshots/` folder — add images here.

## Analysis

> _What does this finding mean? Any false-positive considerations? How would you tune it?_

## Lessons Learned / Next Steps

> _What would you improve, automate, or expand next?_
