# Info-Stealer Detection Lab (Blue Team)

This project demonstrates a small blue-team detection lab designed to simulate early-stage Info-Stealer malware behavior using Windows native logging and Elastic SIEM.

## Detection Focus

The lab focuses on detecting:

- PowerShell abuse
- Suspicious process creation
- Fileless malware execution
- Living-off-the-land binaries (LOLBins)

## Detection Logic

A behavior-based detection rule was implemented using:

Event ID 4688 (Process Creation)

The rule detects PowerShell spawning suspicious child processes such as:

PowerShell → cmd.exe

This chain is commonly associated with Info-Stealer loaders.

## Key Techniques Simulated

- Fileless malware execution
- Encoded PowerShell commands
- In-memory execution
- Process chain abuse

## Technologies

- Windows Event Logs
- PowerShell
- Elastic SIEM
- Behavior-based detection

## Documentation

Full report available here:

infostealer-simulation.pdf
