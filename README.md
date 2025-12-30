# Frankkie

**Advanced prompt engineering library for immersive AI roleplay**

Frankkie (formerly APEX v4.1) is a comprehensive SillyTavern preset featuring 48 modular prompts designed for high-quality AI storytelling. Built on anti-slop principles, psychological depth frameworks, and detailed writing standards.

---

## 🚀 Quick Start

1. **Download**: [frankkie.json](./presets/frankkie.json)
2. **Import to SillyTavern**: Settings → User Settings → Import
3. **Configure**: Enable/disable modules based on your needs

---

## 📦 What's Inside

### Core Framework (Always Active)
- **Main Prompt**: Prime directives, player autonomy, character perspective
- **Anti-Slop Rules**: Comprehensive writing quality constraints
- **Response Format**: Turn-by-turn pacing, structure guidelines
- **Pre-Writing Planning**: Internal evaluation checklist
- **Logic & Consistency Check**: Physical and temporal continuity verification

### Always-On Quality Modules
- 🧠 **Psychological Depth Framework**: Multi-layered character motivation
- 💬 **Dialogue Standards**: Realistic speech patterns and subtext
- 🌍 **Sensory Grounding**: Five-senses environmental immersion
- 🎭 **Personality Anchoring**: Character trait consistency
- 🔥 **Tucao Meta-Commentary**: Real-time quality awareness
- 🧠 **Advanced Psychology**: Core vs surface trait modeling
- 📚 **Sensory Vocabulary Libraries**: Rich descriptive palettes
- 🚫 **Nemo Categorical Bans**: Expanded slop prevention

### Optional Content Toggles

| Toggle | Purpose | Conflicts |
|--------|---------|-----------|
| 🔞 Adult Content Realism | Biological realism for intimate scenes | None |
| ⚔️ Combat & Violence System | Grounded combat mechanics | None |
| 🛡️ Plot Armor | User protection from failure | Realistic Failure |
| 💀 Realistic Failure | Stakes & consequences enabled | Plot Armor |

### POV & Voice Options

| Toggle | Purpose | Conflicts |
|--------|---------|-----------|
| 👁️ First-Person POV | Character's direct perspective | Colored Dialogue |
| 🎨 Colored Dialogue | HTML color-coding for multiple NPCs | First-Person POV |

### Response Length Control

| Toggle | Word Count | Conflicts |
|--------|------------|-----------|
| 📏 SHORT | 150-250 words | MEDIUM, LONG |
| 📏 MEDIUM | 400-600 words | SHORT, LONG |
| 📏 LONG | 700-1000 words | SHORT, MEDIUM |

**Default**: 250-400 words when no length toggle is active.

### Style Presets

| Style | Description |
|-------|-------------|
| 📖 Minimalist (Hemingway) | Short sentences, sparse description |
| 📖 Noir/Hardboiled | Cynical tone, atmospheric shadows |
| 📖 Epic Fantasy | Elevated language, scope and grandeur |
| 📖 Horror/Dread | Wrongness in details, building tension |
| 📖 Literary Fiction | Rich interiority, subtext-heavy |

### Chain-of-Thought Specialists

| CoT Module | Optimized For |
|------------|---------------|
| ⚔️ Combat | Spatial awareness, tactical planning |
| 💕 Romance/Intimacy | Power dynamics, emotional layers |
| 🔍 Mystery | Information control, red herrings |
| 👻 Horror | Dread building, isolation tactics |

### Utility Modules

- 🎭 **Character Initiative Mode**: Proactive NPCs that drive plot
- 📍 **Position & State Tracker**: Visual status panel for complex scenes
- 🧾 **Simple HTML Artifacts**: In-world documents rendered as HTML
- 🔀 **CYOA Mode**: Choice menus at response end
- 🧵 **Recap Generator**: On-demand story summaries
- 🎬 **Genre-Specific Guidance**: Tailored techniques per genre
- 📊 **Automated Consistency Tracker**: Long campaign memory aid

---

## 🎛️ Configuration Guide

### For Beginners
Enable these first:
- Core Framework (always on)
- Default response length (250-400 words)
- No style presets

### For Experienced Users
Customize based on your story:
1. Choose ONE response length toggle
2. Choose ONE style preset (or none)
3. Choose content toggles as needed
4. Choose utility modules based on scene complexity

### Conflict Matrix

❌ First-Person POV + Colored Dialogue
❌ Plot Armor + Realistic Failure
❌ SHORT + MEDIUM + LONG (choose one only)

text

---

## 📊 Parameters

| Parameter | Value | Purpose |
|-----------|-------|---------|
| Temperature | 0.95 | Creative variance |
| Top-K | 120 | Wider vocabulary |
| Top-P | 0.95 | Nucleus sampling |
| Frequency Penalty | 0.17 | Reduce repetition |
| Presence Penalty | 0.15 | Encourage variety |
| Repetition Penalty | 1.13 | Anti-loop |
| Max Tokens | 6000 | Response ceiling |

---

## 🙏 Credits

Built upon community presets: Sushi, DeepSeek, Poppet, Lucid Loom, Izumi, Nemo Engine.
Commit changes.
