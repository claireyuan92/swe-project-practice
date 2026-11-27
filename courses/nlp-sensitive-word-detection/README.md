# Course 4 — NLP Sensitive-Word Detection

Build a real-time sensitive-word detection pipeline. Start with the classic
algorithm — the Aho-Corasick automaton for single-pass multi-pattern matching —
then add a model-based layer by fine-tuning BERT for toxic-comment
classification.

## Tech stack

Python · Aho-Corasick / DFA trie · BERT · Hugging Face Transformers · PyTorch

## What you build

A content-moderation filter that handles Chinese text correctly (traditional/
simplified conversion, full/half-width, pinyin, fuzzy matching) at real-time
speed, plus a BERT classifier for cases a word list cannot catch.

## Videos

1. **Advanced Data Structures: Aho-Corasick Automaton** (~10 min, en, Niema Moshiri)
   https://www.youtube.com/watch?v=O7_w001f58c
   Concise visual walkthrough of building the Aho-Corasick automaton — trie construction, failure links, single-pass multi-pattern search; the core algorithm behind fast sensitive-word filtering.
2. **Lecture on Aho Corasick Algorithm and Applications — Sergey Kulik, Indian Programming Camp 2016** (en, CodeChef)
   https://www.youtube.com/watch?v=xkGkWmthlF0
   In-depth lecture on Aho-Corasick and real-world applications (multi-pattern matching at scale); good follow-up once basics are clear.
3. **C4. Алгоритм Ахо-Корасик — Кирилл Кришталь** (~1 h 45 min, ru)
   https://www.youtube.com/watch?v=-IepoOSQGC8
   Rigorous lecture on Aho-Corasick (trie + suffix/failure links, counting occurrences); notably uses filtering profanity in chat messages as its motivating example. In Russian — skip if language is a blocker.

## Docs, articles & repos

- **〖敏感词检测〗01 – 任务介绍** (小傻瓜别回头, zh)
  https://tlylft.github.io/NLP/sensitive_word/sensitivewords/
  Chinese hands-on tutorial covering the full sensitive-word detection landscape — DFA/trie filtering, Aho-Corasick, Chinese word-list sources, AI-based approaches — with Python code.
- **ToolGood.Words — 高性能敏感词检测过滤组件** (GitHub, zh docs, C#/Python)
  https://github.com/toolgood/ToolGood.Words
  Production-grade open-source sensitive-word detection/filtering library built on Aho-Corasick, with traditional/simplified Chinese conversion, full/half-width handling, pinyin conversion and fuzzy search — the standard reference implementation for real-time Chinese content moderation.
- **Toxic Comment Classification using BERT** (GeeksforGeeks, en)
  https://www.geeksforgeeks.org/machine-learning/toxic-comment-classification-using-bert/
  Step-by-step tutorial fine-tuning BERT (PyTorch + Hugging Face Transformers) for multi-label toxic-comment classification — the model-based complement to dictionary/AC filtering, directly applicable to real-time moderation pipelines.
