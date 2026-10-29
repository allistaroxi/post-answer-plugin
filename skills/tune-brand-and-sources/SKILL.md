---
name: tune-brand-and-sources
description: Bring a brand's Post Answer setup in line with what the person knows about their business, by updating its brand voice (about the business, audience, tone, phrases, words to avoid) and the sources Radar watches (subreddits, X accounts and searches, news sites). Use when the person wants Post Answer to sound more like them, says the ideas are off-topic, or asks to add, switch off or remove a subreddit, X account, search or site.
---

# Tune the brand and Radar's sources

Post Answer writes and ranks topics from the brand's voice settings and searches only the sources on its list. These steps use the Post Answer connector.

## Brand voice

1. Call `get_workspace_context` to see what Post Answer has now.
2. Compare it with what the person has told you in this chat. Propose only the changes that follow: how they describe the business, who the audience is, the tone, phrases they really use, words to avoid, topics they never cover.
3. Keep the person's own wording. Never invent facts about the business.
4. Read the changes back as "now: … / change to: …" and ask for a yes.
5. After their yes, call `update_brand_voice` with only the fields that change. Its answer includes what each field was before, so a change can be undone.

## Radar sources

1. Call `list_sources`. Sources come in three groups (subreddits, X accounts and searches, news sites), and each group has a limit on how many can be on at once, because every source costs money on each search.
2. Suggest sources where this brand's audience really talks. Prefer a few active ones over many quiet ones.
3. After the person agrees, call `add_sources`. Post Answer checks that each one exists before saving it, and says which ones it could not add and why.
4. To pause a source, use `set_source` to switch it off. It stays on the list. `remove_source` takes it off completely, so confirm with the person first.
5. If a group is full, ask which source to switch off before adding another.

Changes apply from the next Radar search. Saved topics do not change.
