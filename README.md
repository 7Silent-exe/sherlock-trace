# sherlock-trace
# OSINT Trace: Sherlock + HaveIBeenPwned

Цепочка анализа по никнейму и email.  
Инструменты: Sherlock (GitHub) + HaveIBeenPwned (open-source web API).

---

## 🧠 Цель

Найти цифровые следы через открытые данные:

- Никнейм → активные аккаунты
- Email → утечки в базах данных

---
⚠️ Важно

Sherlock обновлён.  
Команда `python sherlock username` больше не работает.  
Нейросети, туторы и видео на YouTube часто выдают устаревший запуск.

✅ В этом репозитории — **реальная схема** и рабочая структура.

---

🔧 Установка Sherlock

git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
pip install .
(если не работает — python -m pip install .)

▶️ Запуск Sherlock
python sherlock_project/__main__.py SIMPSON 

📂 Сохранить результат:
python sherlock_project/__main__.py SIMPSON --output results.txt
🔍 Проверка через HaveIBeenPwned
Перейти: https://haveibeenpwned.com/

Ввести email, найденный в одном из профилей

Получить список утечек: сервис, год, данные

📁 Файлы
results.txt — терминальный вывод Sherlock

screenshot_hibp.png — вырезка с подтверждением утечки

🧩 Пример цепочки
Ник: SIMPSON
→ Найдено в GitHub, SoundCloud, Reddit  
→ Email в профиле  
→ HIBP: LinkedIn (2016), Tumblr (2013)
Автор
7Silent-exe
OSINT, код, дисциплина.
Тишина — это тоже инструмент.
