# OpenSCA - Software Composition Analysis

OpenSCA is a lightweight, privacy-first vulnerability scanner that runs entirely in your browser. It analyzes your project's dependency manifest files (like package-lock.json or requirements.txt) and checks them against the OSV.dev database to identify known security vulnerabilities.

![Alt text](https://github.com/Th3l0newolf/openscaproject/blob/main/OpenSCA.png)
 

# 🚀 Features

* Zero Backend Required: No servers, no databases, no complex setup.

* Privacy First: Your manifest files are parsed locally in your browser. Only package names and versions are queried against the public OSV API. Your source code never leaves your device.

* Multi-Ecosystem Support: Scans dependencies for Node.js, Python, Go, Java, Rust, and PHP.

* Smart Scoring: innovative "Health Score" and "Risk Grade" (A-F) system to instantly gauge project security.

* Detailed Reporting: View severity (CVSS), affected versions, fix versions, and direct links to GitHub Advisories (GHSA).

* Export Data: Download full reports in JSON or CSV formats.

* Modern UI: Responsive design with built-in Dark Mode.

# 📦 Supported Ecosystems

OpenSCA supports parsing for the following lock files and manifests:
Ecosystem

| Ecosystem | Language(s)        | Supported Files                    |
|-----------|---------------------|------------------------------------|
| npm       | JavaScript / Node.js | package-lock.json, package.json    |
| PyPI      | Python               | requirements.txt                   |
| Go        | Go                   | go.mod                             |
| Maven     | Java                 | pom.xml                            |
| Crates.io | Rust                 | Cargo.lock                         |
| Packagist | PHP                  | composer.lock                      |

# 🛠️ How to Use


* Select Ecosystem: Choose the platform your project uses (e.g., npm for a Node.js project).

* Upload Manifest: Select your dependency file (e.g., package-lock.json).

* Scan: Click the "Scan" button.

* Analyze: Review the Health Score, Risk Grade, and individual vulnerability cards. Click any card for full details including fix versions.

# 🏗️ Tech Stack

* Core: Native HTML5, JavaScript (ES6+).

* Styling: Tailwind CSS (via CDN).

* Icons: Lucide.

* Data Source: OSV API (Google).

# 🔒 Privacy & Security

We believe security tools should be secure themselves.

Client-Side Parsing: All file parsing happens in JavaScript within your browser session.

Minimal Data Transfer: We do not upload your files. We only send a batch JSON query containing { package: "name", version: "1.0.0" } to the public OSV.dev API.

# 👤 Author

Crafted with ❤️ by Th3l0newolf.


