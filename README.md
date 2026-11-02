CyberShield – Digital Evidence & Privacy Protection

Protecting Digital Evidence. Preserving Privacy.

CyberShield is a privacy-focused web application designed to help cybercrime victims and authorized investigators protect sensitive information and organize digital evidence.

The application provides tools to redact personal information from text, generate SHA-256 hashes for evidence files, and create downloadable reports.

1. Project Overview

Cybercrime victims often need to share screenshots, messages, emails, and documents when reporting online fraud, phishing, harassment, or identity theft.

These files may contain sensitive personal information such as CNIC numbers, phone numbers, email addresses, and financial identifiers.

CyberShield aims to reduce the risk of exposing this information while helping users maintain an organized record of their digital evidence.

2. Project Features

Sensitive Information Redaction

Detect and redact common personal identifiers from text, including:

- CNIC numbers
- Email addresses
- Pakistan-style mobile phone numbers
- Long numeric sequences that may contain sensitive information

Detected information is replaced with labels such as "[REDACTED:CNIC]" or "[REDACTED:EMAIL]".

Digital Evidence Hashing

Generate SHA-256 hashes for selected evidence files.

Each file's manifest includes:

- Filename
- File size
- Last modified date
- SHA-256 hash

This helps users maintain an inventory of evidence and check whether file contents have changed.

Downloadable Reports

- Export evidence manifests as JSON files.
- Download redacted text for safer sharing.
- Copy redacted text to the clipboard.

Privacy-First Processing

All file hashing and text redaction take place locally in the user's browser.

The application does not upload evidence files or pasted text to an external server.

3. Project Structure

cybershield-evidence-analyzer/
│
├── index.html
│   └── Main application interface and functionality
│
├── vercel.json
│   └── Vercel deployment configuration
│
├── README.md
│   └── Project documentation
│
├── LICENSE
│   └── MIT License
│
└── .gitignore
    └── Files excluded from version control

4. Technology Stack

- HTML5 – Application structure
- CSS3 – Responsive user interface
- JavaScript – Application functionality
- Web Crypto API – SHA-256 hashing
- Vercel – Website deployment
- GitHub – Source code hosting

5. How the Application Works

1. User opens the CyberShield website.
2. User selects evidence files or pastes text.
3. JavaScript processes the selected information locally.
4. Sensitive identifiers are detected and redacted.
5. SHA-256 hashes are generated for selected files.
6. A JSON evidence manifest or redacted text file is created.
7. User downloads the generated report.

6. Installation and Setup

Run Locally

Clone the repository:

git clone https://github.com/YOUR_USERNAME/cybershield-evidence-analyzer.git

Open the project folder:

cd cybershield-evidence-analyzer

Open "index.html" in a modern web browser.

No backend or database is required.

7. Deployment on Vercel

1. Create a GitHub repository.
2. Upload the project files.
3. Sign in to Vercel.
4. Import the GitHub repository.
5. Select the Other framework preset.
6. Deploy the project.

Vercel will generate a live website URL.

8. Intended Users

CyberShield is designed for:

- Cybercrime victims preparing evidence for reporting.
- Individuals who want to redact personal information before sharing documents.
- Cybersecurity students learning about digital privacy and evidence integrity.
- Authorized investigators organizing digital evidence.
- Developers interested in privacy-focused cybersecurity projects.

9. Project Limitations

- Redaction uses pattern matching and may miss some sensitive information.
- The application does not identify or trace cybercriminals.
- SHA-256 hashing does not prove who created a file or when it was originally created.
- This tool is not a replacement for professional digital forensics or legal chain-of-custody procedures.
- Very large files may be limited by browser memory.

Always review redacted content before sharing it.

10. Responsible Use

CyberShield is intended for lawful, defensive cybersecurity and privacy protection.

Use it only with evidence you own or are authorized to handle. Do not use it to collect, access, or expose another person's private information without permission.

11. Future Improvements

- Urdu and Roman Urdu sensitive information detection
- Scam message classification
- Phishing URL analysis
- Evidence timeline generation
- PDF report generation
- Additional sensitive information detection patterns

12. Contact

Developer: Fari Mazhar

Email: Farimazhar101@gmail.com

For questions, suggestions, or collaboration, feel free to contact me.

13. License

Copyright (c) 2026 Fari Mazhar

This project is licensed under the MIT License. See the "LICENSE" (LICENSE) file for details.

---

CyberShield – A privacy-first tool for safer digital evidence handling.
