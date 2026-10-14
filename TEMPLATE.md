# <Box Name>

| Field | Value |
| --- | --- |
| Source | VulnHub / HTB / other |
| Difficulty | Easy / Medium / Hard |
| Target IP | 10.10.50.x |
| Attacker IP | 10.10.50.100 |
| Date | YYYY-MM-DD |
| Result | Not started / User / Root |

## Executive summary

Two or three sentences in plain language: what the box was, how it was compromised at a high level, and the single most important lesson. Written so someone who will never read the technical detail still understands the risk.

## Flags

| Flag | Location | Value |
| --- | --- | --- |
| local / user | | |
| root / proof | | |

## Tooling

List the main tools used (nmap, gobuster, etc.). Keep it short.

## Enumeration

### Host discovery

How the live target was found on the lab network.

```
# command
# output
```

### Port and service scan

```
# nmap command
# relevant open ports and versions
```

Summary of what is listening and what each service suggests is worth looking at.

### Service enumeration

For each interesting service, what was found. Web roots, directories, versions, shares, users, anything that feeds the next step.

```
# commands and output
```

## Initial foothold

### Vulnerability

Name the weakness and explain in one or two sentences *why* it exists and why it is exploitable.

### Exploitation

Step by step, with the exact commands and output. Enough that the box could be redone from this section alone.

```
# commands and output
```

### Proof of access

Evidence of the first shell: `id`, `hostname`, `ip addr`, and the local flag.

```
# output
```

## Privilege escalation

### Enumeration

What was checked on the box (SUID binaries, sudo rights, cron, kernel, configs, credentials) and what stood out.

```
# commands and output
```

### Vulnerability

The misconfiguration or weakness that allowed escalation, and why it worked.

### Exploitation

Step by step to root.

```
# commands and output
```

### Proof of access

`id` showing root and the proof flag.

```
# output
```

## Remediation

How each issue above should be fixed, most impactful first. This is the part a client actually acts on.

| Finding | Severity | Fix |
| --- | --- | --- |
| | | |

### Detection

How a defender (SOC / blue team) could have spotted or blocked each step: what logs, alerts, or controls would have caught it.

## Lessons learned

What to remember for next time: a tool that helped, a dead end that wasted time, a technique worth drilling.

## References

- Links to docs, CVEs, or writeups consulted.
