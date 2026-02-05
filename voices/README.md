# Voices

Specific voice modes for different communication situations. Each mode has distinct patterns, phrases, and tone. Pick one based on audience, goal, and emotional stakes.

---

## Your Choices

| Voice | File | Use When |
|-------|------|----------|
| **Collaborative** | `01-collaborative.md` | Peer problem-solving, aligning on approach, exploring options together |
| **Design Critique** | `02-design-critique.md` | Reviewing UX flows, giving craft feedback, evaluating components |
| **Strategic Leadership** | `03-strategic-leadership.md` | Announcing roadmap, setting strategy, making decisions clear |
| **Leader Conversation** | `05-leader-conversation.md` | Updating a leader, running something by them, briefing without performing |
| **Presenter** | `04-presenter.md` | Presenting to executives, pitching, high-stakes visibility |

### Modes Referenced but Not Yet Built

- **Coaching & Feedback** — Performance reviews, addressing missed deadlines, developmental feedback. Use Collaborative with directness about behavior until this file exists.
- **Caring Manager** — Supporting someone overwhelmed, well-being check-ins. Use Collaborative with emphasis on support until this file exists.

---

## How to Call Them

### When prompting an AI

Reference the file directly:

```
@voices/01-collaborative.md Write a Slack message to Aligning on the token architecture approach.
```

```
@voices/02-design-critique.md Give feedback on this component design.
```

```
@voices/03-strategic-leadership.md Draft an EGDS roadmap announcement for the team.
```

```
@voices/05-leader-conversation.md Draft an email to my VP updating her on the token rollout and one blocker.
```

```
@voices/04-presenter.md Help me summarize our impact for an executive briefing.
```

### When unsure which voice

Use the selection guide:

```
@voices/07-selection-guide.md I'm writing [situation]. Which voice should I use?
```

Or specify audience and goal:

```
I'm writing to [audience] about [goal]. Which voice from @voices should I use?
```

### By name

You can also refer by name in natural language:

- "Use Collaborative voice for this"
- "Write this in Strategic Leadership mode"
- "Apply Design Critique tone"
- "Leader Conversation voice" (05-leader-conversation)

The AI will need to map the name to the file (01-collaborative, 03-strategic-leadership, 02-design-critique, 05-leader-conversation).

---

## Quick Selection

| Situation | Voice |
|-----------|-------|
| Slack to peer about design decision | Collaborative |
| Feedback on component design | Design Critique |
| Roadmap announcement | Strategic Leadership |
| Email to VP with update or running a decision by director | Leader Conversation |
| Executive presentation | Presenter |
| Performance review | Coaching & Feedback (use Collaborative + directness for now) |
| Check-in with burnt-out teammate | Caring Manager (use Collaborative + support for now) |

---

## Decision Tree (Summary)

1. **Who is your audience?** Peer → Collaborative. Designer for craft → Design Critique. Broader team → Strategic Leadership. Leader (updating/briefing) → Leader Conversation. Executive (presenting/pitching) → Presenter.
2. **What's your goal?** Align/explore → Collaborative. Elevate craft → Design Critique. Set direction → Strategic Leadership. Update or run something by a leader → Leader Conversation. Communicate value (formal pitch) → Presenter.
3. **What are the stakes?** Low → Collaborative, Design Critique, Presenter. Medium → Strategic Leadership. High → Caring Manager.

Full decision tree and edge cases: `07-selection-guide.md`
