---
name: 💡 Feature Request
about: Suggest an idea for the Me2em protocol or SDK  ← было: description
title: '[Feature]: '
labels: ['enhancement', 'triage']
assignees: []
---

## 🎯 Problem Statement

<!-- What problem are you trying to solve? Describe the user story or use case. -->

> As a [role], I want to [goal], so that [benefit].

**Example**:
> As a developer building an IoT app, I want to derive child Handles programmatically, so that I can provision devices without manual seed entry.

---

## 🚀 Proposed Solution

<!-- Describe the feature you'd like to see. Be as specific as possible. -->

### API Design (if applicable)

```typescript
// Example: what would the new API look like?
import { Identity } from '@me2em/protocol-core';

const identity = await Identity.fromSeed(seed);
// Your proposed addition:
const childHandle = await identity.deriveSubHandle('device-001', {
  metadata: { type: 'sensor', location: 'warehouse-A' }
});
```

### Protocol Changes (if applicable)

<!-- If this affects the protocol spec, describe:
- New message types
- Changes to Handle/Session structure
- Backward compatibility considerations
-->

---

## 🔍 Alternatives Considered

<!-- What other approaches did you consider? Why is this proposal better? -->

| Alternative | Pros | Cons | Why not chosen |
|-------------|------|------|---------------|
|             |      |      |               |
|             |      |      |               |

---

## 🧪 Use Cases

<!-- List concrete scenarios where this feature would be valuable. -->

1. **IoT Device Provisioning**: Bulk-create Handles for sensors with metadata tags
2. **Enterprise SSO**: Allow employees to generate department-scoped Handles
3. **Privacy Preservation**: Let users create one-time Handles for untrusted apps

---

## ⚖️ Impact Assessment

| Aspect | Assessment |
|--------|-----------|
| **Breaking Change?** | <!-- Yes / No / Unsure --> |
| **Performance Impact** | <!-- e.g., "Adds ~5ms to Handle derivation" --> |
| **Security Implications** | <!-- e.g., "Requires new key derivation path; needs crypto review" --> |
| **Backward Compatibility** | <!-- e.g., "Old clients ignore new metadata fields" --> |
| **Documentation Needed** | <!-- e.g., "Update SDK guide + protocol spec section 4.2" --> |

---

## 📚 References

<!-- Link to related discussions, research, or external standards. -->

- [Discussion: Multi-tenant Handle management](https://github.com/me2em-org/me2em-protocol/discussions/__)
- [W3C DID Core Spec](https://www.w3.org/TR/did-core/)
- [NIST SP 800-56C: Key Derivation](https://csrc.nist.gov/pubs/sp/800/56/c/final)

---

### ✅ Before Submitting

- [ ] I searched [existing discussions](https://github.com/me2em-org/me2em-protocol/discussions) and confirmed this idea hasn't been proposed
- [ ] I described the problem clearly, not just the solution
- [ ] I considered security and privacy implications
- [ ] I'm willing to help implement or test this feature (optional)

> 💡 **Tip**: For major changes, consider starting a [Discussion](https://github.com/me2em-org/me2em-protocol/discussions) first to gather community feedback before opening a formal issue.
