# Git rebase flow

## ⛳ Benefits
 - simple work with dependent tasks
 - pretty history

## 🚦convention
- ❌ Merge commit
- ❌ Development process history
- ❌ commit without task
- 1️⃣ Task – 1️⃣ commit
- 1️⃣ Branch – 1️⃣ developer
- 1️⃣ Main branch
- ✅ Rebase
- ✅ Stateless release
- ✅ Rebase only task branches
- ✅ Atomic tasks

## 🛠 Tools
- ⚙️  Automatization
- 🏗 Decomposition
- 🚩 Feature flags
- 🔍 Testable changes
- 🔗 Backward compatibility

## Requirements

- Automated (or described) CI/CD process - possibility of seamless delivery of software

## Base concepts

1. Main branch always stable and represent current production state
2. Tasks should be decomposed to a small pieces as much as possible
3. Release master always build new `release branch` using cherry-piking
4. After release `master branch` is fast-forwarding to `release branch`

## Disadvantages

 - rebase dangerous, it easy to "shoot yourself in the foot"
