# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in Web Harmonium, please **do not** open a public issue. Instead:

1. **Email** the details to [security contact or use GitHub private vulnerability reporting]
2. **Include**:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if you have one)
3. **Response time**: We'll respond within 24-48 hours
4. **Responsible disclosure**: We appreciate responsible disclosure practices

## Security Measures

Web Harmonium implements several security best practices:

### Content Security Policy (CSP)
- Restricts script execution to authorized sources
- Prevents XSS (Cross-Site Scripting) attacks
- Configured in `.htaccess`

### HTTP Security Headers
- **HSTS** (HTTP Strict Transport Security) - Forces HTTPS
- **X-Frame-Options** - Prevents clickjacking
- **X-Content-Type-Options** - Prevents MIME sniffing
- **Referrer-Policy** - Controls referrer information

### Input Validation
- All user input is properly validated
- MIDI data is sanitized
- Keyboard input is handled safely

### HTTPS
- Website enforces HTTPS
- All external resources loaded over HTTPS
- Mixed content prevented

### Dependencies
- Minimal external dependencies
- All external resources loaded from trusted CDNs
- Libraries regularly updated

## Browser Security

Web Harmonium uses modern browser APIs securely:

- **Web Audio API** - Isolated audio context
- **Web MIDI API** - Requires user permission
- **localStorage** - Used only for user preferences
- **No localStorage of sensitive data**

## Third-Party Services

External services used:
- **GitHub API** - For fetching star count (read-only, no authentication)
- **Vercel** - Hosting platform with built-in security
- **CDNs** - Font Awesome, Google Fonts, CDNJS (trusted sources)

## Privacy

Web Harmonium respects user privacy:

- ✅ No personal data collection
- ✅ No tracking pixels
- ✅ No analytics beyond basic server logs
- ✅ No cookies (only localStorage for app settings)
- ✅ No third-party data sharing
- ✅ All audio processing happens locally

## Updates & Patches

Security updates are:
- Deployed immediately upon discovery
- Documented in release notes
- Applied to all deployed instances

## Best Practices for Users

When using Web Harmonium:

1. **Keep browser updated** - Ensures latest security patches
2. **Use HTTPS** - Always access via https://harmoniumweb.vercel.app
3. **Secure your system** - Use antivirus software
4. **Report suspicious activity** - Let us know about unusual behavior

## Supported Versions

| Version | Status | Support Until |
|---------|--------|----------------|
| 1.0.x | Active | Current |
| < 1.0 | Unsupported | - |

## Compliance

Web Harmonium complies with:
- OWASP Top 10 security guidelines
- GDPR (no personal data collection)
- Browser security standards
- Web content accessibility guidelines

## Security Checklist

- ✅ HTTPS enforcement
- ✅ CSP headers configured
- ✅ XSS protection enabled
- ✅ CSRF tokens (where applicable)
- ✅ Input validation
- ✅ Output encoding
- ✅ Secure dependencies
- ✅ Privacy-first design
- ✅ No sensitive data in logs
- ✅ Security headers configured

## Questions?

For security questions or concerns:
- Open a private security advisory on GitHub
- Email with security details
- Check our security policy

---

**Last Updated:** April 1, 2026  
**Status:** Active & Maintained
