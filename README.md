# CyberShield Evidence Analyzer — Vercel Edition

A static, browser-based helper for lawful cybercrime evidence handling. It hashes selected files with SHA-256 and redacts common sensitive identifiers from text.

## Privacy design
- Evidence files and pasted text are processed in the user's browser.
- This app does not send files or text to a backend.
- No accounts, tracking, analytics, or third-party APIs are included.
- Redaction is heuristic and must be reviewed before sharing.

## Deploy to Vercel
1. Create a GitHub repository and upload `index.html`, `vercel.json`, and this README.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Framework preset: **Other**. No build command or output directory is required.
4. Deploy. Vercel will serve the static page.

You can also deploy from the Vercel CLI:
```bash
npm i -g vercel
vercel
```

## Features
- SHA-256 manifest for selected evidence files
- Local file metadata inventory
- Redaction for common CNIC-like IDs, emails, Pakistan-style mobile numbers, and long digit sequences
- Downloadable JSON manifest and redacted text

## Limitations
- This is not a forensic acquisition tool, legal chain-of-custody system, or compliance certification.
- Browser memory limits may make very large files impractical.
- Redaction can miss formats or redact harmless text. Manually review output.
- Use only evidence you own or are authorized to process.

## License
MIT
