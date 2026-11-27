# Course 1 — Twitter Backend in Python

Build a Twitter-like backend from scratch: posting, following, likes, and a
home timeline that stays fast at scale. The core design problem is fan-out —
push on write vs pull on read — and the celebrity problem that breaks naive
fan-out.

## Tech stack

Python · FastAPI or Django · PostgreSQL · Redis

## What you build

A working Twitter clone backend with a home timeline, fan-out on write with a
hybrid path for high-follower accounts, cursor pagination, and Redis-backed
timeline caching.

## Videos

1. **Design Twitter: Home Timeline, Fan-out & the Celebrity Problem | System Design Interview** (~15 min, en)
   https://www.youtube.com/watch?v=7VF3tmwPLUM
   Building a small Twitter in Python + PostgreSQL + Redis with fan-out on write, the celebrity problem, and hybrid merge.
2. **Design the News Feed (Twitter / X) — System Design Interview** (~25 min, en, The Hot Path)
   https://www.youtube.com/watch?v=M1Xv-sxBG1E
   Deriving fan-out on write vs on read from read/write ratios, celebrity hot keys, hybrid model, cursor pagination, outbox pattern.
3. **Let's Build Twitter With Django and Python - Django Wednesdays Twitter #1** (~14 min, en, Codemy.com)
   https://www.youtube.com/watch?v=KXunlJgeRcU
   Hands-on Django series opener building a Twitter clone (Musker) from scratch; later episodes cover follow/unfollow and posting.
4. **Python FastAPI Tutorial: Full Course for Beginners - Build a Full-Stack Web App** (~14 h 24 min, en, Corey Schafer)
   https://www.youtube.com/watch?v=iukOehU5aF4
   Full FastAPI stack — SQLAlchemy/Pydantic, CRUD, async, JWT auth, pagination, PostgreSQL/Alembic, testing and deployment; the FastAPI foundation for this course.
5. **Design the Twitter Timeline: Fan-out, the Celebrity Problem, and Search — Real-Run** (~8 min, en, Real-Run)
   https://www.youtube.com/watch?v=xUd3sSbkqWY
   Pull vs push fan-out trade-offs, celebrity write storms, fan-count-based hybrid routing, with a Python stdlib live demo.

## Docs, articles & repos

- **Redis patterns — building a Twitter clone (Retwis)**, official Redis tutorial (en)
  https://redis.io/docs/latest/develop/clients/patterns/twitter-clone/
  Designing a Twitter clone's data model, follow graph, and timelines with Redis structures (List/Set/Hash/Sorted Set).
- **Design Twitter: Feed Fanout and Timeline Guide**, System Decoder (en)
  https://www.systemdecoder.com/guide/hld/twitter-system-design
  Interactive system-design guide comparing fan-out on read / on write / hybrid, with Redis timeline caching (LPUSH/LTRIM, capped at 800 items).
- **实战案例：社交网络 Twitter**, karanpratapsingh/system-design case study, Chinese walkthrough (zh)
  http://opendeep.wiki/karanpratapsingh/system-design/interviews-case-studies.twitter
  Requirements, capacity estimation, APIs, data model, push/pull/hybrid fan-out, message queues and cache layers.
