# 🔒 Security Policy - Kitchen Safety Rules

> *"A safe kitchen is a happy kitchen. Same goes for code!"*

## 🍳 Supported Versions

Like recipes, only the **latest version** gets all the safety updates:

| Version | Supported | Kitchen Status |
|---------|-----------|----------------|
| Latest (main branch) | ✅ | 🔥 Hot & Fresh |
| Older forks | ❌ | 🥶 Cold leftovers |

**Always use the latest version** from the `main` branch for the safest experience.

---

## 🚨 Reporting a Vulnerability

Found a security issue? **Don't post it publicly!** Follow these steps:

### 📝 How to Report

1. **Open a Draft Security Advisory** on GitHub
   - Go to: `Repository → Security → Advisories → New draft`
   - Or use this [direct link](https://github.com/realmg51-cpu/KotlinCookBook/security/advisories/new)

2. **Include these details:**
   - What recipe/file has the issue?
   - How can someone reproduce it?
   - What's the potential impact?
   - (Optional) Suggested fix

3. **Wait for response** (within 48 hours)

### 🔐 What happens next?

| Step | Action | Time |
|------|--------|------|
| 1 | Acknowledge receipt | 24 hours |
| 2 | Investigate & validate | 3-5 days |
| 3 | Fix (if needed) | 7-10 days |
| 4 | Release patch | After fix |
| 5 | Public disclosure | After patch |

---

## 🛡️ What We Consider a Vulnerability

### 🔴 Critical (Report immediately)
- Code execution vulnerabilities in recipes
- Malicious code in examples
- Exposed secrets or API keys
- Path traversal issues

### 🟡 Moderate
- Infinite loops that could freeze the JVM
- Resource exhaustion (memory/CPU)
- Incorrect null safety that could cause crashes

### 🟢 Low (Not a vulnerability)
- Typos in comments
- Style guide violations
- Non-working examples (please open a regular Issue)

---

## 🧪 Safe by Design

This cookbook follows **safe coding practices**:

```kotlin
// ✅ Good: Safe operations
val safe = input?.let { it } ?: "default"

// ❌ Never: Unsafe operations in examples
// Runtime.getRuntime().exec("rm -rf /")

What we guarantee:

· ✅ All recipes are read-only - they don't modify your system
· ✅ No external network calls unless explicitly shown
· ✅ No file system writes without warning
· ✅ All examples use safe Kotlin idioms

---

📦 Dependency Safety

This project has minimal dependencies:

Component Version Security Notes
Kotlin Compiler 2.3.20+ Official security advisories
Docker (optional) Latest Docker security

No third-party libraries - just pure Kotlin!

---

🐳 Docker Security

If using Docker:

```bash
# ✅ Safe way to run
docker run --rm -it kotlincookbook kotlin recipe.kt

# ⚠️ Don't run with extra privileges
# docker run --privileged kotlincookbook ...  # NOT recommended
```

---

## 🔐 Reporting Process (Kitchen Analogy)

```
You find a spoiled ingredient
        ↓
Tell the head chef privately (Security Advisory)
        ↓
Chef investigates (48 hours)
        ↓
If confirmed → Fix the recipe
        ↓
New safe version released
        ↓
You get credited (if you want!)
```

---

## ✨ Responsible Disclosure

We follow responsible disclosure:

· Report privately first
· Give us time to fix
· Don't share exploits publicly
· We'll credit you in the release notes

---

## 📜 Security Hall of Fame

Researchers who helped make this cookbook safer:

Name Issue Fix
Your name here Found something? Report it!

---

## 🆘 Getting Help

Question Where to ask
Is this a security issue? Open a Discussion first
I found something sensitive Use Security Advisory
General safety questions Issues with question label

---

## ⚖️ License & Liability

This project is under Apache 2.0 License.

Disclaimer: This is an educational cookbook. While we strive for safety, always review code before running it, especially if you modified it!

---

## 🔄 Updates

This policy is reviewed:

· 📅 Quarterly (or after major changes)
· 📧 Announcements via GitHub Security tab

Last updated: April 2026

---

"A safe kitchen is the first ingredient of a great meal. Stay safe, stay curious!" 🍳

Report vulnerabilities responsibly. Protect the kitchen! 🔒
