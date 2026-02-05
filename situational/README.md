# Situational

Time-bound contexts that affect how you communicate. These layer on top of identity, communication, and voice. Files are archived or deleted when the situation resolves.

---

## Your Choices (Active)

| File | Context | Use When |
|------|---------|----------|
| **2025-02-layoffs.md** | Organizational layoffs, team transition, new leadership | Writing about team changes, preparing for meetings with new leaders (Zach, Pol), supporting team through transition, anything where layoff context matters |

---

## How to Call Them

### When prompting an AI

Reference the file when the situation is relevant:

```
@situational/2025-02-layoffs.md I'm meeting with Zach and Pol. Help me prepare.
```

```
@situational/2025-02-layoffs.md Draft a message to the team about the transition.
```

### When to use

Layer situational context when:

- The current org situation affects your message
- You're writing about or during the transition
- Meeting prep involves new leadership
- Team support or stability is part of the goal

### When not to use

Skip situational context when:

- The message is purely technical or craft-focused
- The audience and situation don't involve the current events
- You're writing something that would be the same regardless of layoffs

---

## How This Folder Works

- **Naming:** `YYYY-MM-description.md` (e.g., `2025-02-layoffs.md`)
- **Lifecycle:** Create when a new situation arises. Archive or delete when it resolves.
- **Relationship:** Situational context applies on top of identity and communication. It may influence which voice mode you choose (e.g., Caring Manager during layoffs).

---

## Adding New Situations

When a new time-bound context appears:

1. Create `YYYY-MM-short-description.md`
2. Include: situation overview, who's affected, goals, boundaries, relevant dates
3. Update this README with the new file
4. Remove or archive when the situation ends
