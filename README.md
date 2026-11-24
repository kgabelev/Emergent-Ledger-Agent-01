# Emergent-Ledger-Agent-01
AI Agent Employee
# Emergent Ledger Agent 01: General Social Media Agent

An AI agent employee, built in the open. This is the first agent in the Emergent Ledger agent offerings. Status: prototype, not live.

## What it does
Handles the basic, most frequent social media office tasks for one brand at a time: captions, hashtags, comment reply drafts, weekly content calendars, and inbox summaries. It drafts only. A human reviews and posts.

## How it is built
- **Job description**: a written role with what the agent may do, what it may never do, and who approves. See JOB_DESCRIPTION.md.
- **Context pack**: the brand voice, facts, and banned list the agent must read before every task.
- **Task log**: one row per task with the ask, the context used, the draft, the human verdict, and a 1 to 5 score.
- **Trajectories**: one short record per task showing each step the agent took, its output, and a rubric score.
- **Daily read**: a one-page summary of what worked, what failed, and the trend.

## Permission levels
0 read and draft only (start here). 1 send drafts to the owner by email. 2 post to one account after approval. An agent moves up only after it passes a test set.

## Build order
1. Room and audit trail first.
2. Run tasks by hand to learn what the agent should do.
3. Automate with n8n.
4. Add email access.
5. Test on a fixed set of real tasks before anything goes live.

## Why the audit trail
Every task and step is recorded so a person can read the trajectory, see what is working and what is not, and judge the agent on evidence.

Built by Kirill Gabelev, Emergent Ledger.

