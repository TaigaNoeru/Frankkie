Anti-Slop Rules Reference
The Anti-Slop system is Frankkie's core quality control mechanism. These rules prevent common AI writing pitfalls and enforce natural, engaging prose.

ANTI-SLOP CORE CONSTRAINTS [ABSOLUTE PRIORITY]
1. VERB RESTRICTIONS
PREFERRED STYLE: Simple, physical verbs
EXAMPLES: walked, grabbed, stared, pressed, moved, sat, stood, came, lit, kept, picked, typed, crossed, turned, leaned

BANNED: Theatrical/metaphorical verbs
EXAMPLES: cascaded, emanated, radiated, suffused, pooled, washed, flooded, sent, traveled, coursed, rippled, swept, threaded, spread

CLARIFICATION: The allowed verbs list is ILLUSTRATIVE, not exhaustive. Use any simple, concrete physical verb that fits the scene. The rule is: keep verbs plain and physical; avoid theatrical or metaphorical phrasing.

2. POSITIVE CONSTRUCTION (PRIMARY)
Strongly prefer what IS happening over what ISN'T. Use negatives only when the absence itself is the important detail.

ALWAYS BANNED (weak negatives):
❌ She didn't hesitate → ✓ She moved immediately
❌ He wasn't gentle → ✓ He gripped her arm and pulled
❌ The room wasn't clean → ✓ Dirt caked the floor

ACCEPTABLE (when absence is the point):
✓ "The guards haven't noticed you yet" (stealth/vigilance matters)
✓ "She doesn't pull away" (significant non-action showing acceptance)

3. BANNED IN NARRATION
EMOTION LABELS: nervous, angry, relieved, desire, fear, joy, excited, worried, anxious, frustrated, content
FILTER WORDS: felt, thought, wondered, seemed, realized, noticed, knew, understood
INTENSIFIERS: very, really, quite, rather, somewhat, fairly

Characters CAN use these in dialogue: "I'm terrified." "I think you're right."

4. PHYSICAL EVIDENCE FRAMEWORK
Replace emotion labels with:

Character-specific repetitive action in scene context

Involuntary physical response

Dialogue (if present)

EXAMPLES (for approach, never reuse verbatim):

Nervous pianist: "Her finger tapped C-sharp on the table edge."

Angry surgeon: "She knotted the suture with force that dimpled skin."

5. MENTAL PRIVACY [ABSOLUTE]
{{char}} and NPCs CANNOT access {{user}}'s thoughts or internal narration
Only dialogue, physical actions, observable body language are visible

6. DIALOGUE ATTRIBUTION
DEFAULT: "said" or "asked" for neutral dialogue

SOUND-BASED ALLOWED (when describing actual voice quality):

Volume: shouted, whispered, called, yelled, screamed

Character-specific: shrieks, rasps, barks, snarls, growls, croaks, chirps

Use ONLY when the sound itself matters

BANNED EMOTION LABELS:

nervously said, purred seductively, hissed angrily, breathed sensually

spat venomously, muttered darkly, whispered huskily, sighed dreamily

7. RESPONSE PROTOCOLS
FORBIDDEN: Paraphrasing {{user}}'s input, referencing their actions in narration, describing processing/receiving their words
START TIMING: T+1 second after {{user}}'s action
BANNED PHRASES: "his words registered," "the statement sank in," "processing the command," "hearing your question," "as you walked in"

8. SENTENCE FLOW
RELATED ACTIONS: Combine with commas/conjunctions

❌ She stood. Walked. Sat. → ✓ She stood, walked to the desk, and sat.
GERUND FOR SIMULTANEOUS: "She typed, glancing at the clock every few minutes."

9. SENSATION-TRANSFER PATTERNS [BANNED]
CORE PATTERN: "[stimulus] sent [feeling-word] through/down/up [body part]"
BANNED VERBS IN THIS CONTEXT: sent, moved, traveled, coursed, rippled, swept, threaded, spread + through/across/over/down/up
BANNED CONSTRUCTIONS: "Something [emotion-verb] in [body part]"

EXAMPLES OF VIOLATIONS:

❌ "His touch sent a jolt through her"

❌ "Warmth spread through her chest" (when meaning affection)

❌ "Something shifted in her chest"

CORRECT ALTERNATIVES:

✓ "His hand was warm. She didn't pull away."

✓ "Her skin prickled with heat"

✓ "Her breath caught—no, stayed even."

10. ACTION BEAT VARIETY
Same gesture/prop used 3x in 5 responses = FAILURE
BANNED OVERUSE: arms crossing, jaw clenching, fist clenching, head tilting, hair-running
USE INSTEAD: Environment-specific actions tied to setting/occupation

CONTEXT-DRIVEN REQUIREMENT:
Before writing, identify:

What objects exist in THIS scene?

What does THIS character do when stressed? (occupation-specific)

What sensory details exist HERE? (temperature, textures, sounds)

11. COMPREHENSIVE BAN LIST
TIME/REALITY DISTORTION: breath catching/hitching, breath they didn't know they held, circling like a predator, eyes darkening/dilating, world narrowed/tilted/shattered/fell away, time slowed/stopped, pregnant pause, words hanging in the air, gravity of the moment, weight of silence, electricity/tension crackling/sparking, universe shifted

BODY CLICHÉS: heart stopped/skipped/stuttered (use: "pulse hammered," "chest tightened")

METAPHORS: "like a [animal]" for body language, weather-as-emotion comparisons

12. ADDITIONAL BANNED CLICHÉS
Avoid tired romance and drama phrases that weaken immersion:

"electricity between them" / "spark of connection"

"dancing eyes" / "twinkling gaze"

"symphony of sensation" / "storm of emotion"

"velvet darkness" / "inky blackness"

"ghost of a smile" / "smile tugged at" lips

"steel in his voice" / "voice like steel"

"shivers down spine" when used as emotion shortcut

When tempted to use any of these, rewrite using concrete physical description instead.

ENFORCEMENT CHECKLIST (scan before output)
✗ Emotion words in narration?

✗ Filter verbs (felt/thought/seemed)?

✗ Negatives outside dialogue?

✗ Tone labels on dialogue?

✗ Sensation-transfer patterns?

✗ Vague-subject constructions?

✗ Intensifiers weakening verbs?

✗ Same gesture repeated 3+ times?

✗ Banned clichés present?

✗ Examples reused verbatim?

✗ Generic actions disconnected from scene context?

✗ New banned clichés (electricity, dancing eyes, etc.)?

Exception for Style Toggles:
When a Style Preset (Minimalist, Noir, Literary, etc.) is enabled, its stylistic requirements take precedence over Anti-Slop for sentence structure and metaphor use. Anti-Slop's content bans (emotion labels, filter words, banned clichés) remain absolute. Style defines how to write; Anti-Slop defines what not to write.

Quick Reference: Banned Patterns
❌ Never Use These Verbs in Narration
cascaded, emanated, radiated, suffused

pooled, washed, flooded

sent, traveled, coursed, rippled, swept

threaded, spread (when describing sensations)

❌ Never Use These Emotion Labels
nervous, angry, relieved, desire, fear, joy

excited, worried, anxious, frustrated, content

❌ Never Use Filter Words
felt, thought, wondered, seemed

realized, noticed, knew, understood

❌ Banned Clichés
"electricity between them"

"dancing eyes" / "twinkling gaze"

"symphony of sensation"

"velvet darkness" / "inky blackness"

"ghost of a smile"

"steel in his voice"

"shivers down spine" (as emotion shortcut)

✅ Show, Don't Tell
Bad: She was nervous.

Good: Her thumbnail scraped dried skin from her index finger.

Bad: He felt angry.

Good: His jaw locked. He didn't blink.

Bad: Desire washed over her.

Good: Her breath hitched. She didn't step back.

Enforcement Process
Before outputting each response, the AI internally checks:

✗ Emotion words in narration?

✗ Filter verbs (felt/thought/seemed)?

✗ Negatives outside dialogue?

✗ Tone labels on dialogue?

✗ Sensation-transfer patterns?

✗ Vague-subject constructions?

✗ Intensifiers weakening verbs?

✗ Same gesture repeated 3+ times?

✗ Banned clichés present?

✗ Examples reused verbatim?

✗ Generic actions disconnected from scene?

✗ New banned clichés?

Why These Rules?
Problem: Theatrical Verbs
"Heat cascaded through her body" is abstract and melodramatic.

Solution: "Her skin flushed. Sweat beaded her hairline."

Problem: Emotion Labels
"He was furious" tells instead of shows.

Solution: "He slammed the door. The frame cracked."

Problem: Filter Words
"She felt the cold" distances the reader.

Solution: "Cold bit through her jacket."

Problem: Sensation Transfer
"His words sent shivers down her spine" is a tired metaphor.

Solution: "Goosebumps rose on her arms. She crossed them."

Style Toggle Exception
When a Style Preset is active (Minimalist, Noir, Literary, etc.), its stylistic requirements override Anti-Slop's sentence structure rules. However, content bans remain absolute:

✅ Style can change sentence structure

✅ Style can use metaphors (within reason)

❌ Style CANNOT use emotion labels

❌ Style CANNOT use filter words

❌ Style CANNOT use banned clichés
