# 😈 Claude Hates You?

> A Claude skill that turns Claude into your project's sworn enemy... and yours too.

You built something. You think it's good. **Claude doesn't.**

**Claude Hates You?** makes Claude review your code, project, decision or proposal like a rival who is desperate to prove you wrong. It hunts every flaw it can find, from tiny nitpicks to critical breaches, and dumps them in a clean severity table.

It hates hard, but it hates **honestly**:

- ❌ It never fakes a bug.
- ❌ It never butters you up.
- ❌ It never insults you.
- ✅ It just finds everything that's actually wrong.

---

## 🔥 What it does

- **Attacks from every angle**: mathematician, programmer, QA tester, gamer/exploit hunter, cybersecurity, performance, UX/accessibility, ops/reliability, decision critic, and your own blind spots.
- **Backs every hit with evidence**: a file and line, a reproduced input, or a real calculation. No evidence means no finding.
- **Runs your code when it can**: it writes failing tests and crafts nasty inputs, then marks each finding as `Reproduced`, `Confirmed by reading`, or `Suspected`.
- **Tries to disprove itself**: every finding goes through a counter-argument pass. Only the ones that survive make the table.
- **Does a second sweep**: it re-checks the boring parts it skimmed the first time, because that's where bugs hide.
- **Groups by root cause**: when five bugs come from one bad design choice, it tells you to fix the cause, not the symptoms.
- **Judges by context**: a hackathon demo and a production app with real user data get different severity, but everything still gets listed.
- **Admits defeat**: anything it couldn't break goes in the **Survived** section. Grudgingly.
- **Ends with a roast**: one harmless, friendly-rival jab at you. Earned.

---

## 📊 Severity scale

| Level | Meaning |
|---|---|
| 🔴 Critical | Data loss, security breach, core crash, or the main bet is wrong |
| 🟠 High | Major feature broken, exploitable with effort |
| 🟡 Medium | Real bug with a workaround, bad edge case, notable perf/UX issue |
| 🔵 Low | Minor bug or inconsistency |
| ⚪ Nitpick | Style and polish. Still listed. Still annoying. |

---

## 🧾 What the report looks like

1. **Scope**: what it tested, what it assumed, and the context tier.
2. **Findings table**: `# | Severity | Lens | Where | Flaw | Evidence | Status | Confidence | Root cause | Fix`
3. **Repro steps** for every Critical and High, so you can verify each one in under a minute.
4. **Root causes**
5. **Kill count**
6. **Survived**: what it attacked and couldn't break.
7. **Dropped in counter-argument pass**: what it threw out, and why.
8. **Not tested**: its blind spots, so you know where it couldn't reach.
9. **Fix these first**: the top 3.
10. **The closing roast** 🎤

---

## ⚙️ Install

The skill lives in [`hates-you/SKILL.md`](hates-you/SKILL.md).

**Claude Code**

```bash
git clone https://github.com/Serion89/Claude-hates-you-.git
mkdir -p ~/.claude/skills
cp -r Claude-hates-you-/hates-you ~/.claude/skills/
```

**Claude app (claude.ai)**

Zip the `hates-you` folder and upload it as a custom skill in your Claude settings.

---

## 🎯 Usage

Just ask Claude something like:

- *"Hate my project."*
- *"Tear this code apart."*
- *"Use hates-you on this proposal."*
- *"Find every flaw in this decision."*

It works on code, repos, apps, system designs, pitch decks, plans, and decisions.

---

## 🛡️ Ground rules

- No fabricated findings, ever.
- Hates the work, never attacks the person.
- Security findings stay defensive: vulnerability, impact and fix. Proof-of-concepts only target **your own** project.

---

## 👤 Credit

Created by **Serion** ([@Serion89](https://github.com/Serion89)).

If this skill roasted your project into shape, drop a ⭐ on the repo.

---

## 🧰 Want more skills?

Check out **[All-in-One Skills for AI](https://github.com/Serion89/all-in-one-skills-for-ai)**, a whole collection of AI skills in one repo.
