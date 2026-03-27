# FakeGPT Browser Extension Investigation

## 1. What Happened?

The cybersecurity team detected suspicious activity on the organization's network. Multiple users reported unusual browser behavior after installing a browser extension named "ChatGPT", which appeared to be legitimate.

---

## 2. Analysis Performed

- Investigated the browser extension behavior.
- Identified a Base64-encoded string used within the extension:
  - `d3d3LmZhY2Vib29rLmNvbQ==`
- Decoded the Base64 string, revealing:
  - `www.facebook.com`
- Determined that the extension was redirecting users to a fake or misleading login page to capture credentials.
- Identified the domain used for data exfiltration:
  - `mo.elshaheedy.com`
- Observed that the extension accessed browser cookies, indicating potential session hijacking or credential theft.

---

## 3. Evidence / Indicators of Compromise (IOCs)

- Base64 Encoded URL:
  - `d3d3LmZhY2Vib29rLmNvbQ==`
- Decoded URL:
  - `www.facebook.com`
- Suspicious Domain:
  - `mo.elshaheedy.com`
- Data Accessed:
  - Browser cookies (session and authentication data)

---

## 4. Is it Malicious?

**True Positive**

This extension is malicious because:
- It impersonates a trusted service (ChatGPT)
- Uses encoded URLs to hide its behavior
- Redirects users to credential harvesting pages
- Exfiltrates sensitive data to an external domain
- Accesses cookies, enabling session hijacking

---

## 5. Recommended Actions

- Immediately uninstall the malicious browser extension
- Clear browser cookies and sessions
- Change all affected account passwords
- Perform a full system security scan
- Monitor network traffic for suspicious domains
- Educate users about installing only trusted extensions

---

## 6. Conclusion

The investigation confirms that the browser extension is malicious and was designed to steal user credentials and sensitive session data. Immediate remediation steps are required to prevent further compromise.
