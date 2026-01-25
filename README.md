# Security-First AI Assistant Prompt

A comprehensive, production-grade system prompt for AI coding assistants that enforces security-first architecture, automated vulnerability detection, threat modeling, and zero-trust principles.

## 🎯 Overview

This prompt transforms AI assistants into **Principal Security Architects** with 15+ years of production experience, operating with security-first principles by default. It enforces automatic vulnerability detection, threat modeling, secure-by-default configurations, and comprehensive security practices across all code generation.

## ✨ Key Features

### 🔒 Security-First Architecture
- **Default Security Mode**: All backend outputs are security-first by default
- **Automated Vulnerability Detection**: Automatically scans for 11+ vulnerability types
- **Auto-Patching**: Immediately patches vulnerabilities found in code
- **Zero-Trust Architecture**: No implicit trust, explicit authentication everywhere

### 🛡️ Threat Modeling & Risk Analysis
- **Mandatory Threat Modeling**: Performs STRIDE-based threat modeling for all backends/APIs
- **Attack Surface Minimization**: Identifies and restricts unnecessary exposures
- **Performance Threat Modeling**: Treats performance as a security concern
- **Supply-Chain Security**: Analyzes dependencies for risks and maintenance status

### 🔍 Advanced Capabilities
- **JavaScript Reverse-Engineering**: Expert-level deobfuscation and analysis
- **GodMode**: Web-connected research mode with source verification
- **Legacy-Aware Refactoring**: Secure refactoring that preserves behavior
- **Observability & Logging**: Security-focused structured logging

### 📋 Code Quality & Architecture
- **Schema-First Validation**: Explicit schemas and DTO-based validation
- **Backward Compatibility Guardian**: Detects and warns about breaking changes
- **Architecture Decision Records (ADR)**: Documents significant decisions
- **Cognitive Load Optimization**: Prioritizes readability and maintainability

## 📖 Usage

### For Cursor IDE

1. Copy the contents of `prompt.txt`
2. Go to Cursor Settings → Rules for AI
3. Paste the prompt as a custom rule
4. The AI assistant will now operate with security-first principles

### For Other AI Assistants

1. Copy the contents of `prompt.txt`
2. Add it as a system prompt or custom instruction
3. Configure your AI assistant to use this prompt

## 🏗️ Architecture Principles

The prompt enforces:

```
architecture decisions → trust boundaries → attack surfaces → human factors
→ failure modes → mitigations → recovery → long-term survivability
```

### Core Modes

1. **Security-First Backend Mode** (Default: ON)
   - Never trust client input
   - Schema/DTO-based validation
   - Centralized error handling
   - Strict separation of concerns

2. **Automated Vulnerability Detection**
   - SQL/NoSQL/Command/Template Injection
   - XSS (stored/reflected/DOM)
   - CSRF, IDOR, Auth bypass
   - Broken access control
   - Mass assignment vulnerabilities
   - And more...

3. **Threat Modeling** (Mandatory)
   - Assets at risk
   - Trust boundaries
   - Threat actors
   - Attack surfaces
   - Abuse cases
   - Mitigations

4. **Zero-Trust Architecture**
   - No trusted network
   - No trusted service
   - Explicit authentication everywhere
   - Least-privilege by default

## 🚀 GodMode Feature

**GodMode** is a special web-connected research mode that:

- Accesses the internet for current information
- Performs ULTRATHINK-level analysis
- Generates high-leverage ideas and solutions
- Requires at least 3 independent reliable sources
- Provides Insight Maps, Opportunity Lists, and Top 3 Action Plans

**Activation Triggers:**
- User explicitly requests "GodMode"
- Time-sensitive queries (latest version, current price, CVE, etc.)
- Uncertain information with 10%+ recall risk

## 📊 Response Formats

### Default Mode
- Rationale (1 sentence)
- Secure & patched solution
- Threat Model Summary
- Design / Architecture Review
- ADR (if applicable)

### ULTRATHINK Mode
- Deep reasoning
- Full threat model
- Failure & abuse analysis
- Final hardened solution
- Improvement & resilience plan

## 🔐 Security Guarantees

- ✅ Never outputs knowingly vulnerable code
- ✅ Automatically patches vulnerabilities
- ✅ Validates all inputs
- ✅ Fails closed
- ✅ Never leaks internals in errors
- ✅ Secure-by-default configurations
- ✅ PII-aware logging and data handling

## 🛠️ Supported Technologies

- **PHP** (ULTRA LEVEL, modern + legacy)
- **Node.js**
- **Python** (ULTRA LEVEL)
- **JavaScript / TypeScript** (ULTRA PROFESSIONAL)

## 📝 Best Practices Enforced

- Schema-first / Contract-first architecture
- Configuration-as-code
- Observability & security logging
- Data privacy & PII compliance (GDPR-style)
- Incident response thinking
- Chaos engineering awareness
- Knowledge transfer optimization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is open source and available under the [MIT License](LICENSE) (or specify your preferred license).

## ⚠️ Disclaimer

This prompt is designed for security-focused development. While it significantly improves code security, it should be used as part of a comprehensive security strategy including:
- Regular security audits
- Penetration testing
- Code reviews
- Security training
- Incident response plans

## 🙏 Acknowledgments

Built with security-first principles and production experience in mind. Designed to help developers write more secure code by default.

---

**Remember**: Security is not a feature, it's a fundamental requirement. This prompt helps enforce that principle in every line of code generated.
