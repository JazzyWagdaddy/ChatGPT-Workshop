# Hands-On Lab: ChatGPT Custom Instructions, Projects, Skills and Apps

You set up four ChatGPT personalization features in about 20 minutes and leave with a rule for choosing among them. Two things differ from the Claude version of this lab. ChatGPT now calls connectors apps, and skills are limited to certain plans, so Exercise 3 includes a fallback.

## Before you start

Get these ready before the clock starts:

- A ChatGPT account for this lab. Check your plan first, because skills (Exercise 3) and apps (Exercise 4) depend on it.
- One real file or a few related files on your laptop. A template, a policy doc, a past deliverable. Anything you would normally attach to an email.
- Notifications off. You need 20 uninterrupted minutes.
- Use ChatGPT in a browser. Some project features, including project-only memory, may be missing from the desktop and mobile apps.

## The four features in one line each

Each feature answers a different question: how should ChatGPT always behave, what does it need to know about this subject, how should it do this task, and where does the live data sit.

| ChatGPT feature | What it does | Where it applies |
| --- | --- | --- |
| Custom instructions | Standing preferences that shape every response | Every conversation, everywhere |
| Projects | A workspace with files, chats, and instructions for one ongoing subject | Only inside that project |
| Skills | A reusable workflow ChatGPT follows when a task calls for it | Any chat where the skill is available |
| Apps (formerly connectors) | A live link to an outside service such as Gmail or Google Drive | Any chat where you turn the app on |

---

## Exercise 1: Custom instructions

**Goal:** Set a standing preference and watch it apply without asking.

**Steps**

1. Click your profile icon in the bottom left and open Settings.
2. Go to Personalization and find the Custom instructions field.
3. Write two sentences. One about your role, one about how you want ChatGPT to respond. Example:

```text
I run onboarding for a 40-person sales team. Keep answers under 150 words and skip the caveats.
```

4. Save it.
5. Start a brand-new chat, not inside a project, and ask something generic, such as "how do I run a good 1:1?"

**What to notice:** ChatGPT answered in your style without you asking. It now applies to every future chat. Make a few more iterations based on your role and persona, save each change, and open a new chat to check the result.

**Reflection question:** Would this same preference cause a problem in a totally different context, like a legal memo? If yes, it is too broad for custom instructions. That is your signal to use a project instead.

---

## Exercise 2: Projects

**Goal:** Build a workspace that already knows a specific subject before you type a word.

**Steps**

1. Click Projects in the left sidebar, then New project.
2. Name it something specific. Not "Work." Try "Q4 Client Onboarding." Add a name, icon, and color. A project can be shared with teammates or kept private.
3. Under More options, choose the memory setting. Default memory lets the project draw on your saved memories. Project-only memory limits ChatGPT to chats and files inside the project. Choose it when you create the project, because you may not be able to change it later.
4. Open the project and add project instructions. Tell ChatGPT who it is working for in this one context only. You write the role, tone, and rules once, and every chat started inside the project inherits them along with the project files.
5. Upload a file that is relevant to this project.
6. Upload two or three more related files. ChatGPT projects take individual files rather than folders, so select the files from the folder you would have added.
7. Start a new chat inside the project and ask a question that depends on those files. Be creative and use the T-C-O framework.

**What to notice:** ChatGPT used the files without you attaching them to the chat. Every new chat inside the project starts already briefed. Chats outside the project do not carry any of this. Project instructions also override your global custom instructions inside the project.

**Reflection question:** Custom instructions apply everywhere. Project instructions apply only inside one project. What recurring subject in your own work deserves its own project?

---

## Exercise 3: Skills

**Goal:** Watch ChatGPT apply a procedure on its own, only when the task calls for it.

**Plan check first.** OpenAI lists skills for eligible ChatGPT Business, Enterprise, Healthcare, and Edu accounts, subject to workspace settings. If you do not see a Skills page, skip to the fallback at the end of this section.

### Install an existing skill

1. Open the Skills page from the sidebar.
2. Check the Installed, Created by me, Shared with me, and Shared by your workspace tabs. Eligible accounts include one skill by default, skill-creator.
3. If a teammate or your workspace has shared a skill, open its more options menu and select Install.
4. Open a new chat. Ask for a task the skill covers, or type @ and the skill name to select it explicitly.

**What to notice:** You did not have to paste the procedure. ChatGPT can pick a relevant skill automatically, and the @ mention is there when you want to force it. It works the same way inside a project or in a plain chat.

### Create your own skill

1. Choose something you or your team does the same way every time. Formatting meeting notes into action items, writing a weekly status update, converting a transcript into a client-ready summary. The narrower the task, the more useful the skill. Avoid vague goals like "write better emails."
2. Write down what good looks like. Grab a real example of the task done well, with the input and the output you want. This is the biggest factor in whether the skill works.
3. On the Skills page, select Create, then Create with chat. You can also ask ChatGPT to create a skill in any chat. It uses skill-creator, asks follow-up questions, and prompts you to install the result.
4. Paste your example. Try one of these prompts:

```text
Create a skill that makes all my responses sound like they are coming from <your favorite TV character>.
```

```text
I want a skill that turns raw meeting notes into a table of action items with owners and due dates. Here is an example of notes and the table I want back.
```

5. Check the name and description. ChatGPT uses the description to decide when to apply the skill, so it must say exactly what the skill is for. "Formats raw meeting notes into an action-item table with owners and due dates" works. "Helps with meetings" is too vague to trigger reliably.
6. Test it in a new chat with a different set of notes. Confirm the skill fires and the output matches the pattern you taught. If it does not trigger, tighten the description.
7. Refine one thing at a time. Tell ChatGPT what to fix, ask it to update the skill, and re-test. Changing five things in one edit hides which change worked.

**Fallback if your plan has no skills:** Build a custom GPT with the same instructions and example in its configuration. It is a reusable, configured tool you open on demand, so it does not load automatically the way a skill does. Teach the difference when you present this exercise.

**Reflection question:** A skill holds procedural knowledge, the how of a task. A project holds background knowledge, the what and who of a subject. Where is the line for something you do the same way every week, like formatting a status report?

---

## Exercise 4: Apps (formerly connectors)

**Goal:** Give ChatGPT access to a live outside source instead of a file you handed it.

OpenAI renamed connectors to apps on December 17, 2025. Your settings may say Apps, Connectors, or both, depending on your account.

**Steps**

1. Open Settings and go to Apps. If you see Connectors instead, use that.
2. Pick one you actually use, such as Google Drive, Gmail, or Slack, and connect it. Complete the sign-in.
3. Ask a question that requires current data, not a document. Example: "What is on my calendar tomorrow?" or "Find my most recent email from [name]."

**What to notice:** ChatGPT did not summarize a file you gave it. It pulled the current record. That is the core difference. Apps read live systems. Projects and skills work with content you have directly provided.

**Notes by plan**

- Google Docs, Sheets, and Slides actions now sit inside the Google Drive app. Connect Google Drive for all of them.
- On Enterprise and Edu, those Google Drive actions are off until a workspace admin enables them. Ask your admin if the connection fails.
- Reports conflict on whether free accounts can connect apps. Confirm in your own settings before you teach this step.

---

## Wrap-up: the decision framework

Ask these questions in order. Stop at the first yes.

1. **Does this need to apply to every conversation, regardless of topic?** Use custom instructions.
2. **Is this an ongoing subject with its own files and context?** Use a project.
3. **Is this a repeatable task you want done the same way, anywhere you work?** Use a skill, or a custom GPT if your plan has no skills.
4. **Do you need ChatGPT to see live, current data instead of a document you give it?** Use an app.

**The mistake to watch for:** People stuff formatting and tone rules into every new project's instructions, then wonder why every project feels like starting from zero. Project instructions override your global custom instructions, so a preference that applies everywhere belongs in custom instructions once, not copied into each project.

---

## What to verify before you teach this

Five items depend on plan or interface and should be checked in a live account first. Three changes from the Claude original are deliberate.

| Item | Issue | Confidence |
| --- | --- | --- |
| Skills availability | OpenAI's help page lists Business, Enterprise, Healthcare, and Edu. Your plan may differ | Medium |
| Apps on free plans | Two sources disagree on whether free accounts can connect apps | Low |
| Project memory setting | One source says choose at creation only. Another says eligible unshared projects can switch later | Medium |
| Settings labels | Custom instructions sit under Personalization in most guides. Some older ones say Customize ChatGPT | Medium |
| Desktop and mobile apps | Older reports say project-only memory and some project features are web-first | Medium |
| Dropped: /learn skill and Browse skills | No matching ChatGPT built-in was confirmed, so Exercise 3 uses shared skills and skill-creator | High |
| Dropped: Claude Styles | The Claude lab points to Styles. This version points to projects instead | High |
| Kept: T-C-O framework | Carried over unchanged from the original. Confirm it matches your workshop deck | High |

## Sources

Adapted from the [Claude-Workshop lab](https://github.com/JazzyWagdaddy/Claude-Workshop/blob/main/claude-lab-projects-skills-connectors-instructions.md). ChatGPT details come from search results, not from a logged-in account, so treat them as unverified until you test them.

- [Skills in ChatGPT, OpenAI Help Center](https://help.openai.com/en/articles/20001066-skills-in-chatgpt)
- [Skills resource, OpenAI Academy](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/skills)
- [Projects in ChatGPT, OpenAI Help Center](https://intercom.help/openai/en/articles/10169521-projects-in-chatgpt)
- [Projects, OpenAI Academy](https://academy.openai.com/public/clubs/work-users-ynjqu/resources/projects)
- [Admin controls in apps, OpenAI Help Center](https://help.openai.com/en/articles/11509118-admin-controls-security-and-compliance-in-connectors-enterprise-edu-and-business)
- [How to use ChatGPT Projects, Elephas](https://elephas.app/resources/how-to-use-chatgpt-projects)
- [ChatGPT Connectors guide, Context Link](https://www.context-link.ai/blog/chatgpt-connectors)
- [Custom instructions setup, Temperstack](https://www.temperstack.com/learn/chatgpt/set-up-custom-instructions/)
