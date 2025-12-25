
# Gimbal CLI — Release Repository

This repository is used exclusively for publishing **Gimbal CLI release artifacts**.
It does not contain source code — only packaged builds intended for installation and automated updates.

The source code for Gimbal is maintained privately.

---

## 📦 Release Contents

Each GitHub release may include one or more of the following artifacts:

| Artifact                                | Description                                    |
| --------------------------------------- | ---------------------------------------------- |
| `gimbal-app-<version>.jar`              | Gimbal CLI application JAR                     |
| `gimbal-bundle-win64-<version>.zip`     | Full portable distribution with embedded JRE   |
| `gimbal-runtime-win64-<jreVersion>.zip` | Portable Windows runtime used by Gimbal        |
| `manifest.json`                         | Update manifest consumed by the Gimbal updater |

These artifacts are intended for:

* end-users installing Gimbal
* automated / silent update workflows
* enterprise deployment environments

---

## 🚀 Distribution Model

Gimbal is distributed as a **self-contained portable runtime**, meaning:

* the application ships with its own JRE
* no system-installed Java is required
* updates can be applied silently via the updater

Runtime and application updates are versioned and delivered through **GitHub Releases**.


---


## 📚 Documentation

Full product documentation, usage guides, and technical reference are available at:

👉 **[https://gimbal-docs.netlify.app](https://gimbal-docs.netlify.app)**

This site includes:

* installation and onboarding guides
* CLI usage and command reference
* update and deployment documentation

---

## 🧩 Intended Usage

Release artifacts in this repository are consumed by:

* Gimbal installer packages
* the Gimbal silent self-updater
* automated provisioning pipelines
* managed deployment environments

They may also be referenced by:

* enterprise software distribution tools
* internal update orchestration systems

---

## 🔒 Integrity & Verification

Gimbal distribution components may include:

* checksum validation
* integrity verification

If a release fails validation, the updater will not apply it.

---

## 📜 Licensing & Source Code

This repository does **not** contain source code.

Release artifacts are provided under the licensing terms included with the Gimbal application.

For questions regarding licensing or distribution, please contact the maintainers.

---

## 🧷 Support

For release-related issues:

* open an Issue in this repository
* or contact the Gimbal maintainers

* add a **Release Policy / retention section**
* or generate a **short minimal 5-line README** for corporate environments.

