# CTF Walkthroughs

OSCP-style walkthroughs and reports for intentionally vulnerable machines, worked through on the purplehax streams. The focus is not just getting root, it is practicing how to enumerate methodically and how to write the findings up like a real engagement report.

## Why this repo exists

Compromising a box is half the skill. The other half is reporting: recording what you did, why it worked, proving it, and explaining how a defender would have stopped it. Every box here gets a full writeup built from the same template so the reporting muscle gets as much practice as the exploitation.

## The lab

All targets run in an isolated VirtualBox internal network. Nothing here touches the internet or any production system.

| Role | Host | Address |
| --- | --- | --- |
| Attacker | Kali (`purplehaxlabs`) | 10.10.50.100 |
| Target | ctf-DC-1 | 10.10.50.101 |
| Target | ctf-DC-2 | 10.10.50.102 |
| Target | ctf-Kioptrix1 | 10.10.50.103 |

Addresses come from the lab DHCP server and can change between boots. Confirm the live address with a host-discovery sweep at the start of each session.

## Boxes

| Box | Source | Difficulty | Address | Status | Report |
| --- | --- | --- | --- | --- | --- |
| Kioptrix Level 1 | VulnHub | Easy | 10.10.50.103 | Not started | [boxes/kioptrix-level-1](boxes/kioptrix-level-1/README.md) |
| DC-1 | VulnHub | Easy | 10.10.50.101 | Not started | [boxes/dc-1](boxes/dc-1/README.md) |
| DC-2 | VulnHub | Easy | 10.10.50.102 | Not started | [boxes/dc-2](boxes/dc-2/README.md) |

## Writing a new report

1. Copy [`TEMPLATE.md`](TEMPLATE.md) into `boxes/<box-name>/README.md`.
2. Fill it in as you go. Paste commands and output as you run them, not from memory afterward.
3. Keep screenshots in the box folder next to the report.
4. Commit on a branch named for the box (for example `kioptrix-level-1`) and open a pull request. Keep `main` to finished, reviewed writeups.

## Scope and authorization

Everything in this repo is performed against machines I own, running locally in an isolated lab, for training. Do not point any of these techniques at systems you are not explicitly authorized to test.
