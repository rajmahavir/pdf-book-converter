# AI Quick Reference - PDF Book Converter

> **CRITICAL**: Read this BEFORE making ANY changes!

## ⚡ TL;DR - Do This, Not That

| ✅ DO | ❌ DON'T |
|-------|----------|
| Changes < 100 lines | Changes > 100 lines |
| One feature at a time | Multiple features at once |
| Test in file:// protocol | Assume web APIs work |
| Keep existing patterns | Refactor working code |
| Add validation first | Add UI themes first |
| In-memory state only | Use localStorage |

## 🚨 INSTANT FAIL CONDITIONS

```
❌ localStorage.setItem()     → FAILS in file:// protocol
❌ sessionStorage.setItem()   → FAILS in file:// protocol
❌ 300+ line changes          → TOO COMPLEX, will break
❌ Dark mode with CSS vars    → FAILED before (commit 4fdcfad)
❌ Changing window.changePage → BREAKS onclick handlers
```

## ✅ SAFE TO ADD

```
✅ File validation (size, type)
✅ Error message improvements
✅ Responsive scaling
✅ Warning messages (yellow)
✅ SRI hashes on <script> tags
✅ Better error context
✅ Canvas scaling calculations
```

## 📊 Track Record

### Failed Attempt (4fdcfad)
- 302 insertions, 41 deletions
- Dark mode + Progress bar + Keyboard shortcuts
- **Result**: User reverted ❌

### Successful Attempt (f1986fb)
- 60 insertions, 11 deletions
- File validation + Warnings + Scaling + SRI
- **Result**: Working ✅

## 🎯 Implementation Formula

1. **Pick ONE feature** (not three)
2. **< 100 lines** changed
3. **No browser storage** (localStorage/sessionStorage)
4. **Test file://** open directly
5. **Keep patterns** (don't refactor)
6. **Commit & Push**

## 📁 Critical Files

- `pdf-converter-standalone.html` - Main file (edit carefully)
- `README.md` - Update when features added
- `.ai-instructions.md` - Full guidelines (read if unsure)
- `.env.ai-config` - Config constraints

## 🔍 Before You Code - Ask:

1. Does this use localStorage? → ❌ **STOP**
2. Is this > 100 lines? → ❌ **SIMPLIFY**
3. Does it work in file://? → ✅ **PROCEED**
4. Is it Phase 1 or 2? → ✅ **SAFE**
5. Did I test it? → ✅ **COMMIT**

## 🎓 Key Lesson

**Small working changes > Large broken changes**

---

📖 Full details: `.ai-instructions.md`
⚙️ Config: `.env.ai-config`
