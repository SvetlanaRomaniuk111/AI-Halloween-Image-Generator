# AI-Halloween-Image-Generator 🌿❄️

### Опис
**AI Image & Video Transformer Bot** — це Telegram-бот на базі Python, який використовує найсучасніші 
моделі штучного інтелекту (**Gemini 2.5 Flash** та **Veo 3.0**) для магічного перетворення фотографій. 
Бот дозволяє користувачам завантажувати свої портрети та застосовувати до них художні стилі 
(наприклад, "Лісова Мавка" або "Король Півночі"), зберігаючи реалістичність обличчя, а також генерувати 
короткі відео на основі цих трансформацій.

### Вимоги
* **Python 3.12+**
* Активний **Telegram Bot Token** (від @BotFather)
* **Google API Key** (з доступом до моделей Gemini та Veo)

### Встановлення

1. **Клонуйте репозиторій:**
   ```bash
   git clone https://github.com/SvetlanaRomaniuk111/AI-Halloween-Image-Generator.git
   cd AI-Halloween-Image-Generator
   ```

2. **Налаштуйте віртуальне середовище:**
   ```bash
   python -m venv .venv
   # Для Windows:
   .venv\Scripts\activate
   # Для macOS/Linux:
   source .venv/bin/activate
   ```

3. **Встановіть необхідні бібліотеки:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Налаштуйте змінні середовища:**
   Створіть файл `.env` у кореневій директорії на основі прикладу:
   ```bash
   cp .env.example .env
   ```
   Відкрийте файл `.env` та вставте ваші ключі:
   * `TELEGRAM_TOKEN` — токен вашого бота.
   * `GOOGLE_API_KEY` — ваш ключ із Google AI Studio.

## Структура проєкту
Основними файлами логіки бота є:
* `src/.../myproject/bot.py` — обробка команд Telegram та логіка інтерфейсу.
* `src/.../myproject/ai.py` — інтеграція з моделями Google Gemini та Veo.

### Запуск
```bash
python src/ua/javarush/python/marathon/halloweenbot/myproject/bot.py
```

### Функціонал
* **Image-to-Image Transformation:** Реалістичне редагування фото за допомогою `gemini-2.5-flash-image`.
* **Motion Beats:** Генерація відео на основі текстових сценаріїв руху за допомогою `veo-3.0-fast-generate-001`.
* **Custom Styles:** Попередньо налаштовані магічні промпти для чоловічих та жіночих образів.

