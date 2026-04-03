# Facilitation Plan: "All the Little Things" by Sandi Metz

**Date:** April 9, 2026, 2:30–3:15 PM ET
**Facilitators:** Simon (in-room), Beaudry (Zoom, Group 2), Will (Zoom, Group 3)
**Format:** Hybrid — 1 in-room group + 2 Zoom groups, each with a dedicated facilitator
**Material:** [All the Little Things – RailsConf 2014](https://www.youtube.com/watch?v=8bZh5LMaSmE) (~38 min)

---

## 2-Minute Summary (for those who didn't watch)

Sandi Metz takes the Gilded Rose Kata — a notoriously tangled 43-line `if` statement — and refactors it live on stage. She starts by extracting small methods, then graduates to small objects, and ends up with code whose complexity drops by roughly 75%. Along the way she makes several provocative claims: duplication is far cheaper than the wrong abstraction, intermediate refactoring steps *will* make things worse before they get better, and the principles of OO design (especially Open/Closed) are what give you the confidence to push through that intermediate pain.

---

## Session Flow

### 0:00–0:05 — Welcome + CWG & Reading Group Introduction

*Simon leads. This is the first meeting, so take a moment to orient everyone.*

> "Welcome, everyone! I'm Simon, and I'm really glad you're here — this is the very first session of the Code Writers Guild Reading Group."

Briefly introduce the **Code Writers Guild:**
> "The Code Writers Guild is a community for people at Dartmouth who write code — whether that's software engineers, research software engineers, data scientists, or anyone who spends time in a text editor as part of their job. The goal is to connect across teams, share what we're learning, and improve our craft together."

Then introduce the **Reading Group specifically:**
> "The Reading Group is one of the ways we do that. Once a month, we pick a short piece of content — a talk, a blog post, an article — and get together for 45 minutes to discuss it. It's not a lecture, it's a conversation. No wrong answers, no quiz at the end. You don't even have to have watched the material — though it helps!"

Quick calibration:
> "Quick show of hands: who watched the whole talk? Partway through? Just caught the description? All good either way — I'll give a quick summary once we're in our groups."

---

### 0:05–0:10 — Hybrid Logistics + Group Split

*Simon leads. Explain the plan and get everyone sorted before the clock starts on discussion.*

> "Here's how today works. Because we have people in the room and people on Zoom, we're going to split into three small groups — that way everyone gets a real conversation, not a big awkward hybrid call."

Explain the groups:
> "Group 1 is here in the room with me. Groups 2 and 3 are on Zoom — Beaudry is leading Group 2 and Will is leading Group 3. Each group will have the same discussion questions, so at the end we'll come back together and compare notes."

Logistics:
> "If you're on Zoom, you should be getting moved into a breakout room now. Each breakout room has a facilitator — you'll see Beaudry or Will in there with you. We'll bring everyone back together at 2:35."

*[Move Zoom attendees into breakout rooms. Confirm in-room group is settled.]*

> "Any questions before we split? … Great. Let's go!"

---

### 0:10–0:35 — Breakout Group Discussion

*Each facilitator runs this section independently with their group. All three groups use the same questions below.*

**Start with the 2-minute summary** so everyone has shared context before diving in.

> "Let me give a quick summary for anyone who didn't get to the full talk..."
> *[Deliver the summary from the top of this document.]*

---

#### Question 1 — The Squint Test *(~5 min)*

> Sandi introduces the "squint test" — lean back, squint at your code, and look for changes in shape (nesting) and color (mixed abstraction levels). Have you ever had a visceral, gut-level reaction to code complexity before you fully understood the code? What signals do you use to sense that code is in trouble?

*Why this works:* Low barrier to entry. Everyone has stared at ugly code. Gets people talking from personal experience rather than theory.

**If conversation stalls:** "Think of the last time you opened a file and immediately groaned. What was it about the code that triggered that reaction?"

---

#### Question 2 — "Duplication is far cheaper than the wrong abstraction" *(~10 min)*

> Sandi argues that we teach beginners DRY first because it's the only thing they can recognize — but that experienced developers should be willing to tolerate duplication and wait for a better abstraction to emerge. Do you agree? Can you think of a time when you (or your team) DRY-ed up code too early and ended up fighting the resulting abstraction?

*Why this works:* This is the talk's most quotable and debatable claim. It directly challenges something most of us treat as gospel. Should generate genuine disagreement.

**Follow-up probes if needed:**
- "What does it feel like when you're working with the *wrong* abstraction? How do you recognize it?"
- "She suggests using 'dup tags' to track duplication instead of immediately removing it. Would that fly in a code review on your team?"
- "Is there a threshold — a number of duplicates, or a level of complexity — where you'd say 'OK, now it's time to abstract'?"

---

#### Question 3 — Connecting to Our Work *(~8 min)*

> A lot of us work on research software, data pipelines, or internal tools that may not look like a Rails app. Where do you see the ideas from this talk applying to the kind of code you write? Are there patterns from the talk — small objects, Open/Closed, separating configuration from logic — that feel especially relevant or especially *ir*relevant to your work?

*Why this works:* Grounds the discussion in participants' actual contexts. Research software often has different constraints (small teams, domain experts writing code, "write once" scripts that quietly become infrastructure).

**⚠️ Wrap up your group at 0:33** (two minutes before reconvene) and ask your group:
> "Before we head back — what's the one thing from our discussion you'd most want to share with the other groups?"

*Note down 2–3 highlights to bring to the share-out.*

---

### 0:35–0:45 — Reconvene + Share-Out + Wrap-Up

*Simon leads. Bring Zoom participants back from breakout rooms at 0:35.*

> "Welcome back, everyone! Let's hear from each group. Beaudry, can you kick us off — what were the highlights from your group?"

Each facilitator shares **2–3 highlights** from their group (~2 min each):
- What sparked the most debate?
- Any surprising takes or examples from people's real work?
- Any strong agreement or disagreement with Sandi's claims?

After all three groups have shared, Simon synthesizes:
> "A few things I'm noticing across all three groups: [2–3 common themes or interesting contrasts]."

Close out:
- "What's one thing from today you might actually try or think about differently?"
- Mention the next session topic (or solicit suggestions).
- Remind people about the GitHub Discussion thread for continuing the conversation async.
- Thank everyone:

> "Thanks so much for being here — especially for joining us for the very first session. Notes will be posted in the repo within a few days. Feel free to keep the conversation going in the GitHub Discussion thread. See you next month!"

---

## Facilitator Guidance for Breakout Groups

*This section is especially for Beaudry and Will running the Zoom groups.*

**Before the session:**
- Have the discussion questions open and ready to screen share.
- Have a simple notes doc open (HackMD, Google Doc) to capture highlights for the share-out.
- Know the 2-minute summary well enough to deliver it conversationally.

**During the breakout:**
- Deliver the 2-minute summary first, even if some people watched the talk.
- Use the questions as a guide, not a script — let the conversation flow.
- **Watch the chat.** On Zoom, quieter participants often type instead of speaking. Invite them in: "I see Jamie added something in the chat — Jamie, do you want to say more about that?"
- If someone dominates, thank them and open it up: "Great point — let's hear from a few others on this."

**For the in-room group (Simon):**
- Use the whiteboard if it helps to capture ideas visually.
- Make eye contact around the table to invite quieter participants in.

**Two minutes before reconvene:**
- Wrap up the current thread.
- Ask: "What's the one thing you'd most want to share with the other groups?"
- Jot down your 2–3 highlights — you'll be sharing them in the full-group debrief.

---

## Backup Questions (if you need to fill time or redirect)

- **On tolerating intermediate complexity:** During the refactoring, every intermediate step made the Flog score *worse* — the code got more complex before it got simpler. Sandi says you need to "trust the principles" to push through. In practice, how do you (or your team) handle this? Have you ever abandoned a refactoring partway through because the intermediate state felt too risky or messy?
- **On metrics:** "She says 'metrics are fallible, but opinions are no more precise.' How do you feel about using code metrics (cyclomatic complexity, Flog, etc.)? Does your team use any?"
- **On Open/Closed:** "The Open/Closed Principle says you should be able to add new behavior without editing existing code. That sounds impossible. Can you think of a time your code was set up this way — or a time you wished it had been?"
- **On naming:** "She calls Gilded Rose an 'item factory' once she strips away the middleman logic. How much does finding the right *name* for what code is doing help you see the right design?"
- **On the Kata format:** "The Gilded Rose is a refactoring kata — you can't change the tests, you can only change the code. Has anyone here used katas or exercises like this to practice? Is that something we'd want to try as a group activity?"

---

## Tips for This Specific Session

- **This is the first meeting.** Be warm and welcoming in the intro. Some people may not know anyone else in the group. The logistics explanation is especially important — don't rush it.
- **The talk is long (~38 min).** Some people won't have watched it. The summary and the questions are designed to work even if people only caught the gist.
- **Ruby-specific syntax** might be unfamiliar to some. If someone gets hung up on Ruby details, redirect: "The specific language doesn't matter as much as the *pattern* — what would this look like in your language?"
- **The DRY vs. abstraction question (Q2) is your strongest card.** If you're short on time, spend the most time here — it generates the richest debate.
- **Watch for the "well, actually" trap.** Some people may want to debate whether Sandi's specific OO approach is the *right* approach vs. functional programming, pattern matching, etc. That's fine for a few minutes, but redirect to the underlying principles if it goes too long.
- **Zoom facilitators:** If your group is quiet, try a quick round-robin: "Let's go around quickly — one word or phrase that comes to mind from the talk."
