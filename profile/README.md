# Welcome to Kypello

<div align="center">

### The Open Source, S3-Compatible Object Store.
**High Performance. Enterprise Identity. Fully AGPLv3.**

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Go Version](https://img.shields.io/github/go-mod/go-version/kypello-io/kypello)](https://github.com/kypello-io/kypello)

</div>

---

### 🚀 About Kypello

**Kypello** (Greek for *Vessel* or *Chalice*) is a high-performance, distributed object storage suite designed for the cloud-native era. It is a community-driven fork of the MinIO project, established to preserve and maintain critical enterprise functionality—specifically **OpenID Connect (OIDC)** and **SSO integration**—within the open-source ecosystem.

We believe that secure identity management is a fundamental requirement for modern infrastructure, not a luxury feature. Kypello ensures these features remain accessible to everyone under the **GNU AGPLv3** license.

### 📦 Our Ecosystem

| Repository | Role | Description |
| :--- | :--- | :--- |
| **[kypello](https://github.com/kypello-io/kypello)** | **Core Server** | The object storage server. Fully S3-compatible, resilient, and built for scale. |
| **[kypello-ui](https://github.com/kypello-io/kypello-ui)** | **Console / UI** | The management dashboard. Includes the **restored OIDC/SSO login flows** and identity management tools. |
| **[kes](https://github.com/kypello-io/kes)** | **Encryption** | Key Encryption Service. Bridges the Kypello server with external KMS providers (Vault, AWS KMS, etc). |

### 🔑 Why Kypello?

1.  **Restored OIDC Support:** Seamless integration with Zitadel, Keycloak, Okta, Active Directory, and Google Workspace out of the box.
2.  **100% Open Source:** No "open core" limitations. What you see is what you get, licensed under AGPLv3.
3.  **Drop-in Replacement:** API compatible with S3 and generally compatible with existing MinIO deployments (with configuration updates).

### 🛠️ Quick Start

To build Kypello from source with the restored UI:

```bash
# Clone the server
git clone https://github.com/kypello-io/kypello.git
cd kypello

# Build the binary (automatically embeds the Kypello UI)
make server

# Run the server
./kypello server /data
