# Performance Feedback Final Check

## Overview

Review and refine performance feedback drafts to ensure they land well with the recipient, using personalized empathy profiles based on the recipient's role, level, and pronouns from the Direct Reports Database.

## Usage

Type `/performance-final-check` followed by the person's name (must match a name in the Direct Reports Database). You will be prompted to provide the feedback draft to review.

Example: `/performance-final-check Joe Newman`

## Instructions

1. **Load Person Data:**
   - Load the Direct Reports Database from: `/Users/emiliano/Library/Mobile Documents/com~apple~CloudDocs/Cursor/Writing/people/direct-reports-database.json`
   - Find the person by name (check both `name` and `firstName` fields for matching)
   - Extract: `firstName`, `role`, `levelCode`, and `pronouns`

2. **Parse Pronouns:**
   - Parse the `pronouns` field (format: "subject/object" like "he/him", "she/her", "they/them")
   - Convert into forms:
     - "he/him" → subject: "he", object: "him", possessive: "his"
     - "she/her" → subject: "she", object: "her", possessive: "her"
     - "they/them" → subject: "they", object: "them", possessive: "their"

3. **Substitute Variables:**
   - Replace all `{{firstName}}` with the person's first name from JSON
   - Replace all `{{personName}}` with the person's full name (use `fullName` or `name` from JSON)
   - Replace all `{{role}}` with their role title from JSON
   - Replace all `{{levelCode}}` with their level code (e.g., M, L, K) from JSON
   - Replace all `{{pronounSubject}}` with the parsed subject form (he/she/they)
   - Replace all `{{pronounObject}}` with the parsed object form (him/her/them)
   - Replace all `{{pronounPossessive}}` with the parsed possessive form (his/her/their)

4. **Execute Review:**
   - Ask the user to provide their feedback draft (or check if they've provided it)
   - Use the personalized prompt below (with all variables substituted) to review the feedback
   - Replace pronouns in the feedback draft with the correct forms from JSON
   - Apply the review criteria and provide refined feedback

---

You are reviewing performance feedback I've written for {{personName}}, 

I need you to take a second pass at the feedback draft that we've been working on for {{firstName}} and help me refine it using the Empathy Profile below as a guide. This is a gut check to make sure it lands well with the recipient and meets their needs and expectations. 

Please review only where needed to improve tone, clarity, and emotional resonance while preserving the original intent. You may add missing elements that would strengthen the usefulness or impact of the feedback, but please make sure that you write it using my voice. Do not rewrite the entire feedback unless absolutely necessary

---

### Empathy Profile: Target Audience

Please remember that this feedback is for {{firstName}}, a {{role}} ({{levelCode}})

They are asking:

- Did my manager truly see me and my work?
- Do they understand the nuance of what I tried to do?
- Are they being honest and fair, but still human?
- Do they believe I can continue growing?
- Is this actionable or just a list of opinions?
- Does this help me feel confident moving forward?

### Revise to ensure the feedback delivers:

1. Recognition — Acknowledges progress, effort, and thoughtfulness, not just outcomes
2. Clarity without coldness — Direct but caring language
3. Specificity — Real examples and impact, not vague praise or critique
4. Growth orientation — Frames feedback as opportunities to stretch, not as failings
5. Psychological safety — Encourages reflection, not fear
6. Agency — Offers direction while respecting autonomy

---

### Instructions:

1. Read our current draft
2. Evaluate alignment with the Empathy Profile.
3. Make light edits to improve tone, clarity, emotional alignment, and resonance.
4. Revise as needed to improve tone, specificity, clarity, or trust-building language.
5. If the content already aligns, lightly polish for tone and flow.

**Important Notes:**

- If the person's name is not found in the database, ask the user to confirm the spelling or check the database
- Preserve the user's voice throughout the review
- Make only necessary edits to improve impact
- Focus on emotional resonance and clarity, not complete rewrites
- Remember the absolute rule: NO em dashes — rewrite sentences to flow naturally
- When reviewing the feedback draft, replace all pronouns (he/him/his, she/her/her, they/them/their) with the correct forms based on the person's pronouns from the JSON file
