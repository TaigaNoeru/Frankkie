# Troubleshooting Guide

Common issues and solutions when using Frankkie presets.

---

## Table of Contents

1. [Installation Issues](#installation-issues)
2. [Quality Problems](#quality-problems)
3. [Module Conflicts](#module-conflicts)
4. [Performance Issues](#performance-issues)
5. [Output Problems](#output-problems)
6. [Advanced Configuration](#advanced-configuration)

---

## Installation Issues

### Problem: Import fails in SillyTavern

**Symptoms**: Error message when trying to import JSON file

**Solutions**:
1. Verify JSON file is not corrupted (open in text editor, check for errors)
2. Make sure you're using SillyTavern version 1.10.0 or higher
3. Try importing via: Settings → User Settings → Presets → Import
4. Clear browser cache and try again

---

### Problem: Preset doesn't appear in dropdown

**Symptoms**: After import, preset not visible in selection menu

**Solutions**:
1. Refresh SillyTavern page (F5)
2. Check that import was successful (look for success message)
3. Verify preset saved to correct folder: `/SillyTavern/public/user/presets/`
4. Restart SillyTavern

---

## Quality Problems

### Problem: AI still uses "slop" phrases despite Anti-Slop

**Symptoms**: Output contains banned phrases like "cascaded through," "sent shivers," etc.

**Causes**:
- Model not following instructions well
- Context window too small
- Conflicting character card instructions

**Solutions**:
1. **Switch to better model**: Claude 3.5 Sonnet, GPT-4, or similar high-instruction-following models
2. **Increase max context**: Set to at least 8000 tokens
3. **Check character card**: Remove contradicting style instructions from character description
4. **Use Frankkie Lite**: If using smaller model, try lite version with fewer modules
5. **Add emphasis**: In character card, add: `[CRITICAL: Follow anti-slop rules strictly]`

---

### Problem: Responses are too generic/bland

**Symptoms**: Output lacks personality, feels formulaic

**Solutions**:
1. **Check character card quality**: Vague cards produce vague outputs
2. **Enable Advanced Psychology** (#12): Should be ON by default
3. **Add Personality Anchors**: In character card, add specific behavioral patterns
4. **Increase temperature**: Try 1.0-1.05 (current default: 0.95)
5. **Enable Character Initiative** (#33): Makes NPCs more proactive

---

### Problem: AI repeats same gestures constantly

**Symptoms**: Character crosses arms 5 times in 3 responses

**Causes**:
- Pre-Writing Planning not catching repetition
- Model defaulting to common patterns

**Solutions**:
1. **Regenerate response**: Swipe for alternate
2. **Edit prompt**: Add to character card: `[Character's stress tells: <specific unique gesture>]`
3. **Check model temperature**: Too low = more repetition
4. **Manually note in OOC**: `(Please vary physical actions - arm crossing overused)`

---

### Problem: Dialogue feels unnatural

**Symptoms**: Characters speak in exposition, overly formal, or robotic

**Solutions**:
1. **Verify Dialogue Standards active** (#8): Should be always-on
2. **Check character card speech examples**: Add realistic dialogue samples
3. **Review Anti-Slop Section 6**: Emotion labels on dialogue tags banned
4. **Add speech pattern note**: In character card: `Speech: casual, uses contractions, sentence fragments`
5. **Try Minimalist Style** (#24): Forces brevity and natural speech

---

## Module Conflicts

### Problem: First-Person POV + Colored Dialogue both enabled

**Symptoms**: Error or weird formatting

**Solution**: Disable one. First-person cannot display HTML colors for other characters' internal dialogue.

**How to Fix**:
1. Go to preset settings
2. Find module #19 (First-Person POV) or #20 (Colored Dialogue)
3. Set `"enabled": false` for one of them
4. Save preset

---

### Problem: Plot Armor + Realistic Failure both enabled

**Symptoms**: Inconsistent consequences, AI confused about stakes

**Solution**: Choose your story mode—you can't have both.

**How to Fix**:
1. **For heroic/safe story**: Enable Plot Armor (#17), disable Realistic Failure (#18)
2. **For high-stakes story**: Enable Realistic Failure (#18), disable Plot Armor (#17)
3. Save preset

---

### Problem: Multiple length toggles enabled

**Symptoms**: Inconsistent response lengths, AI confused

**Solution**: Enable only ONE length toggle (SHORT, MEDIUM, or LONG).

**How to Fix**:
1. Find modules #21, #22, #23 in preset
2. Set `"enabled": true` for ONLY ONE
3. Set `"enabled": false` for the other two
4. Or disable all three to use default (250-400 words)
5. Save preset

---

### Problem: Multiple style presets enabled

**Symptoms**: Writing style inconsistent or contradictory

**Solution**: Enable only ONE style preset (or none for default).

**How to Fix**:
1. Find modules #24-28 (Style presets)
2. Choose ONE style or disable all
3. Set `"enabled": true` for chosen style only
4. Set `"enabled": false` for all others
5. Save preset

---

## Performance Issues

### Problem: Responses take very long to generate

**Symptoms**: 30+ seconds per response

**Causes**:
- Too many modules active
- Context window too large
- Model overloaded

**Solutions**:
1. **Use Frankkie Lite**: Streamlined version with core modules only
2. **Disable optional modules**: Turn off CoT specialists, utility modules you're not using
3. **Reduce response length**: Enable SHORT toggle (#21)
4. **Reduce max context**: Try 4000-6000 tokens instead of 100,000
5. **Switch to faster model**: Some models are slower despite equal quality

---

### Problem: Running out of context window

**Symptoms**: "Context limit exceeded" errors, truncated chat history

**Solutions**:
1. **Use Frankkie Lite**: Uses less context
2. **Disable unused modules**: Each active module consumes tokens
3. **Reduce chat history depth**: Settings → Context → Chat History Depth
4. **Enable Automated Consistency Tracker** (#39): Helps maintain continuity with less history
5. **Use summarization**: Periodically summarize older messages and remove them

---

## Output Problems

### Problem: Responses too short

**Symptoms**: 50-100 word responses when expecting 250+

**Causes**:
- SHORT toggle accidentally enabled
- Model cutting off early
- Insufficient max tokens

**Solutions**:
1. **Disable SHORT toggle** (#21): Check it's OFF
2. **Increase max tokens**: Set to at least 1000 (current: 6000)
3. **Check model settings**: Some APIs have separate max token limits
4. **Add to system prompt**: `[Target response length: 250-400 words]`

---

### Problem: Responses too long

**Symptoms**: 800+ word walls of text

**Causes**:
- LONG toggle enabled
- Model ignoring length guidance
- Character card asks for detailed responses

**Solutions**:
1. **Disable LONG toggle** (#23): Check it's OFF
2. **Enable SHORT toggle** (#21): Forces brevity
3. **Reduce max tokens**: Set to 500-600 tokens
4. **Edit character card**: Remove "detailed" or "lengthy" instructions

---

### Problem: AI controls {{user}} / godmodding

**Symptoms**: AI writes your actions, dialogue, or decisions

**Causes**:
- Model not following instructions
- Character card contradicts core rules
- Insufficient instruction following capability

**Solutions**:
1. **Use better model**: This is an instruction-following issue
2. **Check assistant prefill**: Verify it says "I will never write {{user}}'s actions"
3. **Add emphasis in character card**: `[CRITICAL: Never write {{user}}'s dialogue or actions]`
4. **OOC correction**: Stop generation and say `(OOC: Please don't write my character's actions)`
5. **Regenerate**: Swipe for new response

---

### Problem: Inconsistent character personality

**Symptoms**: Character acts differently each response

**Causes**:
- Vague character card
- Personality Anchoring not working
- Model not maintaining consistency

**Solutions**:
1. **Improve character card**: Add specific personality traits, speech patterns, behavioral anchors
2. **Add Personality Anchors**: Use the dedicated field for immutable traits
3. **Enable Automated Consistency Tracker** (#39): Helps maintain long-term traits
4. **Check Logic & Consistency** (#6): Should be always-on
5. **Lower temperature**: Try 0.85-0.90 for more consistency

---

### Problem: World details inconsistent (location, time, etc.)

**Symptoms**: Sun sets twice, character teleports, objects vanish

**Causes**:
- Logic & Consistency Check not catching errors
- Too little chat history in context
- Model attention issues

**Solutions**:
1. **Increase chat history depth**: More context = better continuity
2. **Use lorebook/world info**: Define persistent facts (time of day, locations)
3. **Enable Position Tracker** (#34): Visual reminder of spatial positions
4. **Enable Automated Consistency Tracker** (#39): Tracks world state
5. **Manual correction**: Edit responses to fix continuity breaks

---

## Advanced Configuration

### Customizing Module Priorities

Modules have `injection_order` that determines priority. Lower numbers = earlier execution.

**Current Order**:
- 0: Anti-Slop (highest priority)
- 5: Pre-Writing Planning
- 10: Logic Check
- 15: Psychological Depth
- 20: Dialogue Standards
- 25: Sensory Grounding

**To Change Priority**:
1. Open JSON in text editor
2. Find module's `injection_order` value
3. Change number (lower = higher priority)
4. Save and re-import

---

### Creating Custom Modules

You can add your own prompt modules to Frankkie.

**Structure**:
```json
{
  "identifier": "my-custom-module",
  "system_prompt": false,
  "enabled": true,
  "marker": false,
  "name": "My Custom Module",
  "role": "user",
  "content": "Your prompt text here",
  "injection_position": 1,
  "injection_depth": 0,
  "injection_order": 50,
  "forbid_overrides": false,
  "injection_trigger": []
}
```

**Add to `prompts` array** in JSON.

---

### Parameter Tuning

Current defaults optimized for creative output. Adjust for different needs:

**For More Creativity**:
- Temperature: 1.0-1.1
- Top-K: 150
- Top-P: 0.98

**For More Consistency**:
- Temperature: 0.85-0.90
- Top-K: 80
- Repetition Penalty: 1.15

**For Faster Responses**:
- Max Tokens: 300-500
- Enable SHORT toggle

---

### Model-Specific Tips

**Claude (Anthropic)**:
- Works excellently with Frankkie Full
- Follows anti-slop rules reliably
- Use system prompt mode: enable `claude_use_sysprompt: true`

**GPT-4 (OpenAI)**:
- Strong instruction following
- May need slight temperature increase (1.0)
- Works well with all modules

**Local Models (Llama, Mistral, etc.)**:
- **Use Frankkie Lite** for smaller models (<30B parameters)
- Increase temperature to 1.05-1.1
- May struggle with complex modules (disable CoT specialists)
- Focus on core quality modules only

**Gemini**:
- Works well with Frankkie Full
- May need repetition penalty increase (1.15)
- Use sysprompt mode: `use_makersuite_sysprompt: true`

---

## Still Having Issues?

### Check These First
1. ✅ Using SillyTavern 1.10.0+
2. ✅ Model supports instruction following
3. ✅ Max context at least 8000 tokens
4. ✅ No conflicting modules enabled
5. ✅ Character card doesn't contradict framework

### Get Help
- **GitHub Issues**: Report bugs or request features
- **SillyTavern Discord**: Community support
- **Reddit r/SillyTavernAI**: General discussion

### Reporting Bugs
Include:
1. Frankkie version (Full or Lite)
2. Model being used
3. Active modules (list enabled toggles)
4. Example of problem output
5. Character card (if relevant)

---

## Navigation

- [← Back to Module Reference](./modules.md)
- [Core Framework](./core-framework.md)
- [Anti-Slop Reference](./anti-slop.md)
- [← Back to Main README](../README.md)
