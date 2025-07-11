# Blockchain Evidence Management System

Managing digital forensic evidence with integrity and accountability is critical in law enforcement and legal proceedings. This project proposes a web-based system that ensures the traceability and tamper-evident storage of forensic evidence using blockchain principles.

The system allows investigators to upload, track, and retrieve digital files while maintaining a secure chain of custody. Although it does not implement a full decentralized blockchain, it utilizes cryptographic hashing, timestamping, and audit trails to simulate the core properties of blockchain technology within a Django web application.

---

## 🔧 Technologies

- Python 3.8+
- Django 3.x
- SQLite3
- HTML / Bootstrap
- `hashlib` (for file hashing)

---

## 📦 Modules

- Evidence Upload & Management
- User Authentication (Admin, Investigator)
- Hashing Engine (SHA256)
- Audit Trail with Timestamps
- Tamper Detection View
- Report Generation (PDF/HTML)

---

## ⚙️ How It Works

1. **Evidence Submission**  
   Investigators upload forensic files through a secure web interface. Each file is hashed using SHA256 to generate a unique digital fingerprint.

2. **Hash Chain Ledger**  
   Each uploaded file is timestamped and linked to the previous record, mimicking a blockchain-like chain. This creates a verifiable trail of actions without using a distributed network.

3. **Tamper Detection**  
   Any changes to evidence files or metadata break the hash sequence, triggering an alert that the file may have been tampered with.

4. **Audit & Reporting**  
   The system logs every activity (upload, access, hash verification) and allows administrators to generate detailed audit reports.

5. **Authentication & Roles**  
   Different user roles (Admin, Investigator) control access and ensure accountability for each action performed on the evidence.

---

## 📊 Results

| Task                                      | Output                                                                 |
|-------------------------------------------|------------------------------------------------------------------------|
| File Upload & Hashing                     | ✅ Successful for all tested file formats (PDF, PNG, ZIP, DOCX, etc.)  |
| Tamper Detection Accuracy                 | ✅ 100% detection for file content modification                        |
| Admin vs. Investigator Access Control     | ✅ Successfully enforced role-based actions                            |
| Ledger Integrity Verification             | ✅ Chain maintained correctly across 50+ evidence entries              |
| Report Generation                         | ✅ Exported 100% accurate hash and metadata summaries as PDF/HTML      |

---

