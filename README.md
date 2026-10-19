# AgentTesla Sandbox Analysis

Behavior analysis of an AgentTesla sample (SHA256 e76c5c79066d31f5e84b172d61ba575926a18505efa47a9d9a0c7c1c0ced4768) run in an isolated VirtualBox lab using Process Monitor, Regshot, tcpdump, INetSim and dnsmasq.

## What's in this repository

The full report is the Word document in this repository. It covers the lab setup, process, registry and network findings, classification, indicators of compromise (IOCs), a threat actor hypothesis, and defence recommendations.

## Key findings

- The sample is a .NET information stealer from the AgentTesla family.
- It starts a copy of itself and the original process exits.
- It looks up smtp.yandex.com about every 20 minutes and connects to port 587, the mail submission port.
- The mail content was encrypted, so no stolen data was observed.

## Note

This repository contains no malware. The sample can be obtained from MalwareBazaar using the hash above.
