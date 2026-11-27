# SWE Project Practice

Five hands-on software engineering project courses, each built around a real
system you implement yourself. Every course ships with curated video lessons
and reading material (YouTube, docs, articles, open-source repos).

Companion Space: **SWE Project Practice** (in Muse) — the same five courses
as an interactive hub with search, filters, and progress tracking.

## Courses

| # | Course | Stack | What you build |
|---|--------|-------|----------------|
| 1 | [Twitter Backend in Python](courses/twitter-backend-python/README.md) | Python, FastAPI/Django, PostgreSQL, Redis | A Twitter-like backend: timelines, fan-out, follows, likes |
| 2 | [Self-Driving Car Project](courses/self-driving/README.md) | Python, OpenCV, TensorFlow, CARLA, Apollo | Lane detection, object detection, motion planning in simulation |
| 3 | [Flash-Sale System in Spring](courses/flash-sale-spring/README.md) | Java, Spring Boot, Redis, RabbitMQ/Kafka, MySQL | A seckill system that survives 100k QPS without overselling |
| 4 | [NLP Sensitive-Word Detection](courses/nlp-sensitive-word-detection/README.md) | Python, Aho-Corasick, BERT, Hugging Face | Real-time sensitive-word filtering, dictionary + model based |
| 5 | [Blockchain: Principles to Applications](courses/blockchain/README.md) | Python, Solidity, Ethereum | A blockchain from scratch, then smart contracts and dapps |

## Repo layout

```
.
├── index.html                      # Exported Space page (single-file build)
├── README.md                       # This file
└── courses/
    ├── twitter-backend-python/
    ├── self-driving/
    ├── flash-sale-spring/
    ├── nlp-sensitive-word-detection/
    └── blockchain/
```

Each course directory has its own README with an overview, tech stack, and
the full resource list (videos + docs/repos). Implementation code for each
course lives in its directory as you build it.

## How to use

1. Pick a course and read its README.
2. Watch the videos in order, then read the linked docs/articles.
3. Build the project — each course ends with a working deliverable.
4. Check off milestones on the companion Space as you go.
