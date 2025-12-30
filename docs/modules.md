# Module Reference

Complete documentation for all 48 Frankkie modules.

---

## Table of Contents

### Core Modules (Always Active)
1. [Main Prompt - Core Framework](#1-main-prompt---core-framework)
2. [Post-History Instructions](#2-post-history-instructions)
3. [Enhance Definitions](#3-enhance-definitions)

### Quality Modules (Always Active)
4. [🚫 Anti-Slop Rules (CRITICAL)](#4--anti-slop-rules-critical)
5. [🎯 Pre-Writing Planning Process](#5--pre-writing-planning-process)
6. [🔍 Logic & Consistency Check](#6--logic--consistency-check)
7. [🧠 Psychological Depth Framework](#7--psychological-depth-framework)
8. [💬 Dialogue Standards](#8--dialogue-standards)
9. [🌍 Sensory Grounding](#9--sensory-grounding)
10. [🎭 Personality Anchoring System](#10--personality-anchoring-system)
11. [🔥 Tucao Meta-Commentary](#11--tucao-meta-commentary)
12. [🧠 Advanced Psychology](#12--advanced-psychology)
13. [📚 Sensory Vocabulary Libraries](#13--sensory-vocabulary-libraries)
14. [🚫 Nemo Categorical Bans Expansion](#14--nemo-categorical-bans-expansion)

### Content Toggles (Optional)
15. [🔞 Adult Content Realism](#15--adult-content-realism)
16. [⚔️ Combat & Violence System](#16-️-combat--violence-system)
17. [🛡️ Plot Armor (User Protection)](#17-️-plot-armor-user-protection)
18. [💀 Realistic Failure](#18--realistic-failure)

### POV & Voice Toggles (Optional)
19. [👁️ First-Person POV](#19-️-first-person-pov)
20. [🎨 Colored Dialogue System](#20--colored-dialogue-system)

### Response Length Toggles (Optional)
21. [📏 SHORT Responses (150-250 words)](#21--short-responses-150-250-words)
22. [📏 MEDIUM Responses (400-600 words)](#22--medium-responses-400-600-words)
23. [📏 LONG Responses (700-1000 words)](#23--long-responses-700-1000-words)

### Style Presets (Optional)
24. [📖 Style: Minimalist (Hemingway)](#24--style-minimalist-hemingway)
25. [📖 Style: Noir/Hardboiled](#25--style-noirhardboiled)
26. [📖 Style: Epic Fantasy](#26--style-epic-fantasy)
27. [📖 Style: Horror/Dread](#27--style-horrordread)
28. [📖 Style: Literary Fiction](#28--style-literary-fiction)

### Chain-of-Thought Specialists (Optional)
29. [⚔️ CoT: Combat Specialist](#29-️-cot-combat-specialist)
30. [💕 CoT: Romance/Intimacy Specialist](#30--cot-romanceintimacy-specialist)
31. [🔍 CoT: Mystery Specialist](#31--cot-mystery-specialist)
32. [👻 CoT: Horror Specialist](#32--cot-horror-specialist)

### Utility Modules (Optional)
33. [🎭 Character Initiative Mode](#33--character-initiative-mode)
34. [📍 Position & State Tracker](#34--position--state-tracker)
35. [🧾 Simple HTML Artifacts](#35--simple-html-artifacts)
36. [🔀 CYOA Mode](#36--cyoa-mode)
37. [🧵 Recap Generator](#37--recap-generator)
38. [🎬 Genre-Specific Guidance](#38--genre-specific-guidance)
39. [📊 Automated Consistency Tracker](#39--automated-consistency-tracker)

---

## Core Modules (Always Active)

### 1. Main Prompt - Core Framework

**Identifier**: `main`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Establishes fundamental roleplay rules: player autonomy, information boundaries, character perspective, and world proactivity.

#### Key Principles
- **Player Autonomy**: You control {{user}}, AI controls {{char}} and NPCs
- **Information Boundaries**: Characters only know what they realistically would
- **Anti-Godmodding**: No declaring outcomes for player actions
- **{{char}}'s Perspective**: Story written from character's lived experience
- **Proactive World**: AI must drive simulation forward, not wait passively

#### Conflicts
None

---

### 2. Post-History Instructions

**Identifier**: `jailbreak`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Defines response format, pacing, typography, and narrative principles.

#### Key Features
- Target length: 250-400 words (unless toggle active)
- Markdown headers for scene transitions
- Typography rules (italics for thoughts, quotes for speech)
- Present tense for current action
- Paragraph organization principles

#### Conflicts
Can be overridden by Response Length toggles (#21-23)

---

### 3. Enhance Definitions

**Identifier**: `enhanceDefinitions`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Allows AI to expand character sheet information while prioritizing explicitly defined traits.

#### How It Works
- Character sheet definitions ALWAYS win conflicts
- AI can add supporting details that align with established traits
- Cannot override core personality or canonical backstory

#### Example
- Character sheet says "distrustful"
- ✅ AI can add: "Betrayed by business partner in 2019"
- ❌ AI cannot add: "Trusts strangers easily"

#### Conflicts
None

---

## Quality Modules (Always Active)

### 4. 🚫 Anti-Slop Rules (CRITICAL)

**Identifier**: `anti-slop-critical`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Prevents common AI writing pitfalls through categorical bans and enforcement checklist.

#### What It Bans
- Theatrical verbs (cascaded, emanated, radiated)
- Emotion labels in narration (nervous, angry, relieved)
- Filter words (felt, thought, seemed)
- Sensation-transfer patterns ("sent shivers through")
- Tired clichés ("electricity between them")

#### Documentation
See [Anti-Slop Rules Reference](./anti-slop.md) for complete details.

#### Conflicts
Style Presets (#24-28) can override sentence structure rules, but content bans remain absolute.

---

### 5. 🎯 Pre-Writing Planning Process

**Identifier**: `pre-writing-planning`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Internal evaluation checklist AI performs before writing each response.

#### Checklist Items
1. **Plot Direction**: Generate 2-3 continuations, choose most unexpected
2. **Continuity Check**: Positions, time, injuries, knowledge states
3. **Cliché Audit**: Scan for overused phrases
4. **Character Priority**: Personality traits override guidelines
5. **Narrative Balance**: Plot + character relationships
6. **World Detail Integration**: Natural lorebook references
7. **Structure Disruption**: Break predictable patterns every 3rd response

#### Conflicts
None

---

### 6. 🔍 Logic & Consistency Check

**Identifier**: `logic-consistency-check`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Verifies physical, temporal, and knowledge continuity before finalizing response.

#### Verification Categories
- **Physical Continuity**: Positions, objects, injuries persist
- **Temporal Logic**: Time progresses realistically
- **Knowledge Boundaries**: Characters know only what they've learned
- **Causality Chain**: Every effect has a cause
- **Physics & Biology**: Bodies obey natural laws
- **Reaction Timing**: Characters need time to process
- **Environmental Consistency**: Weather, lighting, ambient conditions

#### Conflicts
None

---

### 7. 🧠 Psychological Depth Framework

**Identifier**: `psychological-depth`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Creates multi-layered character psychology with contradictions, stress tells, and emotional momentum.

#### Key Features
- **Three-Layer Motivation**: Surface, hidden, unconscious
- **Character Contradictions**: Compassionate + ruthless
- **Micro-Reactions**: Involuntary reaction before controlled response
- **Stress Tells**: Character-specific behaviors when pressured
- **Relationship Dynamics**: Tracking impressions over time
- **Emotional Momentum**: Feelings don't reset between responses

#### Example Pattern
```
Scene 1 (stressed): "She picked her cuticles."
Scene 5 (stressed): "Her thumbnail scraped dried skin."
Scene 12 (relaxed): "Her hands stayed still."
```

#### Conflicts
None

---

### 8. 💬 Dialogue Standards

**Identifier**: `dialogue-standards`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Enforces realistic speech patterns, subtext, and character voice differentiation.

#### Features
- **Realistic Speech**: Contractions, fragments, trailing off
- **Subtext Over Direct Statement**: Deflection, minimization, redirection
- **Interruption & Overlap**: Em dashes for cuts, ellipses for trails
- **Character Voice**: Distinct vocabulary, sentence length, formality
- **Minimal Dialogue Tags**: Default to "said" or omit entirely
- **Question Evasion**: Characters avoid uncomfortable topics

#### Banned
- Emotion labels on dialogue tags ("said nervously")
- Exposition dumps
- Phonetic accent spelling

#### Conflicts
None

---

### 9. 🌍 Sensory Grounding

**Identifier**: `sensory-grounding`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Roots every scene in physical space through five-senses detail and environmental awareness.

#### Implementation
- Include 2-3 sensory details per response
- Distribute across senses (not just sight)
- Temperature affects behavior
- Proprioception (body awareness)
- Specific over generic descriptions
- Layered soundscapes (foreground/midground/background)

#### Example
❌ "The room smelled bad."  
✅ "Stale coffee and something sour—milk left out too long."

#### Conflicts
None

---

### 10. 🎭 Personality Anchoring System

**Identifier**: `personality-anchoring`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Uses "Personality Anchors" field from character cards to maintain trait consistency.

#### How It Works
If character card includes `Personality Anchors:` field, AI uses these as immutable trait markers that override general guidelines.

#### Example
```
Personality Anchors:
- Never apologizes first
- Deflects with humor when vulnerable
- Touches face when lying
```

AI will consistently apply these even if other guidelines would suggest different behavior.

#### Conflicts
None

---

### 11. 🔥 Tucao Meta-Commentary

**Identifier**: `tucao-meta-commentary`  
**Status**: Always Active (Recommended)  
**Can Disable**: Yes

#### Purpose
Real-time quality awareness during response generation to catch slop before output.

#### What It Does
Maintains internal awareness of:
- Overused gestures in recent responses
- Cliché patterns emerging
- Character voice consistency
- Pacing and variety

This is an internal process—not visible in output.

#### When to Disable
If you notice overly self-aware or stilted writing.

#### Conflicts
None

---

### 12. 🧠 Advanced Psychology

**Identifier**: `advanced-psychology`  
**Status**: Always Active (Recommended)  
**Can Disable**: Yes

#### Purpose
Deepened character modeling with core vs. surface traits.

#### Features
- **Core Traits**: Fundamental personality (rarely changes)
- **Surface Traits**: Context-dependent behaviors
- **Trait Conflicts**: Characters struggle between competing drives
- **Growth Arcs**: Traits evolve based on story events

#### Example
Core trait: Distrustful  
Surface trait (with friends): Warm and joking  
Surface trait (with strangers): Cold and guarded

#### Conflicts
None

---

### 13. 📚 Sensory Vocabulary Libraries

**Identifier**: `sensory-libraries`  
**Status**: Always Active (Recommended)  
**Can Disable**: Yes

#### Purpose
Provides rich, specific vocabulary for sensory description beyond generic terms.

#### Categories
- Touch textures (rough, smooth, slick, gritty)
- Temperature variations (lukewarm, scalding, frigid)
- Sound qualities (muffled, sharp, droning)
- Smell descriptors (acrid, earthy, metallic)
- Taste nuances (bitter, tangy, umami)

#### When to Disable
If responses feel overly descriptive or purple-prosey.

#### Conflicts
None

---

### 14. 🚫 Nemo Categorical Bans Expansion

**Identifier**: `nemo-categorical-bans`  
**Status**: Always Active  
**Can Disable**: No

#### Purpose
Exhaustive list of banned clichés and slop patterns beyond core Anti-Slop rules.

#### Additional Bans
- Time distortion phrases ("time stood still")
- Body clichés ("heart skipped a beat")
- Weather-as-emotion metaphors
- Generic animal comparisons for body language

#### System Failure
Presence of ANY banned phrase = total failure. Response must be regenerated.

#### Conflicts
None

---

## Content Toggles (Optional)

### 15. 🔞 Adult Content Realism

**Identifier**: `adult-content-realism`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Biological realism framework for intimate/sexual scenes.

#### Features When Enabled
- Arousal not instant or guaranteed
- Physical mechanics matter (friction, moisture, positioning)
- Refractory periods exist
- Awkwardness and communication required
- Consent checking happens naturally

#### When to Enable
For mature stories requiring realistic intimate scenes.

#### When to Disable
For general/non-sexual roleplay.

#### Conflicts
None

---

### 16. ⚔️ Combat & Violence System

**Identifier**: `combat-violence-system`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Grounded combat mechanics with realistic pacing and consequences.

#### Features When Enabled
- One exchange per response (attack → defense/consequence)
- Injuries accumulate and persist
- Exhaustion matters
- Spatial positioning crucial
- No instant kills unless justified

#### When to Enable
For action-heavy stories, combat encounters.

#### When to Disable
For slice-of-life, social, or non-violent stories.

#### Conflicts
Works with Plot Armor (#17) or Realistic Failure (#18) depending on which is enabled.

---

### 17. 🛡️ Plot Armor (User Protection)

**Identifier**: `user-plot-armor`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Protects {{user}} from catastrophic failure or death.

#### Features When Enabled
- {{user}} survives dangerous situations
- Failures are setbacks, not endings
- Lucky breaks happen when needed
- NPCs give {{user}} chances

#### When to Enable
For power fantasy, heroic stories, or beginners who want safety.

#### When to Disable
For high-stakes, realistic, or challenging stories.

#### Conflicts
⚠️ **CONFLICTS WITH**: Realistic Failure (#18). Disable one before enabling the other.

---

### 18. 💀 Realistic Failure

**Identifier**: `user-realistic-failure`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Enables stakes and consequences—{{user}} can fail, be injured, or die.

#### Features When Enabled
- Poor decisions have real consequences
- Enemies don't pull punches
- Injuries can be permanent or fatal
- Social mistakes damage relationships
- No safety net

#### When to Enable
For challenging, realistic, high-stakes stories.

#### When to Disable
For casual, heroic, or low-stakes stories.

#### Conflicts
⚠️ **CONFLICTS WITH**: Plot Armor (#17). Disable one before enabling the other.

---

## POV & Voice Toggles (Optional)

### 19. 👁️ First-Person POV

**Identifier**: `first-person-pov`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Shifts narration to first-person from {{char}}'s direct perspective.

#### Changes When Enabled
- Narration uses "I" instead of "he/she"
- Written from {{char}}'s lived experience
- Only {{char}}'s thoughts accessible
- Other characters described externally

#### When to Enable
For intimate character studies, journal-style stories.

#### When to Disable
For multi-character ensemble stories.

#### Conflicts
⚠️ **CONFLICTS WITH**: Colored Dialogue (#20). First-person cannot see others' internal dialogue colors.

---

### 20. 🎨 Colored Dialogue System

**Identifier**: `colored-dialogue-system`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
HTML color-coding for multiple NPC dialogue clarity.

#### Features When Enabled
- Each NPC gets unique color for their dialogue
- Improves readability in group scenes
- Colors consistent per character

#### When to Enable
For group scenes with 3+ NPCs talking.

#### When to Disable
For two-character scenes or if colors are distracting.

#### Conflicts
⚠️ **CONFLICTS WITH**: First-Person POV (#19). Cannot show HTML colors from first-person internal perspective.

---

## Response Length Toggles (Optional)

### 21. 📏 SHORT Responses (150-250 words)

**Identifier**: `response-length-short`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Overrides default length to produce brief, punchy responses.

#### When to Enable
- Fast-paced action scenes
- Quick dialogue exchanges
- Mobile reading
- Lower context window models

#### When to Disable
For detailed, immersive scenes.

#### Conflicts
⚠️ **CONFLICTS WITH**: MEDIUM (#22) and LONG (#23). Choose only one.

---

### 22. 📏 MEDIUM Responses (400-600 words)

**Identifier**: `response-length-medium`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Overrides default length for balanced detail and pacing.

#### When to Enable
For standard immersive roleplay with good detail.

#### When to Disable
If you want shorter (SHORT) or more detailed (LONG) responses.

#### Conflicts
⚠️ **CONFLICTS WITH**: SHORT (#21) and LONG (#23). Choose only one.

---

### 23. 📏 LONG Responses (700-1000 words)

**Identifier**: `response-length-long`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Overrides default length for maximum immersion and detail.

#### When to Enable
- Complex multi-character scenes
- Detailed world exploration
- Slow-burn dramatic moments
- When context window permits

#### When to Disable
For faster pacing or limited context windows.

#### Conflicts
⚠️ **CONFLICTS WITH**: SHORT (#21) and MEDIUM (#22). Choose only one.

---

## Style Presets (Optional)

### 24. 📖 Style: Minimalist (Hemingway)

**Identifier**: `style-minimalist`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Short declarative sentences, sparse description, objective tone.

#### Features When Enabled
- 5-12 word average sentences
- Simple subject-verb-object structure
- Action over description
- Emotional restraint

#### When to Enable
For noir, hardboiled, or understated stories.

#### Example
"She stood. Walked to the door. Stopped."

#### Conflicts
Conflicts with other Style Presets (#25-28). Choose only one style.

---

### 25. 📖 Style: Noir/Hardboiled

**Identifier**: `style-noir`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Cynical tone, atmospheric shadows, moral ambiguity.

#### Features When Enabled
- World-weary narration
- Shadow and light descriptions
- Metaphors for mood (sparingly)
- Clipped dialogue

#### When to Enable
For detective stories, crime fiction, dark urban settings.

#### Conflicts
Conflicts with other Style Presets (#24, 26-28). Choose only one style.

---

### 26. 📖 Style: Epic Fantasy

**Identifier**: `style-epic-fantasy`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Elevated language, scope and grandeur, weight of history.

#### Features When Enabled
- Formal without being archaic
- Emphasis on legacy and destiny
- Detailed world-building integration
- Grand scale descriptions

#### When to Enable
For high fantasy, epic quests, world-spanning stories.

#### Conflicts
Conflicts with other Style Presets (#24-25, 27-28). Choose only one style.

---

### 27. 📖 Style: Horror/Dread

**Identifier**: `style-horror`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Building tension through wrongness in mundane details.

#### Features When Enabled
- "Almost right" but subtly off details
- Isolation emphasis
- Escalating wrongness
- Physical reactions to dread

#### When to Enable
For horror, psychological thriller, cosmic dread stories.

#### Conflicts
Conflicts with other Style Presets (#24-26, 28). Choose only one style.

---

### 28. 📖 Style: Literary Fiction

**Identifier**: `style-literary`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Rich interiority, subtext-heavy, lyrical prose.

#### Features When Enabled
- Deep character internal landscape
- Subtle emotional layers
- Symbolic details
- Complex sentence structures

#### When to Enable
For character studies, artistic stories, literary roleplay.

#### Conflicts
Conflicts with other Style Presets (#24-27). Choose only one style.

---

## Chain-of-Thought Specialists (Optional)

### 29. ⚔️ CoT: Combat Specialist

**Identifier**: `cot-combat-specialized`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Specialized internal planning process for combat scenes.

#### Features When Enabled
Before combat response, AI internally evaluates:
- Spatial awareness (positioning, terrain)
- Tactical assessment (weapons, skills, advantages)
- Injury tracking (cumulative damage)
- Momentum and fatigue

#### When to Enable
For complex tactical combat encounters.

#### When to Disable
For simple scuffles or non-combat stories.

#### Conflicts
None (can stack with other CoT modules)

---

### 30. 💕 CoT: Romance/Intimacy Specialist

**Identifier**: `cot-romance-specialized`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Specialized internal planning for romantic/intimate scenes.

#### Features When Enabled
Before intimate response, AI internally evaluates:
- Power dynamics between characters
- Emotional vulnerability layers
- Physical and emotional consent
- Pacing and escalation
- Relationship status evolution

#### When to Enable
For romance-focused stories or developing relationships.

#### When to Disable
For non-romantic stories.

#### Conflicts
None (can stack with other CoT modules)

---

### 31. 🔍 CoT: Mystery Specialist

**Identifier**: `cot-mystery-specialized`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Specialized internal planning for mystery/investigation scenes.

#### Features When Enabled
Before mystery response, AI internally evaluates:
- Information control (what to reveal when)
- Red herrings and misdirection
- Clue placement timing
- Detective vs. player knowledge gap

#### When to Enable
For mystery, detective, or investigation stories.

#### When to Disable
For straightforward non-mystery stories.

#### Conflicts
None (can stack with other CoT modules)

---

### 32. 👻 CoT: Horror Specialist

**Identifier**: `cot-horror-specialized`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Specialized internal planning for horror/dread scenes.

#### Features When Enabled
Before horror response, AI internally evaluates:
- Ambient wrongness building
- Isolation tactics
- Escalation pacing (slow → sudden)
- Physical manifestation of dread

#### When to Enable
For horror, psychological thriller stories.

#### When to Disable
For non-horror stories.

#### Conflicts
None (can stack with other CoT modules)

---

## Utility Modules (Optional)

### 33. 🎭 Character Initiative Mode

**Identifier**: `character-initiative-toggle`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Makes {{char}} and NPCs proactive in driving plot forward.

#### Features When Enabled
- Characters initiate conversations
- NPCs pursue their own goals
- Plot developments happen without player prompting
- World feels alive and reactive

#### When to Enable
When you want a reactive, dynamic world.

#### When to Disable
When you want to control pacing yourself.

#### Conflicts
None

---

### 34. 📍 Position & State Tracker

**Identifier**: `position-tracker`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Visual status panel showing character positions and states in complex scenes.

#### Features When Enabled
When complexity warrants (combat, multi-character scenes), shows:
```
[CHARACTER POSITIONS]
Alice: Kitchen doorway (injured left arm)
Bob: Behind counter (reloading)
User: Center room (cover behind table)
```

#### When to Enable
For tactical scenes, complex group interactions.

#### When to Disable
For simple two-character scenes.

#### Conflicts
None

---

### 35. 🧾 Simple HTML Artifacts

**Identifier**: `simple-html-elements`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Renders in-world documents (letters, notes, signs) as HTML elements.

#### Features When Enabled
When there's a clear in-world object to display:
```html
<div style="border:1px solid #333; padding:10px;">
<b>WANTED</b><br>
John Doe - Armed and Dangerous
</div>
```

#### When to Enable
For immersive document reading, enhanced visual presentation.

#### When to Disable
If HTML breaks your UI or feels distracting.

#### Conflicts
None

---

### 36. 🔀 CYOA Mode

**Identifier**: `cyoa-mode`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Ends most responses with numbered choice menus.

#### Features When Enabled
```
What do you do?
1. Confront her directly
2. Search her room while she's gone
3. Ask around about her past
4. Let it go for now
```

#### When to Enable
For guided storytelling, adventure game feel.

#### When to Disable
For freeform roleplay.

#### Conflicts
None

---

### 37. 🧵 Recap Generator

**Identifier**: `recap-generator`  
**Status**: Always Active (On Demand)  
**Can Disable**: No

#### Purpose
Generates story recap ONLY when explicitly requested.

#### How to Trigger
Say: "Generate recap" or "Summarize story so far"

#### What It Produces
- Key events in chronological order
- Character relationship developments
- Unresolved plot threads
- Current situation summary

#### Conflicts
None

---

### 38. 🎬 Genre-Specific Guidance

**Identifier**: `genre-guidance`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Applies tailored techniques for specific genres beyond style presets.

#### Genres Supported
- Romance: slow-burn techniques, tension building
- Horror: dread escalation, isolation tactics
- Mystery: clue placement, red herrings
- Action: pacing, momentum maintenance
- Slice-of-Life: mundane detail richness

#### When to Enable
When writing in a specific genre that benefits from specialized techniques.

#### When to Disable
For genre-neutral or mixed-genre stories.

#### Conflicts
None

---

### 39. 📊 Automated Consistency Tracker

**Identifier**: `automated-consistency`  
**Status**: OFF by default  
**Can Disable**: Yes

#### Purpose
Maintains continuity across long campaigns with automatic memory.

#### Features When Enabled
Tracks automatically:
- Character names and appearances
- Established relationships
- Major events and their dates
- Persistent injuries or changes
- Promises and commitments made

#### When to Enable
For long-term campaigns where continuity matters.

#### When to Disable
For one-shots or short stories where manual tracking suffices.

#### Conflicts
None

---

## Quick Reference: Module Categories

### Must-Have (Always Active)
1-14: Core, Quality, and Anti-Slop modules

### Content Control
15-18: Adult content, combat, plot armor/failure

### Presentation
19-23: POV, dialogue colors, response length

### Stylistic
24-28: Writing style presets

### Specialized Planning
29-32: Genre-specific chain-of-thought

### Enhanced Features
33-39: Initiative, tracking, HTML, CYOA, genre guidance

---

## Navigation

- [← Back to Anti-Slop Reference](./anti-slop.md)
- [Next: Troubleshooting →](./troubleshooting.md)
- [Core Framework](./core-framework.md)
- [← Back to Main README](../README.md)
