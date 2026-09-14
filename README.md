🛡️ Cyber Shield: AI-Powered Cyber Threat Intelligence & Analysis Suite

Python Framework ML Extension

An All-in-One Multi-Layered AI Cybersecurity Suite designed for real-time threat
intelligence and vulnerability assessment. The system detects and mitigates
credential compromises, phishing/typo-squatting domains, and zero-day executable
malware using hybrid statistical machine learning, heuristic rules, and
cryptographic verification models.

🏗️ Architecture Flow

flowchart TD
    User["🖥️ User / Chrome Extension (Manifest V3)"]
    
    User -->|Live Passwords| M1["🔑 Password Vulnerability Engine<br/>• Char-level TF-IDF + Logistic Regression<br/>• HIBP API (SHA-1 K-Anonymity)<br/>• Hardware Crack-Time Simulation"]
    User -->|Visited URLs| M2["🌐 Phishing & URL Scanner<br/>• Word-level TF-IDF + Random Forest<br/>• Jaro-Winkler Brand Distance<br/>• WHOIS Domain Age Analysis"]
    User -->|Uploaded Binaries| M3["🛡️ Static PE Malware Analyzer<br/>• pefile Structural Header Parsing<br/>• Shannon Entropy H(X) > 7.0<br/>• Random Forest (100 Trees)"]
    
    M1 --> Core["⚙️ Flask Backend Engine<br/>(Authentication, SQLite DB, Audit History)"]
    M2 --> Core
    M3 --> Core
    
    Core --> Reports["📄 Automated PDF Audit Reports<br/>(FPDF Generator & Authenticity Tokens)"]

🔬 Core Security Engines

1️⃣ AI Password & Credential Engine

  - Character-Level TF-IDF + Logistic Regression: Analyzes character n-grams and
    patterns on a 50/50 balanced strength dataset.
  - K-Anonymity Breach Detection: Hashes user input with SHA-1, querying the
    HaveIBeenPwned API using only a 5-character prefix to preserve credential
    privacy while verifying breach exposure.
  - Hardware Crack-Time Simulation: Calculates brute-force resistance across CPU
    (100 \times 10^6 g/s), GPU (100 \times 10^9 g/s), and Cluster hardware
    environments.
  - NLP Pattern Detection: Flags common dictionary words, leetspeak variations,
    and birth year patterns.

2️⃣ Phishing & Typo-Squatting Scanner

  - Balanced Random Forest Model (50 Trees): Vectorizes URL lexical features
    across 100,000 verified safe and phishing URLs.
  - Jaro-Winkler Distance: Quantifies string distance against brand whitelists
    to flag typosquatting (0.82–0.99 similarity window) and leetspeak mimicry.
  - WHOIS Domain-Age Inspection: Automatically detects and penalizes newly
    registered domains (<182 days old).

3️⃣ Static PE Malware Analyzer

  - Zero-Execution Forensic Parsing: Parses raw Portable Executable headers
    (pefile) to extract 10 structural features without executing the binary.
  - Shannon Entropy Analysis: Computes byte-level section entropy (H(X) > 7.0)
    to identify packed, obfuscated, and encrypted malware payloads.
  - Random Forest Classifier (100 Trees): Evaluates compilation metadata, code
    size, optional headers, and DLL security flags.

4️⃣ Real-Time Chrome Extension (Manifest V3)

  - Debounced Event Listeners (800ms): Monitors browser password fields and
    visited URLs without lagging client performance.
  - Direct Threat Alerts: Dispatches native system notifications for compromised
    credentials or malicious web domains.

5️⃣ Central Portal & Automated Audit Reports

  - Full user authentication with SQLite database history tracking.
  - Generates downloadable, certificate-styled PDF security audit reports using
    FPDF with custom authenticity tokens.

🛠️ Tech Stack

| Domain                   | Tools & Libraries                                                         |
| :----------------------- | :------------------------------------------------------------------------ |
| **Backend**              | Python, Flask, Flask-SQLAlchemy, Flask-CORS                               |
| **Machine Learning**     | Scikit-Learn (LogisticRegression, RandomForestClassifier), Joblib, Pandas |
| **Feature Extraction**   | `TfidfVectorizer`, `pefile`, `textdistance`, `whois`, Regex               |
| **Browser Extension**    | Chrome Manifest V3, Web Workers, Chrome Notifications API                 |
| **Reporting & Frontend** | HTML5, CSS3, JavaScript, Chart.js, FPDF                                   |

🚀 Quickstart

1.  Clone the repository:

git clone https://github.com/Bibisarwataliaziz/AI-powered-cyber-threat-analyzer.git
cd AI-powered-cyber-threat-analyzer

2.  Install dependencies:

pip install -r requirements.txt

3.  Run the application:

python app.py

Access the portal at http://127.0.0.1:5000/.

👤 Author

Bibi Sarwat Ali Aziz
Computer Science Graduate | AI & Full-Stack Engineer

  - 🔗 LinkedIn Profile
    
