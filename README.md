# AI-Based Risk Assessment with Blockchain Case Management

An AI-powered risk assessment system that combines **Machine Learning** with **Blockchain** to evaluate case-level risk and maintain a tamper-evident case management ledger.

The application provides an interactive **Streamlit dashboard** where users can enter case details, receive an AI-generated risk assessment, and securely record the assessment on a custom blockchain ledger.

## 🚀 Features

- 🤖 **AI-Based Risk Assessment**
  - Predicts whether a case is **High Risk** or **Low Risk**
  - Generates a probability-based risk score
  - Uses demographic, control, abuse, and recruiter-related indicators

- ⛓️ **Blockchain Case Management**
  - Stores assessed cases in a blockchain ledger
  - Each block contains case information, timestamp, hash, and previous hash
  - Links blocks using cryptographic hashes

- 🔐 **Blockchain Integrity Validation**
  - Validates the complete blockchain
  - Detects unauthorized modification of stored case records
  - Verifies relationships between consecutive blocks

- 📊 **Interactive Streamlit Interface**
  - Case-data input form
  - Real-time risk assessment
  - Blockchain ledger visualization
  - One-click blockchain validation

## 🏗️ System Architecture

```text
User
  │
  ▼
Streamlit Web Interface
  │
  ├── Case Details
  │     ├── Demographics
  │     ├── Abuse Indicators
  │     ├── Control Indicators
  │     └── Recruiter Relationship
  │
  ▼
Data Preprocessing
  │
  ├── One-Hot Encoding
  └── Feature Alignment
  │
  ▼
Machine Learning Model
  │
  ├── Prediction
  └── Risk Probability
  │
  ▼
Risk Assessment
  │
  ├── High Risk
  └── Low Risk
  │
  ▼
Blockchain Ledger
  │
  ├── Case Data
  ├── Timestamp
  ├── Block Hash
  └── Previous Block Hash
  │
  ▼
Blockchain Validation
