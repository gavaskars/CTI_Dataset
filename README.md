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

## Purpose

This dataset provides the structured MITRE ATT&CK knowledge base required for:

- Knowledge Graph construction
- Technique and tactic retrieval
- Threat actor mapping
- Relationship extraction
- Graph-based Retrieval-Augmented Generation (Graph RAG)

## Source

IEEE DataPort

MITRE ATT&CK Dataset for Knowledge Graph Enhanced RAG Cyber Threat Intelligence

https://ieee-dataport.org/documents/mitre-attack-dataset-knowledge-graph-enhanced-rag-cyber-threat-intelligence

## Contents

Typical files include

- Enterprise ATT&CK Techniques
- Tactics
- Groups
- Software
- Relationships
- STIX Objects
- ATT&CK IDs
- Metadata

## Usage

Used for

- Building Neo4j Knowledge Graph
- Entity Linking
- ATT&CK ontology
- Multi-hop reasoning
- Threat intelligence retrieval

---

# 2. Vulnerability → ATT&CK Mapping Knowledge Base

## Purpose

Provides expert-labelled mappings between vulnerabilities and MITRE ATT&CK tactics and techniques.

This dataset enables:

- CVE → Technique prediction
- ATT&CK classification
- Vulnerability prioritization
- Threat reasoning

## Source

IEEE DataPort

Expert-Labeled Vulnerability Tactic and Technique Mapping Dataset

https://ieee-dataport.org/documents/expert-labeled-vulnerability-tactic-and-technique-mapping-dataset

## Contents

Typical attributes

- CVE ID
- ATT&CK Tactic
- ATT&CK Technique
- Technique ID
- Labels
- Expert annotations

## Usage

Used for

- Supervised learning
- Multi-label classification
- Knowledge Graph enrichment
- Vulnerability reasoning

---

# 3. Cyber Threat Intelligence (CTI) Reports

These datasets provide real-world threat intelligence reports from security vendors and public sources.

---

## 3.1 Public CTI Reports

### Purpose

Collection of publicly available CTI reports describing

- APT campaigns
- Malware
- Ransomware
- Intrusion techniques
- Threat actors

These reports serve as the primary corpus for LLM-based information extraction.

### Source

IEEE DataPort

Cyber Threat Intelligent (CTI) Dataset Generated from Public Security Reports and Malware

https://ieee-dataport.org/open-access/cyber-threat-intelligent-cti-dataset-generated-public-security-reports-and-malware

### Usage

Used for

- Named Entity Recognition
- Relation Extraction
- Event Extraction
- Threat Actor Extraction
- Malware Extraction
- ATT&CK Technique Identification
- Knowledge Graph Construction

---

## 3.2 CVE Dataset

### Purpose

Official repository containing all published CVE records.

Provides detailed vulnerability descriptions for

- Software vulnerabilities
- Vendors
- Products
- CVSS information
- References

### Source

GitHub

CVEProject - cvelistV5

https://github.com/CVEProject/cvelistV5

### Contents

- CVE JSON records
- CVSS scores
- CWE mappings
- References
- Metadata

### Usage

Used for

- Vulnerability Knowledge Graph
- Entity Linking
- CVE enrichment
- Threat intelligence fusion

---

# 4. Vulnerability Dataset

## Purpose

Large-scale dataset containing

- National Vulnerability Database (NVD)
- CVE reports
- Affected libraries
- Software versions

Useful for vulnerability analytics and software risk assessment.

## Source

Kaggle

NVD CVE Reports and Affected Libraries

https://www.kaggle.com/datasets/dngchnhtrn/nvd-cve-reports-and-affected-libraries

## Contents

Typical attributes

- CVE ID
- Vendor
- Product
- Library
- Version
- Description
- Severity
- References

## Usage

Used for

- Vulnerability prediction
- Software dependency analysis
- Product risk assessment
- Knowledge Graph enrichment

---

# Suggested Workflow

```
                Public CTI Reports
                        │
                        ▼
            LLM-based Information Extraction
                        │
                        ▼
               Entity & Relation Extraction
                        │
                        ▼
                Knowledge Graph Creation
                        ▲
                        │
        MITRE ATT&CK Knowledge Base
                        │
                        ▼
      Vulnerability → ATT&CK Mapping Dataset
                        │
                        ▼
             CVE Dataset + NVD Dataset
                        │
                        ▼
            Vulnerability Knowledge Graph
                        │
                        ▼
          Graph Retrieval / RAG / QA System
```

---

# Recommended Directory Layout

```
datasets/

├── attack_knowledge_base/
│   ├── ATTACKEnterprise.xlsx
│   ├── Techniques.xlsx
│   ├── Tactics.xlsx
│   └── Relationships.xlsx
│
├── vulnerability_attack_mapping/
│   ├── mapping.csv
│   └── labels.csv
│
├── cti_reports/
│   ├── public_reports/
│   │     ├── apt1.pdf
│   │     ├── apt28.pdf
│   │     └── ...
│   │
│   └── cve_reports/
│         ├── 2024/
│         ├── 2025/
│         └── 2026/
│
├── vulnerability_dataset/
│   ├── nvd.csv
│   └── affected_libraries.csv
│
└── README.md
```

---

# Research Applications

These datasets support research in:

- Cyber Threat Intelligence (CTI)
- MITRE ATT&CK Mapping
- Knowledge Graph Construction
- Retrieval-Augmented Generation (RAG)
- Graph Neural Networks (GNN)
- Large Language Models (LLMs)
- Vulnerability Analysis
- Threat Hunting
- Attack Path Prediction
- Explainable Cybersecurity AI
- Threat Actor Profiling
- Cybersecurity Question Answering

---

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
