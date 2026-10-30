---
name: jarvis-project
description: "Джарвис — личный Telegram-бот на ПК (Claude + управление ПК, заметки, напоминания, проекты), папка montagh/jarvis"
metadata:
  node_type: memory
  type: project
  originSessionId: ffa84aa7-f11f-40d2-99b2-a978e5986190
  modified: 2026-10-27T10:15:19.294Z
---

Собран 2026-10-27 в C:\Users\tolik\montagh\jarvis (jarvis.py, README.md, setup_autostart.ps1). Формат выбран пользователем: Telegram-бот (не голосовой на ПК), функции — ответы, управление ПК, заметки/напоминания, работа с проектами. Python + requests long polling, Claude Opus 5.5 с ручным циклом инструментов, голосовые через faster-whisper base.

27.10 добавлены: make_presentation (.pptx через python-pptx, стили light/dark, template берёт оформление чужого .pptx, google=true заливает в Google Slides), add_routine (плановые задачи, которые бот выполняет сам — общее хранилище с напоминаниями, kind=task), google_tools.py (Sheets/Slides/Drive через OAuth: credentials.json + data/google-token.json, вход `python jarvis.py --google`).

**Why:** на 2026-10-27 на балансе Anthropic API не было денег (400 credit balance too low) — живой ответ Claude не проверен; токен бота и chat_id в .env ещё не вписаны.
**How to apply:** при доработке начинать с README.md; проверка без Telegram — `python jarvis.py --ask "..."`. Правила по проектам в системном промпте дублируют [[vasiliy-anti-gpt]], [[no-hashtag]], [[tasha-instagram-project]] — менять вместе.
