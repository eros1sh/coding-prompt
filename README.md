# 🚀 Ultra Professional Full-Stack System Prompt

> A comprehensive system prompt for AI assistants specializing in security-first, production-grade full-stack development with 15+ years of real-world expertise.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

## 📋 Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Technical Expertise](#technical-expertise)
- [Core Capabilities](#core-capabilities)
- [Security Features](#security-features)
- [Architecture Patterns](#architecture-patterns)
- [Usage](#usage)
- [Operation Modes](#operation-modes)
- [Response Formats](#response-formats)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This system prompt transforms AI assistants into **Principal-level Security Architects and Full-Stack Engineers** with deep expertise across modern web technologies, security practices, and architectural patterns.

### What Makes This Different?

- ✅ **Security-First by Default** - Every output includes threat modeling and vulnerability detection
- ✅ **Production-Ready Code** - Zero placeholders, copy-paste ready solutions
- ✅ **Zero Noise Policy** - No fluff, no repetition, just actionable solutions
- ✅ **Auto-Patching** - Automatically detects and fixes security vulnerabilities
- ✅ **Web-Connected Intelligence** - GodMode for real-time, verified information

## 🔑 Key Features

### 🛡️ Security Engineering
- Automated vulnerability detection & patching
- Mandatory threat modeling (STRIDE framework)
- Zero-trust architecture enforcement
- Attack surface minimization
- PII/GDPR compliance built-in

### 🎨 Frontend Excellence
- Modern React/Vue/Svelte architecture
- Core Web Vitals optimization (LCP, FID, CLS, INP)
- Advanced TypeScript patterns
- Accessibility (WCAG 2.2 AA/AAA)
- State management strategies (Zustand, Jotai, Redux)

### ⚙️ Backend Mastery
- Multi-language expertise (PHP, Node.js, Python)
- API design (REST, GraphQL, gRPC, WebSocket)
- Database optimization & query tuning
- Microservices & event-driven architecture
- Caching strategies & rate limiting

### 🔍 Advanced Capabilities
- JavaScript reverse-engineering & deobfuscation
- Chaos engineering awareness
- Performance threat modeling
- Supply-chain security analysis
- Architecture Decision Records (ADR)

## 💻 Technical Expertise

### Primary Languages (ULTRA LEVEL)
```
├── PHP          → Modern + Legacy, Laravel/Symfony ecosystems
├── Node.js      → Express, Fastify, NestJS, runtime internals
├── Python       → FastAPI, Django, async/await optimization
└── TypeScript   → ES2024+, advanced types, meta-programming
```

### Frontend Frameworks
```
├── React        → Hooks, Server Components, Concurrent Features
├── Vue          → Composition API, Reactivity internals
├── Svelte       → Runes, SvelteKit, compiler magic
└── Angular      → Signals, Standalone components
```

### Infrastructure & Tools
```
├── Containers   → Docker, Kubernetes, container security
├── IaC          → Terraform, Pulumi, CloudFormation
├── Cloud        → AWS, GCP, Azure (multi-cloud patterns)
├── CI/CD        → GitHub Actions, GitLab CI, Jenkins
└── Observability → OpenTelemetry, Prometheus, Grafana
```

## 🚨 Core Capabilities

### 1. Automated Vulnerability Detection

Automatically scans for and patches:
- ✅ SQL/NoSQL/Command Injection
- ✅ XSS (Stored, Reflected, DOM-based)
- ✅ CSRF & Clickjacking
- ✅ IDOR & Broken Access Control
- ✅ Mass Assignment vulnerabilities
- ✅ Insecure Deserialization
- ✅ Race Conditions & Logic Flaws

**Example:**
```typescript
// ❌ Vulnerable code detected
app.get('/user/:id', (req, res) => {
  db.query(`SELECT * FROM users WHERE id = ${req.params.id}`);
});

// ✅ Auto-patched version
app.get('/user/:id', async (req, res) => {
  // SECURITY FIX: Parameterized query to prevent SQL injection
  const userId = parseInt(req.params.id);
  if (isNaN(userId)) {
    return res.status(400).json({ error: 'Invalid user ID' });
  }
  
  const user = await db.query(
    'SELECT id, name, email FROM users WHERE id = $1',
    [userId]
  );
  res.json(user);
});
```

### 2. Mandatory Threat Modeling

Every backend/API response includes:
```markdown
## Threat Model Summary

**Assets at Risk:**
- User authentication tokens, PII, financial data

**Trust Boundaries:**
- Client ↔ API Gateway ↔ Microservices ↔ Database

**Key Threats & Mitigations:**
1. **Token Theft** → HttpOnly cookies + short expiration + refresh rotation
2. **IDOR** → Authorization checks on every resource access
3. **DoS** → Rate limiting (100 req/15min) + request size limits
```

### 3. Frontend Performance Optimization

Targets Core Web Vitals:
- **LCP** (Largest Contentful Paint): < 2.5s
- **FID** (First Input Delay): < 100ms
- **CLS** (Cumulative Layout Shift): < 0.1
- **INP** (Interaction to Next Paint): < 200ms

**Techniques:**
```typescript
// Code splitting
const Dashboard = lazy(() => import('./Dashboard'));

// Prefetching
<link rel="prefetch" href="/dashboard-chunk.js" />

// Image optimization
<img 
  src="hero.webp"
  srcset="hero-320w.webp 320w, hero-640w.webp 640w"
  sizes="(max-width: 320px) 280px, 640px"
  loading="lazy"
  alt="Hero image"
/>

// Virtual scrolling for large lists
import { FixedSizeList } from 'react-window';
```

### 4. JavaScript Reverse Engineering

Expert-level deobfuscation capabilities:
```javascript
// Before: Obfuscated
(function(_0x4d8f,_0x2a91){var _0x51c2=function(_0x3f12){while(--_0x3f12){_0x4d8f['push'](_0x4d8f['shift']());}};_0x51c2(++_0x2a91);}(_0x2a91,0x1a3));

// After: Cleaned & Analyzed
// SECURITY ANALYSIS: This code establishes a WebSocket connection
// to an external domain and sends user keystrokes.
// RISK: High - Potential keylogger / data exfiltration
function setupWebSocket(url) {
  const ws = new WebSocket(url);
  ws.onopen = () => {
    document.addEventListener('keydown', (e) => {
      ws.send(JSON.stringify({ key: e.key, timestamp: Date.now() }));
    });
  };
}
```

## 🎮 Operation Modes

### 1. DEFAULT MODE
Fast, focused, production-ready solutions.

**Output:**
```markdown
**Rationale:** [1 sentence explanation]

**Solution:** [Complete code]

**Threat Model:** [STRIDE analysis]

**Architecture Review:** [Design decisions]
```

### 2. ULTRATHINK MODE
Deep analysis with comprehensive threat modeling.

**Activated by:** User says "ULTRATHINK"

**Output includes:**
- Deep reasoning & edge case analysis
- Full STRIDE threat model
- Failure mode & chaos scenarios
- Hardened solution with all mitigations
- Long-term improvement plan

### 3. GODMODE
Web-connected intelligence with real-time verification.

**Activated by:** 
- User says "GodMode"
- Time-sensitive queries ("latest", "current", "today")
- Requests about new/niche topics

**Capabilities:**
- ✅ Web search for current information
- ✅ Multi-source verification
- ✅ CVE/security advisory lookup
- ✅ Real-time library version checking
- ✅ Idea generation engine

**Output includes:**
```markdown
**Web-Verified Findings:** [with sources]

**Insight Map:** 5-10 key learnings

**Opportunity List:** 8-12 actionable ideas
  - Security improvements
  - Performance optimizations
  - Product enhancements
  - DX improvements

**Top 3 Plan:**
1. [High-impact idea] - Impact: High | Effort: Low
   First 48h: [concrete steps]
```

## 📐 Architecture Patterns

### Security Architecture
```
┌─────────────────────────────────┐
│   Input Validation Layer        │ ← Zod, Joi, class-validator
├─────────────────────────────────┤
│   Authentication Layer          │ ← JWT, OAuth, Session
├─────────────────────────────────┤
│   Authorization Layer           │ ← RBAC, ABAC, Policies
├─────────────────────────────────┤
│   Business Logic Layer          │ ← Pure, testable functions
├─────────────────────────────────┤
│   Data Access Layer             │ ← Parameterized queries
├─────────────────────────────────┤
│   Security Logging & Monitoring │ ← Audit trails, alerts
└─────────────────────────────────┘
```

### Frontend Architecture
```
Component Layer (Atomic Design)
    ↓
State Management (Zustand, Jotai)
    ↓
Data Layer (React Query, SWR)
    ↓
API Client (Axios, Fetch + interceptors)
```

### Testing Pyramid
```
        E2E (10%) - Playwright, Cypress
       ↗              ↖
  Integration (30%) - Testing Library
     ↗              ↖
Unit Tests (60%) - Vitest, Jest
```

## 🚀 Usage

### Installation

Simply copy the system prompt to your AI assistant configuration:

1. Copy the contents of `system-prompt-v2.md`
2. Paste into your AI assistant's system prompt field
3. Start asking questions!

### Basic Examples

#### Example 1: Secure API Endpoint
```
User: Create a secure user registration endpoint in Node.js with Express
```

**Response includes:**
- ✅ Input validation (email, password strength)
- ✅ Password hashing (Argon2id)
- ✅ Rate limiting
- ✅ CSRF protection
- ✅ SQL injection prevention
- ✅ Threat model
- ✅ Security logging

#### Example 2: Frontend Performance
```
User: Optimize this React component that renders 10,000 items
```

**Response includes:**
- ✅ Virtual scrolling implementation
- ✅ Memoization strategies
- ✅ Code splitting
- ✅ Performance metrics
- ✅ Lighthouse score impact analysis

#### Example 3: Security Audit
```
User: Review this authentication system for vulnerabilities
```

**Response includes:**
- ✅ Automated vulnerability detection
- ✅ STRIDE threat model
- ✅ Patched code
- ✅ Attack surface analysis
- ✅ Compliance check (GDPR, OWASP)

#### Example 4: GodMode Research
```
User: GodMode - What are the latest critical CVEs for React and Next.js?
```

**Response includes:**
- ✅ Web-verified CVE listings with sources
- ✅ Severity assessment
- ✅ Mitigation strategies
- ✅ Upgrade recommendations
- ✅ Impact analysis for your stack

## 📊 Response Formats

### Security Finding Format
```markdown
🔴 CRITICAL: SQL Injection vulnerability detected

**Location:** `app/routes/users.js:45`

**Issue:** User input directly concatenated into SQL query

**Exploit:** `id=1' OR '1'='1`

**Fix Applied:**
- Switched to parameterized queries
- Added input validation
- Implemented prepared statements

**Testing:** Added security test case
```

### Architecture Decision Record
```markdown
## ADR-001: Choosing Zustand over Redux

**Context:**
Team struggling with Redux boilerplate, app state is simple.

**Decision:**
Migrate to Zustand for global state management.

**Alternatives:**
1. Redux Toolkit - Rejected: Still too much boilerplate
2. Context API - Rejected: Performance issues with frequent updates
3. Jotai - Considered: Chose Zustand for DevTools integration

**Consequences:**
✅ 60% less boilerplate code
✅ Better TypeScript support
✅ Easier onboarding
⚠️ Smaller ecosystem than Redux
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Areas for Improvement
- [ ] Additional language-specific patterns (Go, Rust, Java)
- [ ] Cloud-native security patterns
- [ ] GraphQL security best practices
- [ ] Mobile app security (React Native, Flutter)
- [ ] DevSecOps pipeline examples
- [ ] Compliance frameworks (SOC2, HIPAA, PCI-DSS)

### Contribution Guidelines
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-pattern`)
3. Add your improvements with examples
4. Ensure security best practices are maintained
5. Submit a Pull Request

### What We're Looking For
- ✅ Real-world production examples
- ✅ Security-first patterns
- ✅ Performance optimization techniques
- ✅ Accessibility improvements
- ✅ Testing strategies
- ✅ Documentation enhancements

## 📚 Resources

### Security
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)
- [CWE Top 25](https://cwe.mitre.org/top25/)

### Frontend
- [web.dev](https://web.dev/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [React Documentation](https://react.dev/)

### Backend
- [Node.js Best Practices](https://github.com/goldbergyoni/nodebestpractices)
- [Twelve-Factor App](https://12factor.net/)
- [API Security Checklist](https://github.com/shieldfy/API-Security-Checklist)

## ⚖️ License

MIT License - feel free to use this prompt for personal or commercial projects.

## 🙏 Acknowledgments

Built with expertise from:
- 15+ years of production engineering
- Security research & penetration testing
- Open-source contribution experience
- Enterprise architecture consulting

---

## 💬 Support & Feedback

- **Issues:** Open a GitHub issue
- **Discussions:** Use GitHub Discussions for questions
- **Twitter:** Share your experience with #UltraSystemPrompt

---

<div align="center">

**⭐ Star this repo if it helped you build more secure, performant applications!**

Made with ❤️ by developers, for developers

</div>
