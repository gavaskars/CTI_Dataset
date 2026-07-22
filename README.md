# CTI_Dataset
# README.md

# Datasets for Knowledge Graph-Based Cyber Threat Intelligence (CTI)

## Overview

This repository utilizes multiple publicly available cybersecurity datasets for constructing a comprehensive **Cyber Threat Intelligence (CTI) Knowledge Graph**, performing **MITRE ATT&CK mapping**, **vulnerability analysis**, **LLM-assisted information extraction**, and **Retrieval-Augmented Generation (RAG)** based cybersecurity applications.

The datasets have been selected to cover the complete CTI pipeline:

- MITRE ATT&CK Knowledge Base
- CVE → ATT&CK Mapping
- Cyber Threat Intelligence Reports
- Vulnerability Databases
- Common Vulnerabilities and Exposures (CVE)

---

# Dataset Structure

```
datasets/
│
├── attack_knowledge_base/
├── vulnerability_attack_mapping/
├── cti_reports/
│   ├── public_reports/
│   └── cve_reports/
├── vulnerability_dataset/
└── README.md
```

---

# 1. ATT&CK Knowledge Base

## Source
IEEE DataPort
MITRE ATT&CK Dataset for Knowledge Graph Enhanced RAG Cyber Threat Intelligence
https://ieee-dataport.org/documents/mitre-attack-dataset-knowledge-graph-enhanced-rag-cyber-threat-intelligence

# 2. Vulnerability → ATT&CK Mapping Knowledge Base
## Purpose
Provides expert-labelled mappings between vulnerabilities and MITRE ATT&CK tactics and techniques.
## Source
IEEE DataPort
Expert-Labeled Vulnerability Tactic and Technique Mapping Dataset
https://ieee-dataport.org/documents/expert-labeled-vulnerability-tactic-and-technique-mapping-dataset

# 3. Cyber Threat Intelligence (CTI) Reports

These datasets provide real-world threat intelligence reports from security vendors and public sources.

## 3.1 Public CTI Reports

### Source
IEEE DataPort
Cyber Threat Intelligent (CTI) Dataset Generated from Public Security Reports and Malware
https://ieee-dataport.org/open-access/cyber-threat-intelligent-cti-dataset-generated-public-security-reports-and-malware

## 3.2 CVE Dataset

### Source
GitHub
CVEProject - cvelistV5
https://github.com/CVEProject/cvelistV5
# 4. Vulnerability Dataset

## Source

Kaggle

NVD CVE Reports and Affected Libraries

https://www.kaggle.com/datasets/dngchnhtrn/nvd-cve-reports-and-affected-libraries


# Citation

If these datasets are used in academic publications, please cite the original dataset providers:

1. IEEE DataPort – MITRE ATT&CK Dataset for Knowledge Graph Enhanced RAG Cyber Threat Intelligence
2. IEEE DataPort – Expert-Labeled Vulnerability Tactic and Technique Mapping Dataset
3. IEEE DataPort – Cyber Threat Intelligence Dataset Generated from Public Security Reports and Malware
4. CVE Project (cvelistV5)
5. National Vulnerability Database (NVD)
6. Kaggle – NVD CVE Reports and Affected Libraries

---

# License

Each dataset is distributed under its respective license. Users should consult the original dataset providers for licensing, redistribution, and usage restrictions before using the datasets in research or commercial applications.
