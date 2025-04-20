# SoteriaSec LimaCharlie Lookups & Detection Rules

This repository contains automated Infrastructure‑as‑Code (IaC) definitions for creating and maintaining **LimaCharlie** lookup lists and their accompanying detection rules. It is maintained by **SoteriaSec** to help you deploy preconfigured threat indicators and detection logic into your LimaCharlie environment.

## 📂 Repository Structure

Each top‑level folder represents a Lookup pack. Inside each folder you will find:

- A complete **IaC YAML** file that defines:
  - The **Lookup** (list of indicators, domains, IPs, etc.) in JSON format
  - Any associated **Detection Rules** that consume that Lookup
- Supporting documentation or scripts as required

## 🔄 Automated Updates

All Lookups in this repository are **automatically refreshed once a week**. You can inspect the scheduled GitHub Actions workflow to see exactly when and how updates are performed.

## 🚀 Included Lookups

- **LOLRMM-Domains**  
  Infrastructure‑as‑Code for the LOLRMM domain DNS lookup, sourced from [LOLRMM.io](https://lolrmm.io/).

## 🛠️ Getting Started

1. **Apply** the IaC YAML in your LimaCharlie Console or via the CLI to provision the Lookup and Detection Rules.
2. **Manual Sync** in the Lookup Manager to ensure the new lookups are pulled into LimaCharlie.
3. Add any additional **Detection** rules or tuning as needed for each lookup. There are default detections provided, however, you may needs to tune out any false positives.

## 🤝 Contributing

If you find issues, have suggestions, or wish to add new Lookups and Rules:

1. Submit an **Issue** describing your proposal.

We welcome your feedback and contributions!

---

© 2025 SoteriaSec. All rights reserved.  