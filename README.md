This project simulates a Life Sciences Data Ecosystem, bridging the gap between raw analytical instrument output and cloud-based clinical research platforms.

Key Architecture Components:
Edge Data Simulation: Ingests raw batch outputs (CSV/JSON) simulating high-throughput diagnostic instruments (Sequencers/Analyzers).

Automated QC Logic (Pipedream Middleware): A serverless Python engine that executes "Out-of-Specification" (OOS) detection. It validates instrument calibration metrics (e.g., thermal stability) and flags samples that fail data integrity thresholds before they reach the LIMS.

Diagnostic Quality Monitor (Streamlit): A centralized dashboard for lab managers to track batch integrity scores, analyte concentrations, and instrument performance trends in real-time.

Standards-First Approach: Implements data mapping to LOINC and UCUM (Units of Measure) to ensure seamless interoperability with global laboratory information management systems (LIMS).

Engineering Highlights for Thermo Fisher:
Data Integrity: Automated "Chain of Custody" simulation via GitHub-to-Pipedream versioning.

Validation: Implementation of automated "Fail-Safe" triggers for calibration drift.

Scalability: Decoupled architecture ready for FHIR-based clinical trial integration.
