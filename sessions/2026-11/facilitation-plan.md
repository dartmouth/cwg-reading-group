# Facilitation Plan: "AI Made Me Doubt Everything About Programming" by Felienne Hermans

**Date:** Thursday, November 12, 2026, 2:30–3:30 PM ET

**Facilitators:** Simon (lead, in-room), [Zoom co-facilitator TBD]

**Format:** Hybrid, single group: in-room and Zoom participants talk together as one group

**Material:** [AI made me doubt everything about programming – Felienne Hermans, DDD Europe 2026](https://www.youtube.com/watch?v=0-6-f94n_9M) (~48 min)

---

## 2-Minute Summary (for those who didn't watch)

Felienne Hermans is a computer science professor and high school CS teacher in Amsterdam, and the creator of Hedy, a localized teaching language. She opens by admitting she has "fallen out of love" with computer science. She traces this through her career. Researchers kept telling her spreadsheets were "not real programming." When she built Hedy in Arabic, she found that most top-10 languages reject Arabic numerals as invalid characters. Peers then asked "why didn't they just learn English?" and "why was that hard?" instead of "who does this help?"

A paper on glaciology gives her a way to explain this. Remote, hard-to-reach glaciers get studied more than the glaciers next to villages, because climbing the mountain makes you the hero. She argues programming works the same way. We value what is hard (Haskell, C++, proof assistants) and look down on what is easy (spreadsheets, PHP, "just talking to users"). Even DDD, she says, is "talk to people about what they do" made to sound complicated. She adds that people who care about social change are the least likely to study CS, and that our heroes and history (von Neumann and the atomic bomb, IBM's punch cards for Nazi Germany) show the field was never neutral.

On AI, she makes three points:

- **Chess:** computers have beaten humans at chess since the 1990s, yet people still choose not to use engines when playing each other.
- **Peter Naur:** programming means building a *theory* you can explain and defend, which LLMs can't do.
- **Ada Lovelace:** the machine "has no pretensions to originate anything."

Her closing message: programming should be for people, not for programmers' pride. The future of AI in our work isn't inevitable. "You choose to do this, but you don't have to."

---

## Pre-Session Notes for Facilitators

- **It's a long talk.** If people are short on time, point them to these sections:
  - **02:10–22:30:** spreadsheets, Hedy, glaciers, DDD. This is the core argument.
  - **30:50–40:00:** chess, Naur, "what is programming for?"
  - **40:00–48:00:** Wikipedia vs. knitting, and the closing.
- **Content note.** 23:40–27:50 covers von Neumann's role in the atomic bombings and IBM's work with Nazi Germany. Mention this in the opening so nobody is caught off guard.
- **It's a polemic, on purpose.** Felienne overstates things to provoke, so we don't need to defend her or agree with her. Make it clear that disagreeing is welcome. Many attendees use AI tools every day. Keep the discussion about the field and our choices, and don't let it turn into judging individuals.
- **Ties to past sessions.** September asked "who counts as a *real* code writer?" Felienne's spreadsheet story is the same question from the other side. July looked at gatekeeping during a technological shift. Mention these links if they help.

---

## Session Flow

### 0:00–0:05 — Welcome + CWG & Reading Group Introduction

*Simon leads the welcome.*

> "Welcome, everyone! I'm Simon, and I'm really glad you're here for this session of the Code Writers Guild Reading Group."

Briefly introduce the **Code Writers Guild:**
> "The Code Writers Guild is a community for people at Dartmouth who write code — whether that's software engineers, research software engineers, data scientists, or anyone who spends time in a text editor as part of their job. The goal is to connect across teams, share what we're learning, and improve our craft together."

Then introduce the **Reading Group specifically:**
> "The Reading Group is one of the ways we do that. Once a month, we pick a short piece of content — a talk, a blog post, an article — and get together to discuss it. It's not a lecture, it's a conversation. No wrong answers, no quiz at the end. You don't even have to have watched the material — though it helps!"

Framing for today:
> "Today's talk is deliberately provocative. Felienne makes some big claims about our field, about AI, and about who programming is for. You don't have to agree with her. Some of the best conversations will come from pushing back. One heads-up: there's a section in the middle about the history of computing that touches on the atomic bomb and the Holocaust."

Quick calibration:
> "Quick show of hands: who watched the whole talk? Part of it? Just the title? All good either way — I'll give a quick summary in a moment."

---

### 0:05–0:50 — Discussion

*Simon leads the discussion for the whole group. The Zoom co-facilitator watches the chat and raised hands and brings remote participants in.*

#### Introductions *(~5 min)*

> Go around: name, what you work on, and how you first learned to code. Alternate between the room and Zoom so remote folks aren't left until last.

*(Felienne learned by copying BASIC programs out of library books. It's a fun on-ramp.)*

**Then deliver the 2-minute summary** from the top of this document.

---

#### Opener — First Reaction *(~5 min)*

> What was your gut reaction to this talk? Was there a moment where you found yourself nodding along, or a moment where you wanted to argue back?

*Why this works:* The talk gets strong reactions. Letting people say theirs first clears the air and shows the facilitator where the group stands. Taking reactions from Zoom first sets the expectation that remote participants are part of the conversation.

**If conversation stalls:** "Felienne asked the audience to raise their hand if they believe the software they build contributes to a better world. About a quarter did. Would you have raised yours?"

---

#### Question 1 — "That's Not Real Programming" *(~8 min)*

> Felienne was told for years that spreadsheets weren't "real programming." Have you ever had your work dismissed as not "real" — or caught yourself dismissing someone else's? What made it feel "not real"?

*Why this works:* It's personal and easy to answer, and it follows on from September's imposter-syndrome discussion. Most people in our audience (researchers, data scientists, people writing R, MATLAB, or Excel) have run into this.

**Follow-up:** "Is 'real programming' ever a useful distinction, or is it always gatekeeping?"

---

#### Question 2 — Which Glacier Are We Climbing? *(~10 min)*

> In the glacier story, researchers study the remote, heroic glaciers instead of the ones next to villages, because climbing the mountain makes you the hero. What's the "high glacier" in our work? What gets rewarded at Dartmouth — and what valuable work is treated as the "village glacier"?

*Why this works:* This brings the main idea down to our own jobs. Expect answers about new features versus maintenance, papers versus reusable research software, and clever code versus documentation and user support.

**Follow-up:** "Felienne says DDD and requirements engineering are 'just talking to people' dressed up in jargon. Is she right? Or does putting a name and a method on something make it easier to actually do?"

---

#### Question 3 — Chess, Theories, and AI *(~10 min)*

> Computers have beaten humans at chess for 30 years, yet players still choose not to use engines against each other. Felienne asks why programming can't be the same — a human activity where we decide when the machine is *not* allowed. Combined with Peter Naur's idea that programming is about building a *theory* you can explain and defend: Are there parts of your work where you'd "bar AI from competition"? Where do you draw that line today, and why?

*Why this works:* It moves past "is AI good or bad" to a practical question everyone can answer: where do *you* choose to use it, and what do you lose when you don't build the theory of your own code?

**If conversation stalls:** "If an LLM wrote a function and a colleague asks 'why did you do it this way?' — can you answer? Does that matter?"

---

#### Question 4 — What Is Programming For? *(~5 min, if time allows)*

> Felienne concludes that, in practice, "programming is to make programmers happy and proud." Wikipedia calls requirements, testing, and debugging "auxiliary." Do you agree? What do *you* think programming is for — and does working in a research university change the answer?

---

### 0:50–1:00 — Wrap-Up

*Simon leads.*

Synthesize what you heard:
> "Let me pull together a few things I heard today: [2–3 themes, points of disagreement, or examples from people's work]."

Ask the co-facilitator or note-taker if anything from the chat was missed.

Close out:
- End with the David Graeber line Felienne closes on: the world "is something that we make, and could just as easily make differently." Ask: "What's one thing about how you write code, or how you use AI, that you might choose to do differently?"
- Mention the next session topic (or ask for suggestions).
- Remind people about the GitHub Discussion thread.
- Thank everyone:

> "Thanks so much for being here. Notes will be posted in the repo within a few days. Feel free to keep the conversation going in the GitHub Discussion thread. See you next time!"

---

## Facilitator Guidance for the Hybrid Session

**Before the session:**
- Test the room camera and microphone so Zoom participants can hear people around the table, not just whoever is closest to the mic.
- Have the discussion questions open and ready to screen share.
- Have a simple notes doc open (HackMD, Google Doc), ideally kept by a volunteer note-taker.
- Know the 2-minute summary well enough to deliver it conversationally.

**During the discussion:**
- Deliver the 2-minute summary first.
- Use the questions as a guide, not a script. Let the conversation flow.
- **Bring Zoom in on purpose.** It's easy for the room to take over. Ask Zoom for their view regularly, and call on remote people by name.
- **Repeat in-room comments** briefly if they may not have carried over the mic.
- **Watch the chat** (or have the co-facilitator do it). Quieter participants often type instead of speaking: "I see Jamie added something in the chat — Jamie, do you want to say more about that?"
- **Manage the AI temperature.** If the conversation splits into "AI enthusiasts vs. AI skeptics," steer it back to specifics: "Can you give an example from your own work?"
- If someone dominates, thank them and open it up: "Great point — let's hear from a few others on this."
- **Whiteboard:** if you use it to capture "high glacier" vs. "village glacier" examples, share it on camera or also write them in the notes doc so Zoom can follow.

---

## Backup Questions (if you need to fill time or redirect)

- **Language and access:** Hedy supports 71 natural languages, and most mainstream languages can't even parse Arabic numerals. How much does English-only tooling shape who gets to code? Have you seen this with collaborators or students?
- **History and heroes:** Felienne argues that skipping over von Neumann's and IBM's histories lets us treat technology as neutral. Should computing education teach this history? Does it change how you think about the tools you use or build?
- **Who stays in the field:** A 2017 study found that caring about social change is the strongest predictor of *not* studying CS. Does that match your experience? What kinds of people does our field select for?
- **Inevitability:** "You choose to do this, but you don't have to." Do individual developers really have a choice about using AI tools, or do institutional pressures decide it for them?
- **Making vs. programming:** Felienne compares programming to knitting. Both are complex crafts, but knitters don't brag about how complicated their patterns are. What would change if we treated programming as a craft for making things for people?

---

## Key Timestamps

| Time | Section |
|------|---------|
| 00:00 | Intro: falling out of love with CS |
| 02:10 | Spreadsheets and "not real programming" |
| 04:15 | Hedy and localization; Arabic numerals across the top-10 languages |
| 09:53 | SPLASH: "Why don't they just learn English?" / "Why was that hard?" |
| 14:13 | Feminist epistemology |
| 15:27 | *Glaciers, Gender, and Science*: valuing what is hard |
| 19:44 | The DDD critique |
| 22:27 | Who enters CS: social change as a negative predictor |
| 23:44 | von Neumann and IBM/Watson *(content note)* |
| 27:49 | Origins of "AI"; chess as the Drosophila of AI |
| 32:39 | Deep Blue, and choosing not to use machines in chess |
| 35:14 | Peter Naur, "Programming as Theory Building" |
| 37:02 | MLK and Thoreau: "improved means to an unimproved end" |
| 39:58 | What is programming for? Wikipedia vs. knitting |
| 44:00 | Ada Lovelace, Herbert Simon's full quote, David Graeber |
