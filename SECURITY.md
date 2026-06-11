# Security Policy

## Supported Versions

The following versions of the project are currently supported with security updates.

| Version        | Supported |
| -------------- | --------- |
| Latest Release | ✅ Yes     |
| Older Releases | ❌ No      |

Users are encouraged to use the latest version of the project to receive security improvements and bug fixes.

---

## Reporting a Vulnerability

The security of this project is important. If you discover a security vulnerability, please report it responsibly.

### Please Do Not

* Open a public GitHub issue for security vulnerabilities.
* Publicly disclose the vulnerability before it has been reviewed and addressed.

### How to Report

Please provide the following information:

* Description of the vulnerability
* Steps to reproduce the issue
* Potential impact
* Screenshots or proof-of-concept (if applicable)
* Suggested mitigation (optional)

### Contact

To report a security issue, please contact the project maintainer:

**Maintainer:** Aman Sati

You may also create a private security advisory through GitHub Security Advisories if available.

---

## Security Considerations

This project processes data locally on the user's machine and does not intentionally collect, store, or transmit personal information.

### Webcam Access

* The application requires access to a webcam for gesture detection.
* Camera access is only used while the application is running.
* No camera data is intentionally uploaded to external servers.

### Local Data Storage

* Gesture datasets are stored locally.
* Users are responsible for protecting any collected image data.
* Avoid sharing datasets containing sensitive information.

### Machine Learning Model

* The project uses a locally stored trained model (`keras_model.h5`).
* Only trusted model files should be used.
* Do not load models obtained from unverified sources.

### Dependencies

Project dependencies may occasionally contain security vulnerabilities.

Users should regularly update dependencies:

```bash
pip install --upgrade -r requirements.txt
```

and periodically check for known vulnerabilities using:

```bash
pip list --outdated
```

---

## Best Practices

When using this project:

* Keep Python and dependencies updated.
* Use trusted datasets and model files.
* Run the application in a secure environment.
* Review third-party code before integration.
* Avoid exposing sensitive files in public repositories.

---

## Responsible Disclosure Process

When a security report is received:

1. The report will be reviewed.
2. The vulnerability will be verified.
3. A fix will be developed and tested.
4. A security update will be released.
5. Credit may be given to the reporter unless anonymity is requested.

---

## Scope

This security policy applies to:

* Source code
* Machine learning model integration
* GUI application
* Dataset collection module
* Gesture recognition module
* Text-to-speech module

Third-party libraries and external dependencies are governed by their own security policies and are outside the direct scope of this project.

---

## Acknowledgements

We appreciate the efforts of security researchers and contributors who help improve the security and reliability of this project.

Thank you for helping keep this project secure.

