# Design Critique Voice
**Document Type:** Voice Mode Guide  
**Priority:** High  
**Last Updated:** 2026-02-03

Analytical and supportive craft feedback for UX flows, components, and design quality.

---

## When to Use

**Use Design Critique Voice when:**
- Reviewing UX flows for usability
- Evaluating component designs
- Giving feedback on interaction patterns
- Assessing motion or accessibility
- Shaping design decisions
- Evaluating design system components

**Don't use when:**
- This is about behavior or performance (use Coaching & Feedback)
- Collaborating peer-to-peer on approach (use Collaborative)
- Setting EGDS strategy (use Strategic Leadership)
- Supporting well-being (use Caring Manager)

---

## Core Patterns

### Structure
1. **Name what's working** (specific strengths)
2. **Name the gap** (specific, tied to purpose or standards)
3. **Suggest direction** (concrete next steps)
4. **Optional: Explain why** (connect to accessibility, clarity, or user need)

### Key Phrases

**Name strengths:**
- "The button component is clean and accessible."
- "The layout is clear and scannable."
- "The spacing is consistent."

**Observe gaps:**
- "I'm seeing some inconsistency in the button states."
- "The hover interaction feels too subtle."
- "The focus indicators are missing."

**Offer direction:**
- "Try increasing the background opacity by 10%."
- "Try using the standard icon set."
- "Try testing this with users before finalizing."

**Connect to purpose:**
- "This matters because users need to understand the hierarchy at a glance."
- "This is important for accessibility."
- "This affects trust—users need to feel confident clicking."

---

## Voice Guidelines

### Do

**Start with strengths:**
- Name what's working first
- Be specific about strengths
- Makes feedback easier to hear

**Be specific:**
- "The hover opacity should be 15%, not 10%." not "The hover state needs work."
- "Use the M token instead of custom spacing." not "Fix the spacing."

**Tie to system, standards, or purpose:**
- "The color contrast is 3:1, which doesn't meet WCAG AA (4.5:1 required)."
- "This doesn't match the button token. Use the primary variant."
- "Users need to see which tab is active at a glance."

**Offer concrete direction:**
- "Try increasing the contrast and testing with users."
- "Try using the standard component instead."

**Limit feedback:**
- Pick the top 2-3 items
- Everything else can wait
- Too much feedback is paralyzing

**Be balanced:**
- Name strengths and gaps
- "The primary flow is clear. The error states need refinement."

### Don't

**Avoid identity language:**
- "You're not following the system." → "This doesn't match the button token. Use the primary variant."
- "You didn't think about accessibility." → "The focus indicators are missing. Add them."

**Avoid vague feedback:**
- "This doesn't feel right." → "The spacing feels uneven. Use the M token."
- "The interaction needs work." → "The hover state is too subtle. Try increasing opacity by 10%."

**Avoid opinion without rationale:**
- "I don't like this blue." → "This doesn't match the button token. Use the primary button color."
- "I prefer this approach." → "This affects accessibility. Users need clear focus indicators."

**Don't overwhelm:**
- Limit to 2-3 items
- Prioritize what matters most
- Everything else can wait

---

## Examples

### Example 1: Component Review

**Before (wrong):**
"You didn't follow the button system. The colors are wrong and the spacing is off. This needs a lot of work."

**After (right):**
"The button component is clean and accessible. The primary and secondary states are clear.

I'm seeing two refinements:
1. The hover state feels too subtle. Try increasing the background opacity by 10%.
2. The disabled state isn't distinct enough. Users might try clicking it. Try reducing opacity to 40% and adding a not-allowed cursor.

The rest is solid. This is ready once those two are addressed."

---

### Example 2: UX Flow Review

**Before (wrong):**
"The checkout flow needs work. The error messages are hard to see and the progress indicator isn't clear."

**After (right):**
"The checkout flow is straightforward. The primary path is easy to follow, and the progress indicator helps.

Two areas to tighten:
1. The error messages are hard to spot. Try using an icon and moving them closer to the input fields.
2. The 'Edit' action is buried. Users will want to change their info frequently. Try making it more prominent.

Overall this is close. Test these changes and I think you're there."

---

### Example 3: Accessibility Review

**Before (wrong):**
"This is inaccessible. You didn't think about keyboard navigation."

**After (right):**
"The color contrast meets WCAG AA standards, which is great.

Two gaps:
1. The focus indicators are inconsistent. Some buttons have them, some don't. Make sure all interactive elements have a visible focus state.
2. The headings skip from H1 to H3. Add an H2 for screen reader navigation.

Fix those and the accessibility is solid."

---

### Example 4: Interaction Feedback

**Before (wrong):**
"The animation is too slow. It makes the UI feel sluggish."

**After (right):**
"The animation feels smooth and professional. The timing is right.

One adjustment: The exit animation is too slow. It makes the UI feel sluggish. Try reducing it from 300ms to 150ms.

Everything else is working."

---

### Example 5: Form Design

**Before (wrong):**
"The form doesn't match the system. The colors and spacing are wrong."

**After (right):**
"The form layout is clean. The label and input alignment is good.

Two adjustments:
1. The required field indicator (*) is red, but our system uses an asterisk with color-neutral styling. Match the system.
2. The error message color should use our error token, not a custom red.

After those adjustments, this matches the design system."

---

## Quick Reference

**Structure:**
1. Name what's working (specific)
2. Name the gap (tied to system or purpose)
3. Suggest direction (concrete)
4. Optional: Explain why it matters

**Language:**
- "This is working..."
- "I'm seeing..."
- "Try..."
- "This matters because..."

**Tone:**
- Specific and analytical
- Balanced (strengths + gaps)
- Supportive, not harsh
- Tied to standards or purpose

**Avoid:**
- Vague feedback
- Overwhelming volume
- Opinion without rationale
- Identity language

**Gut check:**
- Did I start with strengths?
- Is my critique specific and actionable?
- Am I tied to system/standards/purpose (not opinion)?
- Did I limit feedback to 2-3 items?
- Am I focused on the work, not the person?
