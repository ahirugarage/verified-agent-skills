# Verified Agent Skills — field notes, not a star list

A small, honest index of AI-agent skills that we **actually installed, tested, or indexed** in our own production workflows (game development, 3D research, AI-OS building), with notes on what each one is really for.

Most "awesome" lists copy links. This one only contains entries that passed through our hands, each labeled with how far it got:

- ✅ **Installed & in use** — deployed into our working environments
- 🔬 **Tested locally** — ran its test suite / CLI ourselves and recorded the result
- 👀 **Reviewed & indexed** — read, catalogued, and kept as a candidate (not yet in production)

Last updated: 2026-11-09 · Vol. 1 (10 entries)

---

## The list

### 1. anti-ai-frontend-ui — ✅ Installed & in use
- Source: https://github.com/Emmanuellsensai/anti-ai-frontend-ui (MIT)
- What: Agent skill that bans the "AI-generated look" in frontend UI — 28 named anti-patterns (gradient blobs, glowing badges, tilted floating cards, pill bars, identical card grids, slogan copy).
- Field note: The strict parts are the useful parts: obey the brand, measure real reference sites in a real browser, ship real content, plain copy, then QA. We registered it as a standard skill across all our AI environments, not just one tool.
- Best for: Any UI that must not look machine-made. Not for: teams that actually want the glossy AI aesthetic.

### 2. unslop — ✅ Installed & in use
- Source: https://github.com/heydamir/unslop
- What: Design skill for removing the generic AI flavor from generated designs.
- Field note: We run it as the companion to anti-ai-frontend-ui — one sets the rules before building, the other cleans up taste after. Deployed to all our dev environments on 2026-11-02.

### 3. tacit — 🔬 Tested locally
- Source: https://github.com/abuhuraira99/tacit (MIT)
- What: Captures tacit knowledge for LLM agents.
- Field note: Test suite passed locally (44 tests). Deployed and running on two of our machines as part of a plan to standardize it across all LLM environments. Young project, but the idea — making the unspoken rules explicit for agents — is the real thing.

### 4. TokenEconomizer — 🔬 Tested locally
- Source: https://github.com/microsoft/TokenEconomizer (Apache-2.0)
- What: Cost-reduction plugin for coding agents: per-repo micro-skills learned across sessions, tool-definition pruning, and intervention when an agent loops on the same failure.
- Field note: 849 tests passed in our run and the CLI worked as documented; our verdict was "usable". Honest caveat we measured: its supported host version ranges are narrow, so we paused the broad rollout and kept watch for wider support instead of forcing it everywhere.

### 5. pixelfx — ✅ Installed & in use
- Source: https://github.com/patch-gg/pixelfx
- What: Pixel-art effects collection as an agent skill.
- Field note: Registered across our environments and fed into our game-art pipeline learning. Handy when a game needs retro effects without hand-rolling each one.

### 6. codixel — 👀 Reviewed & indexed
- Source: https://github.com/mankidev/codixel
- What: Pixel/dot-art generation skill.
- Field note: Kept as a candidate for game asset generation. Not yet in production — we list it because the concept fits our pipeline, and we would rather label it honestly than oversell it.

### 7. claude-animation-skills — ✅ Installed & in use
- Source: https://github.com/artemnovitckii/claude-animation-skills
- What: A set of six animation skills for agents.
- Field note: Registered across all our dev environments (2026-11-04). The author also sent demo videos of two of them (graph and minimalistic-graphics), which matched what the skills promise.

### 8. awesome-gamedev-agent-skills — 👀 Reviewed & indexed
- Source: https://github.com/gamedev-skills/awesome-gamedev-agent-skills
- What: An index of 77 game-development agent skills.
- Field note: We indexed it into our game-making database as a map, not as 77 endorsements. Indexes like this are useful exactly when each entry still gets its own check before use.

### 9. awesome-llm-apps — 👀 Reviewed & indexed
- Source: https://github.com/Shubhamsaboo/awesome-llm-apps
- What: A large collection of LLM app examples.
- Field note: We expanded its index (210 entries) into our local archive as a reference shelf. Good raw material for "someone must have built this already" searches — which is always our first step before building anything ourselves.

### 10. roblox-i18n — 👀 Reviewed & indexed
- Source: https://github.com/WhoIsTyfur/roblox-i18n (MIT)
- What: Agent skill that translates a Roblox game into up to 50 locales, with context-aware text checked by independent reviewer agents.
- Field note: Brand new (created 2026-11-09, zero stars when we found it) and not yet tested by us. Registered as a candidate step in our Roblox localization pipeline. Listed with its age shown, because new-and-unproven is fine as long as it is labeled.

---

## How entries get in

1. We find it (usually via our own research feeds), read the actual code/docs — not the announcement post.
2. If it claims to run, we run it. Test results above are our own numbers.
3. It gets a status label, and the label can move down as well as up.

## Notes

- This is a personal field journal, not an official ranking. No entry paid to be here; no code is redistributed — links point to the original repositories, and each skill's own license applies.
- Corrections welcome via issues.

---

## 日本語メモ

実際に自分の開発環境へ入れて使った／テストを回した／索引として保管した AI エージェントスキルだけを集めた、実測メモ付きの選定集です。「すごそう」ではなく「どこまで確認したか」を3段階（✅導入済み・🔬テスト済み・👀検討中）で正直に表示しています。Vol.1 は10件、2026-11-09 時点の記録です。
