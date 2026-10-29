# Post Answer

Post Answer finds what your audience is talking about, helps you turn it into short videos and posts, posts them, answers comments with Auto DMs, and shows how each post did. This plugin brings Post Answer into Claude and ChatGPT: the Post Answer connector, plus skills that tell the assistant how to use it well.

You need a Post Answer account. Start one at [postanswer.com](https://postanswer.com). The full setup guide is at [postanswer.com/ai](https://postanswer.com/ai).

## Install

- **Claude (claude.ai and the desktop app):** Customize, Plugins, Add, Add marketplace, then paste `https://github.com/allistaroxi/post-answer-plugin` and add Post Answer.
- **Claude Code:**

  ```
  /plugin install post-answer --marketplace allistaroxi/post-answer-plugin
  ```

- **ChatGPT:** add `https://postanswer.com/mcp` under Plugins, Add, Add custom MCP server.

## What you can ask

- "What is my audience talking about this week? Breaking stories first."
- "Research the second topic and write me a hook and a 30-second script in my voice."
- "Save that as an Instagram draft for Thursday at 6 pm." Then: "Schedule it."
- "Which of my reels did best this month, and why?"
- "Set up an Auto DM: anyone who comments GUIDE gets the link to my guide."
- "Add r/dentistry to my Radar sources and make my brand voice less formal."

## Skills

| Skill | What it does |
| --- | --- |
| `find-content-ideas` | Reads Radar's saved topics (breaking first when you want what is new), digs into one, and starts new research or a Radar search only when you ask |
| `write-and-post` | Writes captions, hooks and scripts in your brand's voice, saves drafts, and posts or schedules only after you approve a preview in the chat |
| `explain-results` | Explains your Stats: followers, views, which videos beat your usual and why, the best time to post |
| `auto-dm-and-leads` | Sets up, changes and stops Auto DMs, and reads the leads they bring in |
| `tune-brand-and-sources` | Updates your brand voice and the subreddits, X accounts and news sites Radar watches |

## Connect

The plugin connects to `https://postanswer.com/mcp`. The first time you use it, you sign in to Post Answer and choose:

- which workspaces (brands or clients) the assistant may see, and
- what it may do: save drafts, start Radar searches and research, post and schedule, manage Auto DMs and leads, change the brand voice and sources. Each one is off unless you tick it.

You can see and disconnect every connection in Post Answer under Settings, Connected AI tools. Disconnecting stops access at once. It does not cancel posts that are already scheduled.

## Safety

- Posting always shows you a full preview first: each network and account, the caption, the files, the time and any Auto DM. Nothing goes out until you say yes in the chat, and the approval is checked by Post Answer's server, not by the assistant.
- A new Radar search uses one of your plan's runs. The assistant tells you and waits for your yes.
- Text from topics, comments and DMs is treated as material to read, never as instructions.

## Data

The assistant sends your requests to Post Answer at postanswer.com and gets back the data it asks for: your saved topics and research, posts, Stats, Auto DMs and leads, and your brand voice, only for the workspaces and permissions you allowed. Post Answer keeps a short record of each call (which tool, when, whether it worked) for 90 days to enforce limits and to help with support. It does not store your chat. The plugin itself stores nothing and contains no keys.

[Setup guide](https://postanswer.com/ai) · [Privacy policy](https://postanswer.com/privacy) · [Terms](https://postanswer.com/terms) · Support: [info@allistarmedia.io](mailto:info@allistarmedia.io)

Post Answer is a product of Allistar Media.
