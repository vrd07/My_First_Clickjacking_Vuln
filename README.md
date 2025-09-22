🔐 Clickjacking Exploit Demo

📁 Files

    clickjacking-demo.html - Live exploit demonstration

🎯 What This Does

Shows how missing security headers can make websites vulnerable to clickjacking attacks.
⚡ Quick Start

    Download clickjacking-demo.html

    Open in any web browser

    Watch the exploit in action

🔍 The Vulnerability

Missing Security Headers:

    X-Frame-Options - Allows embedding in iframes

    Content-Security-Policy - No frame protection

🎭 The Exploit
```
html

<iframe src="https://vulnerable-site.com"></iframe>
```

Impact: Attackers can overlay fake UI elements, tricking users into clicking hidden buttons.
```
🛡️ The Fix

Add to your server headers:
text

X-Frame-Options: DENY
Content-Security-Policy: frame-ancestors 'none'
```

📸 Demo Screenshots

    Fake login page with transparent iframe

    Victim site loads seamlessly inside

    Red border highlights the exploit area

⚠️ Legal Notice

Only test on websites you own or have permission to test. Unauthorized testing is illegal.
📚 Use Cases

    Security education

    Penetration testing practice

    Developer security awareness

Test responsibly! 🔒
