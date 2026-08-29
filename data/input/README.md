# Target Account Input Dataset

## Purpose

This dataset contains the initial account-level input records used by the AI-Powered GTM Lead Intelligence System.

The dataset is intentionally limited to minimal public company-level information required to begin the intelligence workflow.

The purpose of this dataset is to provide structured starting inputs for:

- Company research
- Data enrichment
- Data normalization
- ICP evaluation
- Intelligence scoring
- Account prioritization

The dataset does not contain downstream intelligence outputs or decision results.

---

## Dataset File

`target_accounts_v1.csv`

The dataset contains 12 real public B2B SaaS companies selected as reference accounts for portfolio system testing.

These companies are not represented as actual prospects, clients, or commercial opportunities.

They are used solely as a controlled demonstration dataset for testing the AI-Powered GTM Lead Intelligence System.

---

## Data Scope

This dataset contains public company-level information only.

It does not contain:

- Personal contact data
- Confidential information
- Client information
- Proprietary employer information
- Private prospect lists
- Credentials or secrets

---

## Input Schema

| Field | Description |
|---|---|
| `account_id` | Unique project-generated identifier |
| `company_name` | Public company name |
| `company_domain` | Primary public company domain |
| `company_type` | High-level company classification |
| `headquarters_country` | Country-level headquarters reference |
| `employee_range` | Normalized approximate employee range |
| `input_source` | Source classification |
| `notes` | Minimal neutral company context |

---

## Input Source Classification

The following source classifications are used:

### `official_website`

The input information was sourced primarily from the company's public official website.

### `official_website_plus_public_profile`

The input information was based on a combination of the company's official public website and publicly available business profile information.

---

## Employee Range Policy

Employee ranges are normalized reference ranges based on publicly available information.

They may be approximate.

The dataset should not be interpreted as an authoritative company directory or an official source of employee counts.

The employee ranges are used only as structured starting inputs for the portfolio demonstration system.

---

## Input Versus Enrichment Boundary

The dataset contains only the minimum information required to begin the intelligence workflow.

The following information must not be treated as input data in this dataset:

- Technology stack
- CRM platforms
- Marketing automation platforms
- Hiring signals
- Growth signals
- Funding signals
- GTM maturity
- ICP fit
- ICP score
- Account priority
- Decision reasoning
- Recommended action

These fields belong to later enrichment and decision stages of the AI-Powered GTM Lead Intelligence System.

---

## Data Quality Rules

The dataset follows these principles:

- One unique account per record
- No duplicate accounts
- Consistent field naming
- Consistent employee range formatting
- Neutral notes
- No hidden ICP conclusions
- No preloaded intelligence outcomes

The purpose is to allow the system to evaluate the accounts independently rather than embedding the expected results into the starting dataset.

---

## Dataset Limitations

This is a portfolio demonstration dataset.

Some public company information may change over time.

Employee ranges may vary across public sources and are treated as approximate normalized values.

The dataset represents a controlled starting point for enrichment and analysis rather than a permanent or authoritative company database.

---

## Intended Workflow

The intended project flow is:

```text
Target Account Input
        ↓
        Research and Enrichment
                ↓
                Data Normalization
                        ↓
                        ICP Evaluation
                                ↓
                                Scoring and Signal Assessment
                                        ↓
                                        Priority Classification
                                                ↓
                                                Explainable Decision Output
                                                        ↓
                                                        GTM Action Readiness
                                                        ```

                                                        ---

                                                        ## Portfolio Data Policy

                                                        This repository uses public company-level information for demonstration purposes.

                                                        No confidential, proprietary, private, or personal contact information should be added to this dataset.

                                                        Any future dataset expansion should follow the same data quality, source traceability, and public-information principles.
                                                        
