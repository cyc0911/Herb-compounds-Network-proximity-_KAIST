# Herb-Compounds Network Proximity Framework

This project aims to predict combinations of natural compounds that can achieve drug-like therapeutic effects while minimizing adverse side effects by applying a network medicine framework.

## Terpenoids.ipynb

Terpenoid-related compounds were extracted from the COCONUT database and mapped to STITCH database entries using standard InChIKeys. Through this process, compound–protein interaction information was successfully integrated, enabling the identification of potential target proteins associated with terpenoid compounds.

This workflow can be extended to compound datasets from natural product and traditional medicine databases such as COCONUT and HERB 2.0.

---

## COCONUT_PubChem_Bulk_data.ipynb

Terpenoids extracted from the COCONUT database were first mapped to PubChem Compound IDs (CIDs). Using these identifiers, compound–protein interaction data were collected from the STITCH database. Only high-confidence experimental interactions were retained to improve biological reliability. Protein identifiers were subsequently converted to Entrez Gene IDs, allowing the construction of a terpenoid–protein interaction network for downstream analyses.

Next, disease-associated proteins were collected and mapped onto the human protein–protein interaction network (Human Interactome). Network proximity between terpenoid target proteins and disease-related protein modules was then calculated to quantify the functional relationship between compounds and diseases.

---

## Project Overview and Future Direction

These analyses were conducted to evaluate whether the Network Proximity framework proposed in previous studies can be successfully applied to terpenoid compounds. The project is currently ongoing.

The ultimate goal is to extend the framework from single-compound analyses to herb-level analyses involving multiple compounds. By representing compound targets as functional protein modules and measuring their proximity to disease-related protein modules, we aim to identify novel therapeutic modules with potential clinical relevance.

Currently, we are developing methodologies that integrate multi-compound information with ADMET-related features to build more accurate and biologically meaningful predictive models. This approach is expected to improve the identification of effective natural compound combinations while considering both therapeutic efficacy and pharmacokinetic properties.
