# SoteriaSec LimaCharlie Lookups & Detection Rules

This repository contains automated Infrastructure‑as‑Code (IaC) definitions for creating and maintaining **LimaCharlie** lookup lists and their accompanying detection rules. It is maintained by **SoteriaSec** to help you deploy preconfigured threat indicators and detection logic into your LimaCharlie environment.

## 📂 Repository Structure

Each top‑level folder represents a Lookup pack. Inside each folder you will find:

- A complete **IaC YAML** file that defines:
  - The **Lookup** (list of indicators, domains, IPs, etc.) in JSON format which link back to the JSON lists in this repository
  - Any associated IaC **Detection Rules** that uses that Lookup lists against events from your sensors
- Supporting documentation or scripts as required

## 🔄 Automated Updates

All Lookups in this repository are **automatically refreshed once a week**. You can inspect the scheduled GitHub Actions workflow to see exactly when and how updates are performed - if you're really keen to see how they work.

## 🚀 Included Lookups

- **LOLRMM-Domains**  
  [Infrastructure‑as‑Code for the LOLRMM domain DNS lookup](LOLRMM-Domains/rmm-domain-lookup-IaC-config.yaml), sourced from [LOLRMM.io](https://lolrmm.io/).

## 🛠️ Getting Started

1. **Apply** the IaC YAML in your LimaCharlie Console or via the CLI to provision the Lookup and Detection Rules.
2. **Manual Sync** in the Lookup Manager to ensure the new lookups are pulled into LimaCharlie.
3. Add any additional **Detection** rules or tuning as needed for each lookup. There are default detections provided, however, you may needs to tune out any false positives.

## 🤝 Contributing

If you find issues, have suggestions, or wish to add new Lookups and Rules:

1. Submit an **Issue** describing your proposal.

We welcome your feedback and contributions!

## Need More Help

Reach out to [SoteriaSec](https://soteriasec.io) directly if you need assistance with LimaCharlie, security operations, threat detection, or incident response in general.

## Disclaimer

The lookup lists and detection rules provided in this repository are for community use and, in the majority of cases, use data sources from third parties that SoteriaSec has no control over. We've provided these lookup lists and detection rules as a "bridge" between other projects with valuable data and those using LimaCharlie. While we try to ensure they are accurate and don't produce too many false positives, we take no responsibility for their accuracy or warrant they will prevent a compromise or even be suitable for your environment. Please use them at your own risk and ensure you test/alter/update/use them to suit your environment best. 

---

© 2025 [SoteriaSec](https://soteriasec.io). All rights reserved.  