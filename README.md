# AI Context Profile — `about_me.md`

A portable, plain-text system for giving AI assistants persistent context about who you are and how you work — without relying on built-in memory features.

Designed for management and leadership roles in government and public sector organizations, where internet access may be restricted and AI session memory is inconsistent.

---

## The Problem

Every time you start a new AI chat session, the assistant knows nothing about you. You re-explain your role, your organization, your preferences. The responses are generic. You spend time correcting the tone. The AI makes assumptions that don't fit your context.

Built-in AI memory features help — but they're inconsistent across tools, unavailable in many secure or air-gapped environments, and opaque about what's actually being retained.

## The Solution

An `about_me.md` file you own, control, and load yourself.

It's a structured markdown document that captures your role, responsibilities, key relationships, writing preferences, and common themes. Load it at the start of any AI session and the assistant immediately understands your context — no re-explanation needed.

Because it's a plain text file, it works everywhere: any AI chatbot, any device, any network environment.

---

## How It Works

```
create_about_me.md  ──▶  AI Interview  ──▶  about_me.md  ──▶  Load every session
   (template)             (5 questions)       (your profile)      (persistent context)
                                                    ▲
                                                    │
                                         Auto-update prompts
                                      at end of project sessions
```

**First time:** Fill in what you know in `create_about_me.md`, load it into an AI chatbot, answer up to 5 refinement questions, and save the generated `about_me.md`.

**Every session after:** Load `about_me.md` at the start. The AI reads it silently and applies your context to every response.

**Over time:** The AI monitors sessions for signals that your profile may be out of date. At a natural break point — after a project wraps up, a priority shifts, or a new key person enters the picture — it asks a single question and proposes a specific amendment for your approval.

---

## Files in This Repository

| File | Purpose |
|---|---|
| `create_about_me.md` | The questionnaire template. Share this with colleagues to help them build their own profile. |
| `about_me_guide.md` | Step-by-step instructions with ready-to-use prompts. |
| `README.md` | This file. |

> **Note:** Your personal `about_me.md` is not included — you generate it yourself using the template. It contains personal and organizational information and should be stored locally or in a private location.

---

## Quick Start

### Step 1 — Fill in the template

Open `create_about_me.md` in any text editor. Fill in **Tier 1** (the required section):

- Your name, title, and department
- A brief description of your role and responsibilities
- The top tasks you'd ask an AI to help with
- Key people you work with

Leave Tier 2 and Tier 3 blank — the AI will help complete those in the next step.

### Step 2 — Start the AI interview

Open an AI chatbot (Claude, ChatGPT, Microsoft Copilot, etc.). Upload or paste the contents of `create_about_me.md`, then send this prompt:

```
I'm uploading my AI context profile template (create_about_me.md).

Please read the full file. I've filled in what I can in Tier 1.

Help me complete and refine my profile by asking me follow-up questions — 
one at a time — to fill in any gaps, clarify my answers, and work through 
Tier 2 (writing style and preferences). Ask me up to 5 refinement questions.

When we're done, generate a clean, complete about_me.md file I can copy 
and save. Write it as if briefing another AI assistant who has never met me.
```

### Step 3 — Answer the questions

The AI will ask up to 5 questions, one at a time. Plain, conversational answers are fine.

### Step 4 — Save your profile

Copy the AI's output and save it as `about_me.md` in a location you can access easily — a desktop folder, shared drive, or USB drive.

---

## Using Your Profile

At the start of any AI session, load your `about_me.md` and send this prompt:

```
I'm sharing my AI context profile (about_me.md). 

Please read it and use it as your background context for our entire 
conversation. You do not need to confirm each detail back to me — 
just apply it. Let me know when you're ready.
```

That's it. The AI will match your tone, understand your role, and anticipate the kind of help you need — for the entire session.

---

## Keeping Your Profile Current

Your profile includes a built-in self-update mechanism.

When you load `about_me.md` at the start of a session, the AI enters **profile monitoring mode**. It quietly watches for signals that something has changed — a new project, a new key relationship, a shift in priorities, or a tone preference you express during the conversation.

At a natural break point, it surfaces a single check-in:

> *"Before we finish — you mentioned a new working group with the Office of Finance that isn't in your profile. Would you like me to suggest an amendment to capture that?"*

If you agree, it shows you exactly what it proposes to change — the section, the current text, and the proposed new text — before asking for your confirmation. You copy the approved update into your file. A change log at the bottom of the profile tracks what was amended and when.

You can also trigger a manual update at any time:

```
I'm sharing my AI context profile (about_me.md).

Please read it, then help me update [describe the section or topic].

Show me the proposed change before finalizing, and give me a 
change log entry I can paste into the Profile Change Log.
```

---

## Profile Structure

The template uses a tiered structure so people can start fast and add depth over time.

**Tier 1 — Core Profile** *(Required)*
The minimum an AI needs to be immediately useful: your identity, role, responsibilities, AI use cases, and key relationships.

**Tier 2 — Working Style & Communication** *(Recommended)*
Your writing tone, how you prefer information delivered, and the recurring themes and language of your work. This is what makes the AI sound like *you*.

**Tier 3 — Organizational & Role Depth** *(Optional)*
Your organization's culture, political dynamics, recurring cycles, and personal working preferences. Fill these in over time as you notice gaps.

---

## Design Principles

**Plain text, no dependencies.** Markdown files work in any environment — no apps, no accounts, no internet required.

**You stay in control.** The AI never modifies your profile automatically. All proposed changes are shown to you first and require your explicit confirmation.

**Works with any AI.** The template is written as instructions the AI reads, not code it executes. It works with Claude, ChatGPT, Microsoft Copilot, Gemini, and any other chatbot that can read a pasted or uploaded text file.

**Built for interrupted environments.** Designed for workplaces with restricted internet access, limited AI tool availability, and no guarantee that session memory persists.

---

## Contributing

Contributions welcome. If you work in a different sector and want to adapt the template — different role types, terminology, or question sets — open a pull request with your version. Please keep the tiered structure and the AI instruction format intact so the self-update mechanism continues to work.

---

## License

MIT License. Use freely, adapt as needed, attribution appreciated but not required.
# Create-About_Me-for-AI
Prompt and template to create an "about_me.md" file that can be used for AI chat.
