# X Tweet Optimizer

Transform draft tweets into algorithm-optimized content using real signals from the [open-sourced X algorithm](https://github.com/xai-org/x-algorithm).

This skill analyzes your drafts against the actual ranking formula (`Final Score = Σ (weight × P(action))`) and rewrites them to maximize positive signals (likes, replies, reposts) while avoiding negative signals (blocks, mutes, reports).

---

## Quick Start

### Clone

```bash
git clone https://github.com/YOUR_USERNAME/x-tweet-optimizer.git
```

Or copy directly to your spawner skills directory:
```bash
cp -r x-tweet-optimizer ~/.spawner/skills/
```

### Use

Feed the `SKILL.md` content as a system prompt to Claude, GPT, or any LLM, then provide your tweet draft:

```
Input: "we just shipped a new feature that lets users export data"

Output: 3 optimized versions + analysis + posting strategy
```

Or invoke directly in Claude Code / Spawner:
```
/x-tweet-optimizer "your draft tweet here"
```

---

## Files

| File | Purpose |
|------|---------|
| `SKILL.md` | Main prompt — the complete optimization system |
| `skill.yaml` | Metadata & algorithm signal weights |
| `patterns.md` | What works: hooks, reply triggers, repost psychology |
| `anti-patterns.md` | What to avoid: spam signals, corporate cringe, rage bait |
| `sharp-edges.yaml` | Algorithmic pitfalls: diversity penalty, negative cascades |

---

## You Are the Creative Engine

**This skill is a compass, not a replacement for voice.**

The optimizer handles structure and signal mechanics:
- Where to place the hook
- How to open curiosity loops
- What triggers replies vs. reposts
- Which patterns the algorithm penalizes

**You bring what it cannot:**
- Your unique perspective and lived experience
- The story only you can tell
- Cultural context and timing instincts
- The weird, specific details that make content memorable
- Knowing when to break the rules

The best viral content isn't optimized — it's authentic content that happens to align with engagement signals. This skill helps you find that alignment without losing your voice.

### The Creative Partnership

Think of it as:
```
Your raw idea (100% you)
    ↓
Skill optimization (structure + signals)
    ↓
Your final edit (reclaim the voice)
```

Always do a final pass. If an optimized version doesn't sound like you on your best day, rewrite it until it does. The skill suggests — you decide.

### When to Ignore the Skill

- When optimization would kill the joke
- When rawness IS the point
- When you're building trust through vulnerability, not hooks
- When your gut says the "unoptimized" version hits harder

The algorithm rewards engagement. Sometimes the most engaging thing is unfiltered honesty that breaks every rule. Trust yourself.

---

## Combining Skills

This optimizer focuses narrowly on X algorithm mechanics. Pair it with complementary skills for better results.

### Grammar & Style Skills (Spawner)

Search for these in your local spawner installation:

```bash
# Find grammar and writing skills
spawner skills search "grammar"
spawner skills search "copywriting"
spawner skills search "writing"
spawner skills search "tone"
```

Recommended combinations:
- **Grammar/proofreading skills** → Clean up before optimizing
- **Copywriting skills** → Sharpen hooks and CTAs
- **Tone matching skills** → Maintain voice consistency across rewrites
- **Storytelling skills** → Structure narratives before optimization

### Workflow Example

```
1. Draft your raw tweet (your ideas, your voice)
2. Run through grammar skill (cleanup typos, clarity)
3. Run through x-tweet-optimizer (structure + signals)
4. Run through tone skill (voice consistency check)
5. Final human edit (make it undeniably yours)
```

The human bookends matter most. You start it, you finish it.

---

## Skills Marketplace

Find more complementary skills at **[skillsmp.com](https://skillsmp.com/)**

Worth exploring:
- Content strategy skills
- Audience research skills
- Thread writing specialists
- Platform-specific optimization (LinkedIn, Threads, Bluesky)
- Hook writing frameworks
- Storytelling and narrative skills
- Personal branding skills

The marketplace has community-contributed skills that slot into your workflow. Mix and match based on what you're building.

### Discovery Tips

```bash
# Browse by category
https://skillsmp.com/category/writing
https://skillsmp.com/category/social-media

# Search for specific needs
https://skillsmp.com/search?q=threads
https://skillsmp.com/search?q=hooks
```

---

## Algorithm Source

Built from analysis of [xai-org/x-algorithm](https://github.com/xai-org/x-algorithm) (Apache-2.0), specifically:

- **Phoenix**: Grok-based transformer for retrieval and ranking
- **Home Mixer**: Feed assembly and scoring pipeline
- **Author Diversity Scorer**: Frequency penalty system

Key algorithmic facts baked into this skill:

| Fact | Implication |
|------|-------------|
| Candidates scored in isolation | Can't "ride" other viral content |
| 15 engagement types weighted | Optimize for high-weight actions |
| Author diversity penalty | Quality > quantity, space out posts |
| Negative signals cascade | One bad tweet hurts future reach |

---

## Example Transformation

**Input:**
```
Transaction heatmap is Mega ready, now I just need to visualize block time comparisons and maybe some other interesting thingies
```

**Weak output (what NOT to do):**
```
🔥 Just finished my transaction heatmap! Block time viz coming soon! #blockchain #dataviz #building
```

**Strong output:**
```
transaction heatmap: done

what should i visualize next?

→ block time comparisons
→ gas patterns
→ your idea

building this live, taking requests
```

The difference: the weak version announces, the strong version invites. Same progress update, but one generates replies and the other gets scrolled past.

---

## Contributing

Found a pattern that works? Discovered a new anti-pattern? The algorithm evolves constantly — this skill should too.

PRs welcome for:
- New patterns with evidence
- Anti-patterns you've seen penalized
- Algorithm changes from X updates
- Voice/niche-specific adaptations

---

## License

MIT — use it, fork it, make it yours.

---

## Final Note

The goal isn't to game an algorithm. It's to say what you mean in a way that actually gets heard.

Optimization without substance is spam. Substance without optimization is a diary.

Find the middle. That's where reach meets meaning.
