# 🛡️ Cyber Shield: AI-Powered Cyber Threat Intelligence & Analysis Suite

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-Flask-black.svg)](https://flask.palletsprojects.com/)
[![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange.svg)](https://scikit-learn.org/)
[![Extension](https://img.shields.io/badge/Browser%20Extension-Manifest%20V3-green.svg)](https://developer.chrome.com/)

An **All-in-One Multi-Layered AI Cybersecurity Suite** designed for real-time threat intelligence and vulnerability assessment. The system detects and mitigates credential compromises, phishing/typo-squatting domains, and zero-day executable malware using hybrid statistical machine learning, heuristic rules, and cryptographic verification models.

---

## 🏗️ Architecture Flow
┌──────────────────────────────────────────────┐
                   │           USER / CHROME EXTENSION            │
                   └──────────────────────┬───────────────────────┘
                                          │
                ┌─────────────────────────┼─────────────────────────┐
                │ (Live Passwords)        │ (Visited URLs)          │ (Uploaded .exe)
                ▼                         ▼                         ▼
    ┌───────────────────────┐ ┌───────────────────────┐ ┌───────────────────────┐
    │   PASSWORD ANALYZER   │ │      URL SCANNER      │ │   MALWARE ANALYZER    │
    ├───────────────────────┤ ├───────────────────────┤ ├───────────────────────┤
    │ • TF-IDF + Logistic   │ │ • TF-IDF + Random     │ │ • Static PE Parsing   │
    │   Regression Model    │ │   Forest Model        │ │   (pefile)            │
    │ • HIBP API (SHA-1     │ │ • Jaro-Winkler Brand  │ │ • Shannon Entropy     │
    │   K-Anonymity)        │ │   Similarity Check    │ │   Calculation         │
    │ • NLP / Common Words  │ │ • WHOIS Domain Age    │ │ • Random Forest       │
    │ • Hardware Crack Time │ │ • Leetspeak Decoder   │ │   Classifier (10 Feat)│
    │ • Smart Generator     │ │ • Safe Brand WhiteList│ │ • Risk Scoring (95/5) │
    └───────────┬───────────┘ └───────────┬───────────┘ └───────────┬───────────┘
                │                         │                         │
                └─────────────────────────┼─────────────────────────┘
                                          ▼
                         ┌──────────────────────────────────┐
                         │       FLASK BACKEND ENGINE       │
                         │ (Auth, SQLite DB, Audit History) │
                         └────────────────┬─────────────────┘
                                          │
                                          ▼
                         ┌──────────────────────────────────┐
                         │   AUTOMATED PDF AUDIT REPORTS    │
                         │        (FPDF Generator)          │
                         └──────────────────────────────────┘
---

## 🔬 Core Security Engines

### 1️⃣ AI Password & Credential Engine
* **Character-Level TF-IDF + Logistic Regression:** Analyzes character n-grams and patterns on a 50/50 balanced strength dataset.
* **K-Anonymity Breach Detection:** Hashes user input with SHA-1, querying the HaveIBeenPwned API using only a 5-character prefix to preserve credential privacy while verifying breach exposure.
* **Hardware Crack-Time Simulation:** Calculates brute-force resistance across CPU ($100 \times 10^6$ g/s), GPU ($100 \times 10^9$ g/s), and Cluster hardware environments.
* **NLP Pattern Detection:** Flags common dictionary words, leetspeak variations, and birth year patterns.

### 2️⃣ Phishing & Typo-Squatting Scanner
* **Balanced Random Forest Model (50 Trees):** Vectorizes URL lexical features across 100,000 verified safe and phishing URLs.
* **Jaro-Winkler Distance:** Quantifies string distance against brand whitelists to flag typosquatting (0.82–0.99 similarity window) and leetspeak mimicry.
* **WHOIS Domain-Age Inspection:** Automatically detects and penalizes newly registered domains (<182 days old).

### 3️⃣ Static PE Malware Analyzer
* **Zero-Execution Forensic Parsing:** Parses raw Portable Executable headers (`pefile`) to extract 10 structural features without executing the binary.
* **Shannon Entropy Analysis:** Computes byte-level section entropy ($H(X) > 7.0$) to identify packed, obfuscated, and encrypted malware payloads.
* **Random Forest Classifier (100 Trees):** Evaluates compilation metadata, code size, optional headers, and DLL security flags.

### 4️⃣ Real-Time Chrome Extension (Manifest V3)
* **Debounced Event Listeners (800ms):** Monitors browser password fields and visited URLs without lagging client performance.
* **Direct Threat Alerts:** Dispatches native system notifications for compromised credentials or malicious web domains.

### 5️⃣ Central Portal & Automated Audit Reports
* Full user authentication with SQLite database history tracking.
* Generates downloadable, certificate-styled PDF security audit reports using `FPDF` with custom authenticity tokens.

---

## 🛠️ Tech Stack

| Domain | Tools & Libraries |
| :--- | :--- |
| **Backend** | Python, Flask, Flask-SQLAlchemy, Flask-CORS |
| **Machine Learning** | Scikit-Learn (LogisticRegression, RandomForestClassifier), Joblib, Pandas |
| **Feature Extraction** | `TfidfVectorizer`, `pefile`, `textdistance`, `whois`, Regex |
| **Browser Extension** | Chrome Manifest V3, Web Workers, Chrome Notifications API |
| **Reporting & Frontend** | HTML5, CSS3, JavaScript, Chart.js, FPDF |

---

## 🚀 Quickstart

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Bibisarwataliaziz/AI-powered-cyber-threat-analyzer.git
   cd AI-powered-cyber-threat-analyzer
   Install dependencies:
code
Bash
pip install -r requirements.txt
Run the application:
code
Bash
python app.py
Access the portal at http://127.0.0.1:5000/.
👤 Author
Bibi Sarwat Ali Aziz
Computer Science Graduate | AI & Full-Stack Engineer
LinkedIn Profile
