# 🛡️ Cyber Shield: AI-Powered Cyber Threat Intelligence & Analysis Suite

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Chrome_Extension-Manifest_V3-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" />
  <img src="https://img.shields.io/badge/Database-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
</p>

An **All-in-One Multi-Layered AI Cybersecurity Suite** designed for real-time threat intelligence and vulnerability assessment. The system detects and mitigates credential compromises, phishing/typo-squatting domains, and zero-day executable malware using hybrid statistical machine learning, heuristic rules, and cryptographic verification models.

---

## 🏗️ System Architecture & Threat Flow

| Layer / Pipeline | Module | Technical Architecture & Mechanisms |
| :--- | :--- | :--- |
| **Client Layer** | **Chrome Extension (Manifest V3)** | Debounced (800ms) DOM input monitoring, active tab URL interception, and desktop threat alerts |
| **Engine 1** | **Password Vulnerability Engine** | Char-level TF-IDF + Logistic Regression, SHA-1 K-Anonymity (HIBP API), and hardware crack-time simulation |
| **Engine 2** | **Phishing & Typo-Squatting Scanner** | Random Forest (100k URLs), Jaro-Winkler brand similarity (0.82–0.99), and WHOIS domain age heuristics |
| **Engine 3** | **Static PE Malware Analyzer** | Zero-execution header parsing via `pefile`, Shannon Entropy calculation ($H(X) > 7.0$), and Random Forest (100 trees) |
| **Core Layer** | **Flask Backend Engine** | REST API endpoints, user authentication, SQLite scan audit history, and security middleware |
| **Audit Layer** | **Automated PDF Reports** | Professional security audit report generation via `FPDF` with cryptographic verification tokens |

---

## 🔬 Deep Technical Breakdown

### 1️⃣ AI Password & Credential Engine
* **Character-Level TF-IDF + Logistic Regression:** Analyzes character sub-words, n-grams, and special symbol patterns trained on a balanced strength dataset.
* **K-Anonymity Breach Detection:** Hashes user input with SHA-1, querying the HaveIBeenPwned API using only the first 5 characters (prefix) to preserve zero-exposure credential privacy.
* **Hardware Crack-Time Simulation:** Calculates brute-force resistance across CPU ($100 \times 10^6$ g/s), GPU ($100 \times 10^9$ g/s), and Cluster hardware environments.
* **NLP Pattern Matching:** Flags common dictionary words, leetspeak variations, and birth year patterns.

### 2️⃣ Phishing & Typo-Squatting Scanner
* **Balanced Random Forest Model (50 Trees):** Vectorizes URL lexical tokens across 100,000 verified safe and phishing websites.
* **Jaro-Winkler Distance:** Quantifies string distance against brand whitelists to flag typosquatting (0.82–0.99 similarity window) and leetspeak mimicry.
* **WHOIS Domain-Age Inspection:** Automatically detects and flags newly registered domains (<182 days old).

### 3️⃣ Static PE Malware Analyzer
* **Zero-Execution Forensic Parsing:** Parses raw Portable Executable headers (`pefile`) to extract 10 structural features without executing the binary on the host machine.
* **Shannon Entropy Analysis:** Computes byte-level section randomness ($H(X) > 7.0$) to detect packed, encrypted, and obfuscated malware payloads.
* **Random Forest Classifier (100 Trees):** Evaluates compilation metadata, code size, optional headers, and DLL security flags.

### 4️⃣ Real-Time Chrome Extension (Manifest V3)
* **Debounced Event Listeners (800ms):** Monitors browser password fields and visited URLs without lagging client performance.
* **Direct Threat Alerts:** Dispatches native system notifications for compromised credentials or malicious web domains.

### 5️⃣ Central Portal & Automated Audit Reports
* Full user authentication with SQLite database history tracking.
* Generates downloadable, certificate-styled PDF security audit reports using `FPDF` with custom authenticity tokens.

---

## 🛠️ Complete Tech Stack

| Domain | Tools & Libraries |
| :--- | :--- |
| **Backend Framework** | Python, Flask, Flask-SQLAlchemy, Flask-CORS |
| **Machine Learning** | Scikit-Learn (LogisticRegression, RandomForestClassifier), Joblib, Pandas |
| **Feature Extraction** | `TfidfVectorizer`, `pefile`, `textdistance`, `whois`, Regex |
| **Browser Extension** | Chrome Manifest V3, Service Workers, Chrome Notifications API |
| **Reporting & Frontend** | HTML5, CSS3, JavaScript, Chart.js, FPDF |

---

## 🚀 Quickstart Guide

## 🚀 Quickstart Guide

**1. Clone the repository:**
<pre><code>git clone https://github.com/Bibisarwataliaziz/AI-powered-cyber-threat-analyzer.git
cd AI-powered-cyber-threat-analyzer</code></pre>

**2. Install dependencies:**
<pre><code>pip install -r requirements.txt</code></pre>

**3. Run the application:**
<pre><code>python app.py</code></pre>

<p>Access the portal locally at <code>http://127.0.0.1:5000/</code></p>

---

## 👤 Author

**Bibi Sarwat Ali Aziz**  
*Computer Science Graduate | AI & Full-Stack Engineer*  
* 🔗 <a href="https://www.linkedin.com/in/bibisarwataliaziz/">LinkedIn Profile</a>  
  
