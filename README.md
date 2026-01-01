# 🔒 Web Security Labs

![Security](https://img.shields.io/badge/Security-Testing-red)
![Labs](https://img.shields.io/badge/Labs-2-blue)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

> A comprehensive collection of hands-on cybersecurity labs focused on web application security testing, vulnerability assessment, and ethical hacking techniques.

⚠️ **DISCLAIMER:** All labs and techniques documented here are for educational and authorized testing purposes only. Only perform security testing on systems you own or have explicit written permission to test. Unauthorized access to computer systems is illegal.

---

## 📚 About This Repository

This repository contains practical cybersecurity labs completed as part of the **ParoCyber Ethical Hacking Training Program**. Each lab provides detailed documentation, screenshots, real-world scenarios, and hands-on demonstrations of security testing techniques used by penetration testers and security professionals.

### 🎯 Purpose

- **Learn by doing** — Practical, hands-on security testing exercises
- **Professional documentation** — Industry-standard reporting and analysis
- **Real-world skills** — Techniques used in actual penetration testing engagements
- **Educational resource** — Reference materials for cybersecurity students and professionals

---

## 🧪 Available Labs

### 1. 🔍 [OWASP ZAP Web Vulnerability Scanner Lab](owasp-zap-lab/)

**Focus:** Web Application Security Testing & Vulnerability Assessment

Learn how to perform automated security scanning using OWASP ZAP (Zed Attack Proxy), one of the most popular open-source web application security scanners.

**Topics Covered:**
- Automated vulnerability scanning
- Active and passive scanning techniques
- Spidering web applications
- Analyzing security alerts and vulnerabilities
- CVE identification and exploitation
- Security header analysis
- Professional vulnerability reporting

**Key Findings:**
- 🔴 2 High-risk vulnerabilities (including Remote Code Execution)
- 🟠 5 Medium-risk vulnerabilities
- 🟡 5 Low-risk vulnerabilities
- Complete remediation recommendations

**Skills Developed:**
- Web application security testing
- Vulnerability classification and prioritization
- Security report generation
- Remediation planning

[📖 View Full Lab Documentation →](owasp-zap-lab/README.md)

---

### 2. 🔐 [Password Cracking Lab](password-cracking-lab/)

**Focus:** Password Security & Hash Cracking Techniques

Explore password cracking methodologies using industry-standard tools like Hashcat and John the Ripper to understand password vulnerabilities and defensive strategies.

**Topics Covered:**
- Password hashing fundamentals (MD5, SHA, bcrypt)
- Dictionary attacks using wordlists
- Hashcat GPU-accelerated cracking
- John the Ripper techniques
- Password security analysis
- Defensive recommendations

**Key Results:**
- 100% success rate cracking MD5 hashes
- Comparative analysis of Hashcat vs John the Ripper
- Performance metrics and speed analysis
- Real-world security implications

**Skills Developed:**
- Password auditing techniques
- Hash identification and cracking
- Tool selection and optimization
- Security awareness training

[📖 View Full Lab Documentation →](password-cracking-lab/README.md)

---

## 🛠️ Tools & Technologies

| Tool | Version | Purpose |
|------|---------|---------|
| **OWASP ZAP** | v2.13.0 | Web application security scanner |
| **Hashcat** | v6.2.6 | GPU-accelerated password cracker |
| **John the Ripper** | 1.9.0-jumbo-1 | CPU-based password cracker |
| **Kali Linux** | Latest | Primary penetration testing platform |
| **DVWA** | Latest | Vulnerable web application for testing |
| **rockyou.txt** | 14.3M passwords | Dictionary wordlist |

---

## 🖥️ Lab Environment

All labs were conducted in a controlled, isolated environment:

```
┌─────────────────────────────────────────┐
│         Virtualized Environment         │
├─────────────────────────────────────────┤
│  Attacker: Kali Linux (VirtualBox)     │
│  Target: DVWA (Vulnerable Web App)      │
│  Network: Isolated virtual network      │
│  Date: January 2026                     │
└─────────────────────────────────────────┘
```

**Environment Specifications:**
- **Hypervisor:** VirtualBox
- **Attacker Platform:** Kali Linux (Latest)
- **Target Applications:** DVWA, custom test environments
- **Network:** Isolated NAT/Host-only networking
- **Security:** No production systems involved

---

## 📖 Learning Outcomes

### Technical Skills

✅ Web application vulnerability assessment  
✅ Automated security scanning and analysis  
✅ Password cracking and hash analysis  
✅ Security tool proficiency (ZAP, Hashcat, John)  
✅ CVE research and exploitation  
✅ Vulnerability remediation strategies  
✅ Professional security report writing  

### Cybersecurity Concepts

✅ OWASP Top 10 vulnerabilities  
✅ Web security best practices  
✅ Defense-in-depth principles  
✅ Password security fundamentals  
✅ Cryptographic hash functions  
✅ Attack vectors and threat modeling  
✅ Risk assessment and prioritization  

---

## 🚀 Getting Started

### Prerequisites

To replicate these labs, you'll need:

1. **VirtualBox or VMware** — For running Kali Linux
2. **Kali Linux ISO** — Download from [kali.org](https://www.kali.org/get-kali/)
3. **Vulnerable Applications:**
   - DVWA (Damn Vulnerable Web Application)
   - Or other intentionally vulnerable web apps (bWAPP, Mutillidae, WebGoat)
4. **Basic Linux Knowledge** — Command line familiarity
5. **Security Training Account** — Optional: Hack The Box, TryHackMe for practice

### Installation Steps

1. **Install VirtualBox:**
   ```bash
   # Download from: https://www.virtualbox.org/
   ```

2. **Set Up Kali Linux:**
   ```bash
   # Download Kali Linux ISO
   # Create a new VM in VirtualBox
   # Install Kali with at least 4GB RAM and 40GB disk
   ```

3. **Update Tools:**
   ```bash
   sudo apt update && sudo apt upgrade -y
   sudo apt install zaproxy hashcat john -y
   ```

4. **Download Wordlists:**
   ```bash
   # Extract rockyou.txt if compressed
   sudo gunzip /usr/share/wordlists/rockyou.txt.gz
   ```

### Quick Start

1. Clone this repository for reference materials:
   ```bash
   git clone https://github.com/yourusername/Web-Security-Labs.git
   cd Web-Security-Labs
   ```

2. Choose a lab and follow the detailed README in each directory

3. Set up your target environment (DVWA or other vulnerable apps)

4. Follow the step-by-step instructions in each lab

---

## 📋 Lab Structure

Each lab directory contains:

```
lab-name/
├── README.md          # Comprehensive lab documentation
├── screenshots/       # Visual evidence and step-by-step images
│   ├── setup.png
│   ├── results.png
│   └── ...
└── resources/         # Optional: scripts, configs, samples
```

### Documentation Standards

All labs include:

- ✅ Clear objectives and learning goals
- ✅ Step-by-step instructions with commands
- ✅ Screenshots for visual guidance
- ✅ Detailed explanations of techniques
- ✅ Results analysis and interpretation
- ✅ Security recommendations
- ✅ References and further reading

---

## 🔐 Security & Ethics

### Ethical Guidelines

These labs teach powerful security testing techniques that must be used responsibly:

1. **Permission Required** — Never test systems you don't own or have written authorization to test
2. **Legal Compliance** — Follow all applicable laws and regulations
3. **Controlled Environment** — Use isolated virtual machines for practice
4. **No Harm** — Do not use these techniques to cause damage or disruption
5. **Professional Conduct** — Maintain ethical standards in all security work

### Legal Notice

The techniques demonstrated in these labs are for:

- ✅ Educational purposes
- ✅ Authorized penetration testing
- ✅ Personal lab environments
- ✅ Bug bounty programs (with proper authorization)
- ✅ Security research (with consent)

**NOT for:**

- ❌ Unauthorized access to systems
- ❌ Malicious hacking or damage
- ❌ Privacy violations
- ❌ Any illegal activities

---

## 🎓 Certification & Training

These labs were completed as part of:

**ParoCyber Ethical Hacking Training Program**

Recommended certifications and training paths:

| Certification | Focus | Level |
|---------------|-------|-------|
| **CEH** | Certified Ethical Hacker | Intermediate |
| **OSCP** | Offensive Security Certified Professional | Advanced |
| **PNPT** | Practical Network Penetration Tester | Intermediate |
| **eWPT** | eLearnSecurity Web Application Penetration Tester | Intermediate |
| **GWAPT** | GIAC Web Application Penetration Tester | Advanced |

**Additional Learning Platforms:**

- [TryHackMe](https://tryhackme.com/) — Guided cybersecurity learning
- [Hack The Box](https://www.hackthebox.com/) — Penetration testing practice
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free web security training
- [OWASP Projects](https://owasp.org/) — Web application security resources

---

## 🤝 Contributing

While this is primarily a personal learning repository, contributions are welcome:

1. **Report Issues** — Found an error or outdated information? Open an issue
2. **Suggest Improvements** — Have ideas for better explanations? Submit a pull request
3. **Share Your Labs** — Add your own security labs with proper documentation
4. **Fix Typos** — Help improve the documentation quality

### Contribution Guidelines

- Follow the existing documentation format
- Include screenshots for visual steps
- Test all commands and procedures
- Add ethical disclaimers where appropriate
- Reference sources and tools properly

---

## 📚 Additional Resources

### OWASP Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)

### Tool Documentation

- [OWASP ZAP Documentation](https://www.zaproxy.org/docs/)
- [Hashcat Wiki](https://hashcat.net/wiki/)
- [John the Ripper Documentation](https://www.openwall.com/john/doc/)

### Security References

- [MITRE ATT&CK Framework](https://attack.mitre.org/)
- [CVE Database](https://cve.mitre.org/)
- [CWE - Common Weakness Enumeration](https://cwe.mitre.org/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

### Vulnerable Applications for Practice

- [DVWA - Damn Vulnerable Web Application](https://github.com/digininja/DVWA)
- [WebGoat](https://owasp.org/www-project-webgoat/)
- [bWAPP](http://www.itsecgames.com/)
- [Mutillidae II](https://github.com/webpwnized/mutillidae)

---

## 🐛 Known Issues

### Password Cracking Lab
- ⚠️ **Missing Screenshot**: The `john-cracked.png` screenshot referenced in the README may be missing from the screenshots directory
- **Status**: Non-critical - Results are documented in text format
- **Workaround**: Refer to the detailed text output in the documentation

### General Notes
- Screenshots are from a specific lab environment; your results may vary based on your setup
- Tool versions may differ; always use the latest stable versions
- Some commands may require modification based on your specific environment

---

## 📅 Roadmap

### Upcoming Labs

- [ ] SQL Injection Lab — Database exploitation techniques
- [ ] Cross-Site Scripting (XSS) Lab — Client-side attack vectors
- [ ] Network Scanning with Nmap — Host and service discovery
- [ ] Metasploit Framework Lab — Exploitation and post-exploitation
- [ ] Wireless Security Lab — WiFi penetration testing
- [ ] Social Engineering Lab — Human-based attack vectors
- [ ] Mobile Application Security — Android/iOS testing
- [ ] API Security Testing — REST/GraphQL vulnerabilities

### Future Enhancements

- Video walkthroughs for each lab
- Interactive Jupyter notebooks
- Docker containers for quick lab setup
- Automated lab deployment scripts
- Additional real-world case studies

---

## 📝 Changelog

### Version 1.0.0 (January 2026)

**Added:**
- ✅ OWASP ZAP Web Vulnerability Scanner Lab
- ✅ Password Cracking Lab (Hashcat & John the Ripper)
- ✅ Comprehensive documentation for both labs
- ✅ Screenshots and visual guides
- ✅ Root-level README with repository overview
- ✅ MIT License

---

## 👤 Author

**Aliu Tijani**  
Cybersecurity Enthusiast | Ethical Hacking Student

- 🔗 **LinkedIn:** [linkedin.com/in/aliutijani](https://www.linkedin.com/in/aliutijani)
- 💻 **GitHub:** [github.com/aliu2211](https://github.com/aliu2211)
- 📧 **Email:** Contact via LinkedIn

### About Me

I'm a cybersecurity enthusiast currently training in ethical hacking and penetration testing. This repository showcases my journey in learning web application security, vulnerability assessment, and defensive security practices. I'm passionate about hands-on learning and practical security research.

**Interests:**
- Web Application Security
- Penetration Testing
- Security Automation
- Cloud Security
- Threat Intelligence

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### MIT License Summary

- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ✅ Private use
- ❌ Liability
- ❌ Warranty

---

## ⭐ Support

If you find these labs helpful:

- ⭐ **Star this repository** to show your support
- 🔄 **Share** with others learning cybersecurity
- 💬 **Provide feedback** through issues or discussions
- 🤝 **Connect** on LinkedIn for networking

---

## 🙏 Acknowledgments

- **ParoCyber** — For providing excellent ethical hacking training
- **OWASP** — For creating and maintaining incredible security tools and resources
- **Kali Linux Team** — For the ultimate penetration testing platform
- **Security Community** — For sharing knowledge and best practices
- **Open Source Contributors** — For developing the amazing tools used in these labs

---

## 📞 Contact

Have questions, suggestions, or want to collaborate?

- **LinkedIn:** [Aliu Tijani](https://www.linkedin.com/in/aliutijani)
- **GitHub Issues:** Use the [Issues](https://github.com/yourusername/Web-Security-Labs/issues) tab for technical questions
- **Discussions:** Start a [Discussion](https://github.com/yourusername/Web-Security-Labs/discussions) for general topics

---

<div align="center">

**⚠️ Remember: With great power comes great responsibility. Use these skills ethically and legally. ⚠️**

---

Made with ❤️ by cybersecurity enthusiasts, for cybersecurity learners.

*Last Updated: January 2026*

</div>
