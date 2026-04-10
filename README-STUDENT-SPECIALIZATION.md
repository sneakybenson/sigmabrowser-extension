# NanoBrowser - Student Specialization

**AI-powered browser automation specialized for academic tasks**

🎓 **Alpha Release** - Specialized fork of NanoBrowser for math assignments, multiple choice, and multi-step academic workflows.

---

## 🎯 Specialized Features

### For Math Assignments
- **MathSolver Agent**: Automatically detects and solves:
  - Arithmetic problems (+, -, *, /, ^, √)
  - Algebra (equations, simplification)
  - Trigonometry (sin, cos, tan)
  - Calculus (derivatives, integrals)
  - Word problems with step-by-step solutions

### For Multiple Choice
- **MultipleChoice Agent**: AI-powered question analysis:
  - Detects radio buttons and checkboxes
  - Analyzes question text with AI
  - High-confidence answer selection (>85%)
  - Batch processing of multiple questions
  - Vision fallback for image-based questions

### For Complex Tasks
- **Multi-Step Workflows**: Handle conditional tasks
  - "If X, then Y, else Z"
  - Sequential problem solving
  - Context-aware decision making
  - State management across steps

---

## 🚀 Why This Specialization?

Built on top of **NanoBrowser** (open-source AI web automation):

- ✅ **Working Foundation**: Proven multi-agent system
- ✅ **No Reinventing**: Uses existing browser automation
- ✅ **Specialized Agents**: Added Math + MC agents
- ✅ **Production Ready**: Based on stable codebase

---

## 📦 Installation

### Option 1: Build from Source

```bash
# Clone this specialization
git clone https://github.com/sneakybenson/nanobrowser-specialized.git
cd nanobrowser-specialized

# Install dependencies (requires pnpm)
pnpm install

# Build the extension
pnpm build

# Load in Chrome
# 1. Go to chrome://extensions/
# 2. Enable "Developer mode"
# 3. Click "Load unpacked"
# 4. Select the dist/ folder
```

### Option 2: Download Release

Download from GitHub releases: [Latest Release](https://github.com/sneakybenson/nanobrowser-specialized/releases)

---

## ⚙️ Configuration

### 1. Set API Keys

Click the extension icon → Settings (⚙️):

- **OpenAI API Key**: For text-based solving
- **Anthropic API Key**: For Claude models
- **Nvidia NIM API Key**: For specialized models
- **Other Providers**: Gemini, Ollama, Groq, etc.

### 2. Configure Agents

Choose which models for which agents:

- **Navigator**: Handles DOM interactions (use GPT-4 or Claude)
- **Planner**: High-level planning (use Claude Opus)
- **MathSolver**: Choose math-specialized models
- **MultipleChoice**: Choose reasoning models

### 3. Set Preferences

- Confidence threshold (default: 85%)
- Enable/disable batch mode
- Use vision fallback for images
- Cache answers for speed

---

## 🧪 Testing

### Test Math Solving

1. Open a math assignment page
2. Click extension icon → Side Panel
3. Type: "Solve all math problems on this page"
4. Watch the MathSolver agent work

### Test Multiple Choice

1. Open a quiz page
2. Click extension icon → Side Panel
3. Type: "Answer all multiple choice questions"
4. Agent analyzes and fills in answers

### Test Multi-Step

1. Open a complex assignment
2. Type: "Complete steps 1-5 in order"
3. Agent handles dependencies and sequence

---

## 📊 Supported Platforms

Works on most educational platforms:

- ✅ Canvas (Instructure)
- ✅ Blackboard
- ✅ Moodle
- ✅ Google Forms
- ✅ WebAssign
- ✅ MyMathLab
- ✅ Pearson
- ✅ Custom school platforms

---

## 🔥 Specialized Capabilities

### Math Problem Detection

```
Smart detection of:
- Input fields with math expressions
- Inline equations
- LaTeX notation
- Math images (via vision)
```

### Multiple Choice Analysis

```
AI reasoning for:
- Conceptual questions
- Fact-based questions
- Calculation-based MC
- Multi-select questions
```

### Conditional Logic

```
Handle complex instructions:
- "If answer > 100, then check option A, else B"
- "Solve step 1, use result in step 2"
- "Skip questions with diagrams"
```

---

## 🛡️ Safety & Ethics

**Designed For:**
- ✅ Practice problems
- ✅ Self-assessment
- ✅ Homework help (non-graded)
- ✅ Learning assistance

**Not For:**
- ❌ Cheating on exams
- ❌ Academic dishonesty
- ❌ Bypassing integrity systems

Use responsibly according to your institution's policies.

---

## 🏗️ Architecture

```
NanoBrowser Specialization
├── Original NanoBrowser Agents
│   ├── Navigator (DOM interaction)
│   ├── Planner (task planning)
│   └── Validator (completion check)
│
└── Specialized Agents (NEW!)
    ├── MathSolver
    │   ├── Arithmetic engine
    │   ├── Algebra solver
    │   ├── Calculus processor
    │   └── Step generator
    │
    └── MultipleChoice
        ├── Question detector
        ├── AI analyzer
        ├── Confidence scorer
        └── Vision fallback
```

---

## 🔧 Development

Based on NanoBrowser's monorepo structure:

- **Package Manager**: pnpm
- **Build System**: Turbo + Vite
- **Language**: TypeScript
- **UI**: React + Tailwind
- **Extension**: Chrome Manifest V3

### Commands

```bash
# Development
pnpm dev

# Build
pnpm build

# Type check
pnpm type-check

# Lint
pnpm lint
```

---

## 📝 Credits

**Base Project**: [NanoBrowser](https://github.com/nanobrowser/nanobrowser)
- Original multi-agent browser automation
- Licensed under MIT

**Specialization**: Math + Multiple Choice Agents
- Added academic-focused capabilities
- Specialized prompts and workflows

---

## 📄 License

MIT License - See LICENSE file

---

## 🆘 Support

- **Issues**: GitHub Issues
- **Docs**: This README
- **Base Project**: [NanoBrowser Discord](https://discord.gg/NN3ABHggMK)

---

**Built with ❤️ on top of NanoBrowser**

*Empowering students with AI automation while maintaining academic integrity.*
