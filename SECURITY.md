# Security Policy

## Reporting a vulnerability
Do not post secrets, private printer/network credentials, exploit details, or sensitive logs in a public issue. Use GitHub private vulnerability reporting if enabled; otherwise open only a minimal issue until a private channel is established.

## Security expectations
- Never commit credentials, private printer endpoints, or user model data.
- Treat parser, file-format, and command-execution paths as untrusted-input surfaces.
- Review geometry/toolpath changes for safety and regression risk.
- Do not add AI that silently changes machine or print parameters.
- Keep dependencies/build tooling reviewable and avoid unnecessary churn.
- Add regression coverage for security-impacting fixes where practical.
