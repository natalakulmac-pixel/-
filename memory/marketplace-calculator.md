---
name: marketplace-calculator
description: Google-таблица калькулятора маркетплейсов 2023–2026 (WB/Ozon/ЯМ/М.Видео/ЗЯ) и как её обновлять
metadata:
  node_type: memory
  type: project
  originSessionId: 69fbf86b-91fa-4c29-bb90-5d36223c2d69
  modified: 2026-10-13T16:31:05.994Z
---

Калькулятор маркетплейсов: Google Sheet id 1utuaH_jbsEd59VyIrwKEr3IK354wW1vWua5wR7vZhEQ (создан 13.10.2026), исходник xlsx и скрипт сборки — montagh/marketplaces/ и scratchpad build_base.py. Данные WB/Ozon/ЯМ взяты из файла пользователя «Изм_комиссии_логистики_и_хранения_2023_2026_…xlsx», методика расчёта повторяет его лист «Свод от цены до СПП».

**Why:** задача из голосового: база ставок по предметам, страны продавца (РФ, Киргизия, Казахстан, Китай), история на 1 января 2023–2026, калькулятор для клиента.

**How to apply:** локаль таблицы ru_RU — в формулах через API разделитель «;». Большие файлы в Google загружать через Claude in Chrome: на drive.google.com подменить HTMLInputElement.prototype.click, перехватить input type=file, затем file_upload; xlsx → «Файл → Сохранить как таблицу Google». Защита листов стоит только как предупреждение (warningOnly).

Версия для Tilda: публичный репозиторий github.com/natalakulmac-pixel/mp-calculator (mpc.js + wb/oz/ym/common.json), подключается через jsDelivr @v1. Tilda не принимает большой код в T123 — данные только внешним файлом. Обновление: новый коммит + НОВЫЙ тег (v3, v4…) и смена тега в коде на сайте — перенос существующего тега jsDelivr не подхватывает даже после purge. С v2 тарифы только из официальных источников (кабинет WB, seller-edu Ozon, справка ЯМ); исходники в scratchpad repo2/ (build_official.py, logic.js, src.html).
