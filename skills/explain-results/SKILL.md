---
name: explain-results
description: Explain how a brand's social posts and videos are doing with Post Answer Stats. Use when the person asks how their posts, reels or videos performed, which video did best or worst, why one did well, their followers or views, or the best time and day to post.
---

# Explain results

These steps use the Post Answer connector's Stats tools. They read the person's connected social accounts.

## Steps

1. Call `list_workspaces` and agree which brand.
2. **Overview:** call `get_stats_summary` without a network for each account's followers and totals.
3. **One network:** call `get_stats_summary` with a `network` and `days` (7, 30 or 90; 30 if they did not say). It returns the typical views, the videos that beat or trailed the account's usual, the best time and day to post, and what stood out.
4. **One video:** call `get_video_stats` with the `network` and a `video_id` from the summary. It returns how many viewers were still watching through the video, where the views came from and who watched.

## How to explain

- Lead with the answer to the question, then the two or three numbers behind it.
- "Times usual" compares a video with the account's own typical views: 3 times usual means three times what this account normally gets. Say it that way, not as a share of some other account.
- To explain why a video did well, use what the numbers show: how many people kept watching, shares and saves, where the views came from, and the time it went out. Say clearly when a reason is your reading of the numbers and not something the data says.
- Report numbers exactly as given. If one is missing, or marked early or partial, say so. Never estimate it.
- Suggest one or two next moves that follow from the numbers, for example posting at the best hour, or making another video on the topic that did best.

## When something is missing

- No connected accounts, or a network with no data: say so. Accounts are connected in Post Answer, on the Post screen.
- A limit message: Stats can be asked about 10 times a minute. Wait a minute and try again.
