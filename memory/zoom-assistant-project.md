---
name: zoom-assistant-project
description: "ИИ-ассистент после Zoom-созвонов (локальная запись → Whisper → Claude → Telegram), папка zoom-assistant"
metadata:
  node_type: memory
  type: project
  originSessionId: 03840dec-b302-42e7-9495-ba45391d648a
  modified: 2026-10-20T09:48:19.055Z
---

Собран 2026-10-20 в C:\Users\tolik\montagh\zoom-assistant. Источник — локальные записи Zoom (папка Документы\Zoom, опрос каждые 15 мин через Планировщик Windows), расшифровка faster-whisper на CPU, выход — Telegram-бот: резюме, задачи, письмо-фоллоуап, идеи для контента.

**Why:** пользователь сначала выбрал облачную запись, потом переключился на запись с компьютера. Ноутбук слабый (i3-7020U, 4 ГБ ОЗУ), поэтому Whisper small, beam_size=1.
**How to apply:** ключи в .env ещё не заполнены на момент создания; при доработке начинать с README.md в папке.
