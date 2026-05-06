# RDK Engineering Self-Signed Certificates

⚠️ **DEVELOPMENT USE ONLY** - These certificates are strictly for development and testing purposes and must **NOT** be used in production environments.

## Overview

This repository contains self-signed certificates used by RDK Management (RDK-M) for development purposes. These certificates are made publicly available to improve the developer experience for the RDK community and facilitate the signing of Bolt applications during development.

## Purpose

The primary goals of this repository are to:

- **Ease Developer Experience**: Provide ready-to-use certificates for developers working with RDK-M and Bolt applications
- **Support Community Development**: Enable RDK community members to build, test, and sign reference Bolt applications
- **Accelerate Application Development**: Remove barriers to getting started with Bolt application development by providing reference signing certificates

## Contents

This repository includes the following certificates:

- `com.rdkcentral.ralf-private.key` - Private key for signing operations
- `com.rdkcentral.ralf-public.crt` - Public certificate
- `com.rdkcentral.ralf.p12` - PKCS#12 format (contains both private key and certificate)
  - **PSK/Password**: `RDKMRalf`

These certificates are used for signing reference Bolt applications provided by RDK-M to the community.

## ⚠️ Important Security Notice

**DO NOT USE THESE CERTIFICATES IN PRODUCTION**

These are self-signed development certificates with no Certificate Authority (CA) backing. They should only be used for local development and testing

### Production Requirements

For production deployments, you **MUST**:

1. Generate or obtain certificates from a trusted Certificate Authority (CA)
2. Implement proper key management and storage procedures
3. Establish secure certificate lifecycle management
4. Follow your organization's security policies and compliance requirements
5. Re-sign applications using your own CA-backed certificates

## Usage

### Downloading Certificates

Clone or download this repository to access the development certificates:

```bash
git clone https://github.com/rdk-m/bolt-engineering-certificates.git
cd bolt-engineering-certificates
```

### Signing Bolt Applications

Refer to [Signing Bolt Applications](https://wiki.rdkcentral.com/spaces/RDK/pages/447124247/Bolt+package+-+signing+and+verification#Boltpackagesigningandverification-BundleSigningProcess-Generatethesignedboltbundle) documentation for instructions on how to use these certificates to sign your applications during development. Remember to replace these certificates with production-grade, CA-backed certificates before deploying to production.

## License

Please refer to the [LICENSE](LICENSE) file for licensing information.

## Additional Resources

- [Signing Bolt Applications](https://wiki.rdkcentral.com/spaces/RDK/pages/447124247/Bolt+package+-+signing+and+verification#Boltpackagesigningandverification-BundleSigningProcess-Generatethesignedboltbundle)
- [Ralf Pack](https://github.com/rdkcentral/ralfpack)
- [Building Bolt Apps](https://wiki.rdkcentral.com/spaces/ASP/pages/463539631/Building+Bolt+Apps)
- [Bolt Applications](https://wiki.rdkcentral.com/spaces/RDK/pages/467661055/Bolt+applications)

---

**Last Updated**: May 2026

For questions or issues, please contact the RDK community.
