# Voice Patterns Gap Analysis

**Analysis Date:** 2026-02-03  
**Purpose:** Compare missing voice patterns from original toolkit against optimized voices folder

---

## Item #5: Casual Teammate Energy Details

### Status: ⚠️ **PARTIALLY PRESENT**

**Original Content from `agent-instructions/voice-rules.md`:**
- **Thinking out loud:** Normalizes not having all the answers, shows reasoning process
- **Playful frustration (when appropriate):** Can express mild frustration with tools/systems, never directed at people, brief and self-aware
- **Clarity over correctness:** Prioritizes being understood over being formal
- **Personal & Emotional:** Weave in subtle opinions, infuse slight humor/curiosity, show you're a person not a machine

### What's Present in Optimized Voices:

✅ **Thinking out loud** - Found in `01-collaborative.md`:
- "I'm thinking..." / "I'm not sure, but..." (line 39)
- Natural entry points that show reasoning process
- Allows uncertainty ("I'm torn between A and B. Both have tradeoffs.")

❌ **Playful frustration** - NOT FOUND
- No examples of mild frustration with tools/systems
- No guidance on when/how to express frustration appropriately

❌ **Clarity over correctness** - NOT EXPLICITLY STATED
- Voice files emphasize clarity but don't explicitly state "prioritize being understood over being formal"
- This principle is implied but not named

❌ **Personal & Emotional** - NOT EXPLICITLY STATED
- Voice files don't explicitly mention weaving in opinions, humor, or curiosity
- "Human > polished" is mentioned but not the emotional/personal nuance aspect

### Recommendation:
- Add playful frustration guidance to `01-collaborative.md` (when appropriate)
- Add explicit "clarity over correctness" principle to voice files or `communication/02-tone-of-voice.md`
- Add "Personal & Emotional" guidance to voice files

---

## Item #6: Emotional Intelligence Patterns

### Status: ⚠️ **PARTIALLY PRESENT IN DIFFERENT FORMS**

**Original Content from `agent-instructions/voice-rules.md`:**

**Feedback Framing:**
- Observation → Impact → Invitation
- "I noticed [specific]. The impact is [specific]. What's your take?"

**Coaching Questions:**
- "What do you need to be successful here?"
- "What's getting in the way?"

**Decision Transparency:**
- "Here's what we're deciding and why it matters..."
- "I'm not sure, but here's what I think so far..."

### What's Present in Optimized Voices:

✅ **Feedback Framing (similar pattern)** - Found in `02-design-critique.md`:
- Structure: Name strengths → Name gaps → Suggest direction
- This is similar but not identical to Observation → Impact → Invitation
- Uses "I'm seeing..." which is observation-based
- Missing the explicit "Impact" and "Invitation" framing

❌ **Coaching Questions** - NOT FOUND
- No explicit coaching question patterns
- Note: `07-selection-guide.md` mentions "Coaching & Feedback" mode but file doesn't exist yet

✅ **Decision Transparency (partial)** - Found in `03-strategic-leadership.md`:
- "Here's why..." (line 44)
- "The rationale: [concise explanation]" (line 45)
- "This matters because [clear impact]" (line 46)
- Missing: "I'm not sure, but here's what I think so far..." (uncertainty transparency)

### Recommendation:
- Add explicit "Observation → Impact → Invitation" pattern to design critique or create coaching voice file
- Add coaching questions to a coaching voice file (when created)
- Add uncertainty transparency patterns to collaborative or strategic leadership voices

---

## Summary

### Fully Present:
- ✅ Thinking out loud patterns (collaborative voice)

### Partially Present (needs expansion):
- ⚠️ Feedback framing (exists but different structure)
- ⚠️ Decision transparency (exists but missing uncertainty patterns)

### Missing:
- ❌ Playful frustration guidance
- ❌ Explicit "clarity over correctness" principle
- ❌ Explicit "Personal & Emotional" guidance
- ❌ Coaching questions patterns
- ❌ Uncertainty transparency ("I'm not sure, but here's what I think so far...")

---

## Recommended Actions

### High Priority:
1. Add playful frustration guidance to `01-collaborative.md` (brief, self-aware, never at people)
2. Add explicit "clarity over correctness" to `communication/02-tone-of-voice.md` or voice files
3. Add "Personal & Emotional" guidance to voice files

### Medium Priority:
4. Add uncertainty transparency patterns to `01-collaborative.md` or `03-strategic-leadership.md`
5. Add explicit "Observation → Impact → Invitation" pattern to design critique or coaching voice

### Low Priority (when coaching voice is created):
6. Add coaching questions to coaching voice file
7. Consolidate emotional intelligence patterns

---

## Files to Review/Update

- `voices/01-collaborative.md` - Add playful frustration, uncertainty transparency, personal/emotional
- `voices/02-design-critique.md` - Consider adding explicit Observation → Impact → Invitation pattern
- `voices/03-strategic-leadership.md` - Add uncertainty transparency patterns
- `communication/02-tone-of-voice.md` - Add "clarity over correctness" principle
- Future: `voices/05-coaching-feedback.md` - Add coaching questions and emotional intelligence patterns
