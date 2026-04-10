# QUICK BUILD GUIDE

## 🚀 Build NanoBrowser Specialization

### Prerequisites
- Node.js (v18+)
- pnpm (`npm install -g pnpm`)

### Windows Build Commands

Open PowerShell or WSL in the nanobrowser-specialized folder:

```bash
# 1. Install dependencies
pnpm install

# 2. Build the extension
pnpm build

# 3. The extension will be in:
#    dist/ folder
```

### Load in Chrome

1. Open Chrome → `chrome://extensions/`
2. Enable "Developer mode" (toggle top-right)
3. Click "Load unpacked"
4. Select the `dist/` folder
5. Done!

---

## 📁 Folder Location

```
C:\Users\User 7\nanobrowser-specialized\dist
```

Load THIS folder in Chrome (not the parent folder).

---

## 🧪 Test It Works

After loading:

1. Click extension icon (NanoBrowser/SigmaBrowser)
2. Side panel opens
3. Configure API keys in Settings
4. Navigate to any webpage
5. Type a command like: "Find all multiple choice questions on this page"
6. The specialized agents will activate!

---

## 🔧 Available Specialized Agents

- **MathSolver Agent** - Detects and solves math problems
- **MultipleChoice Agent** - Handles MC questions with AI
- **Navigator Agent** (original) - DOM interactions
- **Planner Agent** (original) - Task planning

---

## ⚙️ Configure API Keys

Click Settings (⚙️) in the side panel:

1. **LLM Provider**: Choose your provider
2. **API Key**: Enter your key
3. **Model Selection**: Assign models to agents
4. **Save**

Recommended:
- **MathSolver**: Use Claude or GPT-4
- **MultipleChoice**: Use Claude Opus or GPT-4 Turbo
- **Navigator**: GPT-3.5 Turbo (fast)
- **Planner**: Claude Opus (reasoning)

---

## 🧪 Test Pages

After building, test with:

**Math Test:**
- Open: `test-local.html` (from old SigmaBrowser)
- Or create simple math pages

**Multiple Choice Test:**
- Open: `test-local.html`
- Or any quiz platform (Canvas, Blackboard, etc.)

---

## 🐛 If Build Fails

```bash
# Clean everything
pnpm clean

# Reinstall
pnpm install

# Rebuild
pnpm build
```

---

## 📊 What You Get

✅ Full NanoBrowser functionality (browser automation)
✅ Math problem solving agent
✅ Multiple choice analysis agent
✅ Multi-step task handling
✅ Vision support for image-based questions
✅ All original NanoBrowser features

---

## 🎓 Next Steps

1. Build using commands above
2. Load `dist/` folder in Chrome
3. Configure API keys
4. Test on real assignments
5. Profit! 🎉
