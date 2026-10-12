---
name: context-brief
description: Turn a spoken ramble into a proper brief, the way you would brief someone who just started in your team. Walks the person through the new-starter brief (what the business does and who the customer is, the job and exactly how it looks when done, what has gone wrong before and how to avoid it), has them say it out loud with Wispr Flow or any dictation, then tidies it into a clean brief and does the job. Use when someone says "let me brief you", "I'll talk you through it", "new-starter brief", "context brief", "help me explain my business to Claude", "why are your answers so generic", or pastes a long voice-dictated ramble and wants the work done properly.
---

# Context brief

AI isn't short on brains. It's short on context. Most people type one line and get an average answer back. The same person can explain their business all day long to a new starter. This skill gets them to do exactly that: talk to Claude like someone who just started in their team, then turn what they said into a brief the work can be done from.

**Done when:** the person has said their brief out loud (or typed it), they have seen it back as a clean brief in one short block, any real gaps are filled, and the job is done from it. If they asked to save the business part, it is saved and they know where.

## 1. Check for a saved business brief

Look for a saved business brief at `~/.context-brief/business.md`. If it exists, read it and say in one line that you have it ("I've got your business brief from before, so we can skip part one."). Then go to step 3.

If there isn't one, start at step 2.

## 2. Ask for the talk-through

Send one short message, in plain English, close to this:

> Talk me through it like I just started in your team. Press your dictation key (in Wispr Flow that's holding **Fn** on a Mac or **Ctrl + Win** on Windows), speak, and let go when you're done. There's no limit, so the more you say, the better the work.
>
> Cover three things:
> 1. **What the business does and who the customer is.**
> 2. **The job you want done, and exactly how it looks when it's done right.**
> 3. **What's gone wrong before, and how to avoid it this time.**
>
> Don't tidy it up. Ums, tangents and examples are all useful.

If they don't have dictation set up and ask how, give them the short setup in [Wispr Flow setup](references/wispr-flow.md). Typing is fine too. Never make dictation a blocker.

If they would rather fill in a form, give them the template in [brief template](references/brief-template.md) and wait.

## 3. Turn the ramble into a brief

When their talk-through arrives, pull it into the shape in [the brief template](references/brief-template.md). Keep their words and their examples. Do not invent facts, customers, numbers, names or results they did not give you. Leave a part blank rather than guess.

Show it back in one short block, headed **Here's your brief**, with the three parts and a one-line "Done looks like" at the bottom. Keep it under about 200 words unless they gave you a lot of detail that matters.

## 4. Fill only the real gaps

Check the brief against [what a good brief needs](references/brief-guide.md). Ask at most three questions in one message, and only for things that would change the result:

- what "done" looks like, if they didn't say (format, length, where it goes, who reads it);
- an example of a good one, if the job has a look or a voice;
- anything that must never happen (sending, spending, deleting, publishing, naming a customer).

If they would rather not answer, pick the safest sensible default, say which in one line, and keep going.

## 5. Do the job

Do the job from the brief. When you hand it over, end with one line on anything you assumed.

If the job is for another tool or person (another chat, a teammate, an agency), hand the brief over as a copy-ready block instead of doing it.

## 6. Offer to save the business part

The first time, ask once: "Want me to save part one (your business and customer) so you never have to say it again?" Only on a yes, write it to `~/.context-brief/business.md` (create the folder if it's missing) and tell them where it is. Never save the job-specific parts unless they ask.

If they give you new business detail later, offer to update the saved file. Show what changes before writing.

## Good to know

- **Speaking beats typing because people say more.** Two minutes of talking is usually far more context than anyone will type. Encourage length, not polish.
- **Keep their voice.** If they said "tradies", don't write "tradespeople". If they said "quote", don't write "proposal".
- **Never ask for passwords, card numbers or private keys** in a brief, and if someone dictates one, tell them to remove it and don't repeat it back.
- **Questions about the method?** Answer from [the brief guide](references/brief-guide.md) in a few plain lines with an example.

Made by Selr AI.

<!-- Provenance marker: sk-1lqkujc --><!-- Provenance signature: ⁠​‌​‌​​‌‌​‌​​​‌​‌​‌​​‌‌​​​‌​‌​​‌​​​‌‌​​​‌⁠ -->
