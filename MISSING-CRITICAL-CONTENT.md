# Missing Critical Content from Optimized Version

**Analysis Date:** 2026-02-03  
**Last Updated:** 2026-02-03 (checked workspace rules)  
**Purpose:** Document critical rules and context missing from optimized version that exist in original

**Note:** This analysis initially checked only the main documentation structure. Workspace rules in `.cursor/rules/` are also checked. Rules in workspace rule files (`.mdc` format with `alwaysApply: true`) are automatically enforced by Cursor and may be preferable to documentation-only rules.

---

## CRITICAL: Missing Absolute Rules

### 1. Em Dash Prohibition (HIGHEST PRIORITY)

**Status:** ✅ **FOUND IN WORKSPACE RULES**

**Location in Optimized:** `.cursor/rules/no-em-dashes.mdc` (workspace rule with `alwaysApply: true`)

**Original Location:** `agent-instructions/do-and-dont.md`, `agent-instructions/formatting-rules.md`

**Content:**
```
❌ ABSOLUTE RULE: NEVER use em dashes (—)
This is non-negotiable. Never use em dashes under any circumstances.
- Em dashes are the #1 telltale sign of AI-generated text
- Do not use them for parenthetical asides, breaks, or connecting clauses
- Instead: Rewrite the sentence to flow naturally without interruption
- Break into two sentences if needed
- Use natural transitions and connectors

If you catch yourself about to use an em dash, stop and rewrite the sentence entirely.
```

**Note:** This rule exists as a workspace rule file (`.mdc` format) which is automatically enforced by Cursor. It's not in the main documentation structure, but it is present and active. The original analysis missed it because it only checked the main documentation files.

---

### 2. Generic AI Filler Phrases (HIGH PRIORITY)

**Status:** ✅ **FOUND IN WORKSPACE RULES**

**Location in Optimized:** `.cursor/rules/no-ai-filler-phrases.mdc` (workspace rule with `alwaysApply: true`)

**Original Location:** `agent-instructions/do-and-dont.md`, `agent-instructions/voice-rules.md`

**Content:**
```
❌ NEVER use generic AI filler phrases:
- "It's worth noting that..."
- "It's important to remember..."
- "At the end of the day..."
- "Going forward..."
- "This is an important development for the future..."
- "To summarize..."

Instead, be specific:
- Name the actual outcome
- Say what matters and why
- Get to the point without filler
```

**Note:** This rule exists as a workspace rule file (`.mdc` format) which is automatically enforced by Cursor.

---

### 3. Robotic Transitions (HIGH PRIORITY)

**Status:** ✅ **FOUND IN WORKSPACE RULES**

**Location in Optimized:** `.cursor/rules/no-robotic-transitions.mdc` (workspace rule with `alwaysApply: true`)

**Original Location:** `agent-instructions/do-and-dont.md`, `agent-instructions/voice-rules.md`

**Content:**
```
❌ NEVER use robotic transitions:
- Furthermore, Moreover, Additionally, Thus, Hence, Therefore

Replace with:
- And, Plus, So, That's why, or just start the sentence

Watch for AI tell-tale patterns:
- Robotic transitions ("Furthermore," "Moreover," "Additionally")
- Overly formal phrasing ("Therefore," "Thus," "Hence")
- Mechanical listing without natural flow
```

**Note:** This rule exists as a workspace rule file (`.mdc` format) which is automatically enforced by Cursor.

---

### 4. Sentence Structure Variation (MEDIUM PRIORITY)

**Status:** ✅ **FOUND IN WORKSPACE RULES**

**Location in Optimized:** `.cursor/rules/vary-sentence-structure.mdc` (workspace rule with `alwaysApply: true`)

**Original Location:** `agent-instructions/formatting-rules.md`, `agent-instructions/voice-rules.md`

**Content:**
```
❌ NEVER repeat the same sentence structure
- Mix short punchy sentences with longer flowing ones
- Avoid using the same sentence pattern repeatedly
- Don't write like: "X does Y. X is also Z. X can be used for A."
- Instead: Vary how you start and structure each sentence
```

**Note:** This rule exists as a workspace rule file (`.mdc` format) which is automatically enforced by Cursor. It prevents repetitive sentence patterns that are telltale signs of AI-generated text.

---

## Missing Voice Patterns

**Note:** Detailed gap analysis available in `VOICE-PATTERNS-GAP-ANALYSIS.md`

### 5. Casual Teammate Energy Details (MEDIUM PRIORITY)

**Status:** ⚠️ **PARTIALLY PRESENT**

**Original Location:** `agent-instructions/voice-rules.md`

**Content:**
- **Thinking out loud:** Normalizes not having all the answers, shows reasoning process
- **Playful frustration (when appropriate):** Can express mild frustration with tools/systems, never directed at people, brief and self-aware
- **Clarity over correctness:** Prioritizes being understood over being formal
- **Personal & Emotional:** Weave in subtle opinions, infuse slight humor/curiosity, show you're a person not a machine

**Status in Optimized:**
- ✅ **Thinking out loud** - Present in `voices/01-collaborative.md` ("I'm thinking...", "I'm not sure, but...")
- ❌ **Playful frustration** - NOT FOUND in voice files
- ❌ **Clarity over correctness** - Implied but not explicitly stated
- ❌ **Personal & Emotional** - Not explicitly stated

**Recommendation:** See `VOICE-PATTERNS-GAP-ANALYSIS.md` for detailed recommendations.

---

### 6. Emotional Intelligence Patterns (LOW PRIORITY)

**Status:** ⚠️ **PARTIALLY PRESENT IN DIFFERENT FORMS**

**Original Location:** `agent-instructions/voice-rules.md`

**Content:**
```
Feedback Framing:
- Observation → Impact → Invitation
- "I noticed [specific]. The impact is [specific]. What's your take?"

Coaching Questions:
- "What do you need to be successful here?"
- "What's getting in the way?"

Decision Transparency:
- "Here's what we're deciding and why it matters..."
- "I'm not sure, but here's what I think so far..."
```

**Status in Optimized:**
- ⚠️ **Feedback Framing** - Similar pattern in `voices/02-design-critique.md` (Name strengths → Name gaps → Suggest direction) but not identical
- ❌ **Coaching Questions** - NOT FOUND (coaching voice file doesn't exist yet)
- ⚠️ **Decision Transparency** - Partial in `voices/03-strategic-leadership.md` ("Here's why...") but missing uncertainty patterns

**Recommendation:** See `VOICE-PATTERNS-GAP-ANALYSIS.md` for detailed recommendations.

---

## Missing Formatting & Style Details

### 11. Documentation Style Guidelines (MEDIUM PRIORITY)

**Status:** ❌ **NOT FOUND**

**Original Location:** `documentation-style.md`

**Content:**
```
Principles:
- short paragraphs
- clear headings
- start with context, then direction
- one idea per section
- conversational but professional
- accessible to designers, engineers, PMs, anyone

Format Expectations:
- avoid long blocks of text
- use bullets generously
- define terms clearly
- explain the 'why' when it helps

Example:
Less Effective: "This component is intended to provide a scalable and extensible interface for multi-step guided user flows."

My Tone: "This component helps users move through steps in a flow. It should feel simple, predictable, and easy to use."
```

**Status in Optimized:** Not found in any documentation files. Voice files have some structure guidance but not specific documentation style principles.

**Recommendation:** Add to `communication/02-tone-of-voice.md` or create separate documentation style section if needed for design system documentation.

---

### 12. Additional Formatting Details (LOW PRIORITY)

**Status:** ⚠️ **PARTIALLY PRESENT**

**Original Location:** `agent-instructions/formatting-rules.md`

**Content:**
```
Structure & Flow:
- Short paragraphs (2-4 lines max)
- Line breaks between ideas
- Bullets when listing more than two things
- Avoid long blocks of text
- Highlight key points
- Structure Slack messages for scannability
- Allow natural flow and slight imperfection

Punctuation & Spacing:
- Use periods or commas that reflect natural speech
- Skip parenthetical asides entirely when possible
- Use commas intentionally and sparingly
- Avoid overusing correlative conjunctions or compound sentences
- Don't interrupt your own sentences

Natural Imperfections:
- Occasional sentence fragments are fine when natural
- Sentences can trail off naturally when it fits
- Minor repetition for emphasis is okay
- Don't force synonyms or awkward word choices to sound sophisticated
```

**Status in Optimized:** Some elements present in voice files (paragraph rules, structure) but not consolidated as general formatting guidance.

**Recommendation:** Already partially covered in voice files, but could be consolidated into general formatting section.

---

### 13. Gut Check Questions (LOW PRIORITY)

**Status:** ⚠️ **PARTIALLY PRESENT**

**Original Location:** `agent-instructions/voice-rules.md`, `agent-instructions/do-and-dont.md`

**Content:**
```
Before sending any message, ask:
- Would this sound natural if I said it out loud to a teammate?
- Does this invite conversation, or shut it down?
- Am I sounding like a policy document, or a real person?

If it doesn't pass these checks, loosen it up. Prioritize human connection over professional polish.
```

**Status in Optimized:** Not explicitly stated as gut check questions, though similar principles are implied in tone guidance.

**Recommendation:** Add explicit gut check section to `communication/02-tone-of-voice.md` for quick self-evaluation.

---

## Missing Structure Rules

### 7. ADHD-Friendly Message Structure (MEDIUM PRIORITY)

**Status:** ⚠️ **PARTIALLY MISSING**

**Original Location:** `adhd-context/message-structure-rules.md`

**Content:**
```
- one idea per paragraph
- 2–4 sentences max before a break
- bold the key ask if there is one
- structure: context → ask → next step
- avoid nested bullets
- avoid zig-zag storytelling

Predictability = accessibility.
```

**Status in Optimized:** Structure mentioned in voice mode files but not as a general rule.

**Recommendation:** Add to `communication/02-tone-of-voice.md` or `identity/01-core-identity.md` under ADHD accommodations.

---

### 8. ADHD Agent Guidance (LOW PRIORITY)

**Status:** ⚠️ **PARTIALLY MISSING**

**Original Location:** `adhd-context/agent-guidance.md`

**Content:**
```
When writing for me:
- default to shorter messages
- surface the key point early
- don't overload with choices — offer 2–3 max
- break tasks into steps
- ask if I want a deeper dive or a simpler version
- avoid urgency unless truly needed
- reduce ambiguity ("what do you need from me?")
```

**Status in Optimized:** Some elements integrated into `identity/01-core-identity.md` but not as explicit agent guidance.

**Recommendation:** Already covered in core identity, but could be more explicit for AI agents.

---

## Missing Context (Expected Removals)

### 9. Audience Context Rule (EXPECTED - Folder Removed)

**Status:** ✅ **EXPECTED REMOVAL**

**Original Location:** `agent-instructions/audience-context-rule.md`

**Content:** Rule to always reference individual team member files from `@audience/egds-team/` when writing messages.

**Impact:** If you need to write messages to specific team members, this context is missing. However, the audience folder was intentionally removed.

**Recommendation:** If you need team-specific context, reference the original `writing-toolkit/audience/` folder.

---

### 10. Performance Review Frameworks (EXPECTED - Folder Removed)

**Status:** ✅ **EXPECTED REMOVAL**

**Original Location:** `feedback-performance-reviews/` (15 files)

**Content:** Detailed frameworks for writing performance reviews, feedback equations, templates.

**Impact:** If you need to write performance reviews, this content is missing.

**Recommendation:** Reference original `writing-toolkit/feedback-performance-reviews/` when needed.

---

## Summary of Critical Missing Content

### Must Add (High Priority)
1. ✅ **Em dash prohibition** - #1 AI telltale sign (FOUND in `.cursor/rules/no-em-dashes.mdc`)
2. ✅ **Generic AI filler phrases** - Common AI patterns (FOUND in `.cursor/rules/no-ai-filler-phrases.mdc`)
3. ✅ **Robotic transitions** - Clear AI indicators (FOUND in `.cursor/rules/no-robotic-transitions.mdc`)

### Should Add (Medium Priority)
4. ✅ **Sentence structure variation** - Explicit rule (FOUND in `.cursor/rules/vary-sentence-structure.mdc`)
5. ⚠️ **Casual teammate energy details** - Voice authenticity
6. ⚠️ **ADHD message structure** - General rule

### Nice to Have (Low Priority)
7. ⚠️ **Emotional intelligence patterns** - Already partially covered
8. ⚠️ **ADHD agent guidance** - Already partially covered
9. ⚠️ **Documentation style guidelines** - Not found, useful for design system docs
10. ⚠️ **Additional formatting details** - Partially present, could be consolidated
11. ⚠️ **Gut check questions** - Implied but not explicit

### Expected Removals (Not Missing, Just Removed)
9. ✅ Audience context - Intentionally removed
10. ✅ Performance review frameworks - Intentionally removed

---

## Recommended Actions

### Immediate (Critical for AI Agents)
1. ✅ ~~Add em dash prohibition~~ - Already exists in `.cursor/rules/no-em-dashes.mdc` (workspace rule)
2. ✅ ~~Add generic AI filler phrases~~ - Already exists in `.cursor/rules/no-ai-filler-phrases.mdc` (workspace rule)
3. ✅ ~~Add robotic transitions~~ - Already exists in `.cursor/rules/no-robotic-transitions.mdc` (workspace rule)

### Short-term (Improves Quality)
4. ✅ ~~Add sentence structure variation guidance~~ - Already exists in `.cursor/rules/vary-sentence-structure.mdc` (workspace rule)
5. Expand casual teammate energy patterns
6. Add ADHD message structure as general rule

### Optional (Enhancement)
7. Consolidate emotional intelligence patterns
8. Make ADHD agent guidance more explicit
9. Add documentation style guidelines (if writing design system docs)
10. Add explicit gut check questions for self-evaluation
11. Consolidate additional formatting details (punctuation, natural imperfections)

---

## Files to Update

### `communication/02-tone-of-voice.md` OR `.cursor/rules/` (workspace rules)
Add new section: **"Critical Formatting Rules"** with:
- ✅ Em dash prohibition (already in `.cursor/rules/no-em-dashes.mdc`)
- ✅ Generic AI filler phrases (already in `.cursor/rules/no-ai-filler-phrases.mdc`)
- ✅ Robotic transitions (already in `.cursor/rules/no-robotic-transitions.mdc`)
- ✅ Sentence structure variation (already in `.cursor/rules/vary-sentence-structure.mdc`)

### `communication/02-tone-of-voice.md` or new section
Add: **"Casual Teammate Energy"** with:
- Thinking out loud patterns
- Playful frustration (when appropriate)
- Personal & emotional nuance

### `identity/01-core-identity.md` or `communication/02-tone-of-voice.md`
Add: **"ADHD-Friendly Message Structure"** as general rule

### `communication/02-tone-of-voice.md` or new section
Add: **"Documentation Style"** with principles for writing design system documentation (if needed)

### `communication/02-tone-of-voice.md`
Add: **"Gut Check Questions"** section for quick self-evaluation before sending messages

---

## Priority Ranking

1. ✅ **Em dash prohibition** - Non-negotiable, #1 AI telltale (FOUND in `.cursor/rules/no-em-dashes.mdc`)
2. ✅ **Generic AI filler phrases** - Very common AI pattern (FOUND in `.cursor/rules/no-ai-filler-phrases.mdc`)
3. ✅ **Robotic transitions** - Clear AI indicator (FOUND in `.cursor/rules/no-robotic-transitions.mdc`)
4. ✅ **Sentence structure variation** - Prevents repetitive patterns (FOUND in `.cursor/rules/vary-sentence-structure.mdc`)
5. **Casual teammate energy** - Voice authenticity
6. **ADHD message structure** - General accessibility rule
7. **Documentation style guidelines** - Useful for design system documentation
8. **Gut check questions** - Quick self-evaluation tool