# SillyStream

**A free, local-first streaming companion for TikTok LIVE and Twitch.**
One app that merges chat and events from both platforms and drives text-to-speech, alerts,
overlays, goals, timers, points and chat commands. Every feature is free: no subscriptions,
no paid tiers, no telemetry.

> This repository only hosts **releases** of SillyStream.
> Download the latest version from the [Releases page](https://github.com/DanyilVoloschuk/silly-stream-releases/releases).

---

## ✨ Features

- **TikTok LIVE and Twitch at the same time.** Chat, gifts, follows, subs, bits, raids and likes from both platforms in one feed.
- **Text-to-speech.** Free Microsoft Edge voices out of the box, with optional ElevenLabs voices if you have your own API key. Each viewer can get their own voice.
- **Actions and events.** Rules like "when someone sends this gift → play a sound / show an alert / read a message / press a key / switch an OBS scene".
- **OBS overlays.** Alerts, chat, goals, timer, leaderboards and more, all as browser-source links. Pick a built-in theme or make your own with HTML/CSS templates (`.sillytheme` import/export).
- **Goals, stream timer and points.** Like/coin/follower goals, a subathon-style timer, viewer points.
- **Leaderboards.** Top coins and top likes per stream, day, week, month or year.
- **Chat commands.** Custom commands with replies (on platforms that allow sending chat).
- **Pop-out chat window.** An always-on-top chat window with adjustable opacity and click-through mode.
- **English and Ukrainian** interface.

## 💾 Download

Each release has two files:

| File | What it is |
|---|---|
| `SillyStream-Setup-<version>.exe` | **Installer (recommended).** Installs for your user, adds Start menu and desktop shortcuts, and sets up the overlay address. |
| `SillyStream-<version>-portable.zip` | **Portable.** Unzip anywhere and run `SillyStream.exe`. Nothing is installed. |

Both versions use the same settings and data, so you can switch between them.

## 🖥️ Requirements

- Windows 10 or 11 (64-bit)
- Microsoft Edge WebView2 Runtime (already included in Windows 11 and most Windows 10 installs; the installer offers to add it if it's missing)
- OBS Studio, if you want overlays on stream

## 🚀 Getting started

1. Download and run the installer (or unzip the portable build).
2. **Windows SmartScreen warning:** SillyStream isn't code-signed yet, so Windows may show
   *"Windows protected your PC"*. Click **More info → Run anyway**.
3. Open SillyStream and go to **Accounts**:
   - **Twitch:** click *Log in* and enter the code shown on twitch.tv/activate.
   - **TikTok:** enter your TikTok username. You must be LIVE for events to come in.
4. Set up TTS, alerts and actions from the dashboard.
5. In OBS, add a **Browser Source** and paste the overlay link from the **Overlays** page.

## 📁 Where your data lives

All settings, rules and stats are stored locally on your PC:
`%LOCALAPPDATA%\SillyStream`

Login tokens and API keys are kept in **Windows Credential Manager**, never in plain files.
SillyStream doesn't send your data anywhere except to the platforms and services you connect.

## 🔄 Updating

Download the newest installer and run it over the old version. Your settings are kept.
For the portable build, replace the old folder with the new one.

## ⚠️ Notes

- TikTok LIVE support uses an unofficial connection and is **read-only**: SillyStream can read
  TikTok chat and gifts but can't send chat messages to TikTok.
- If TikTok changes things on their side, the TikTok connection may stop working until an update is released.

## 🐞 Bugs and ideas

Open an [issue](https://github.com/YOUR-USER/sillystream-releases/issues) with:
- your SillyStream version (shown in Settings),
- what you did and what happened,
- the log file, if you have one (`%LOCALAPPDATA%\SillyStream\logs`).

---

SillyStream is not affiliated with TikTok, ByteDance, Twitch or Amazon.

| **Українська**

**Безкоштовний локальний помічник для стрімів на TikTok LIVE і Twitch.**
Одна програма збирає чат і події з обох платформ в одну стрічку та керує озвученням тексту,
алертами, оверлеями, цілями, таймерами, балами й командами чату. Усі функції безкоштовні:
без підписок, платних тарифів і телеметрії.

> У цьому репозиторії є лише **релізи** SillyStream.
> Завантажте останню версію на [сторінці релізів](https://github.com/DanyilVoloschuk/silly-stream-releases/releases).

---

## ✨ Можливості

- **TikTok LIVE і Twitch одночасно.** Чат, подарунки, підписки, фоловери, біти, рейди й лайки з обох платформ в одній стрічці.
- **Озвучення тексту (TTS).** Одразу доступні безкоштовні голоси Microsoft Edge, а з власним API-ключем можна підключити голоси ElevenLabs. Кожному глядачеві можна призначити окремий голос.
- **Дії та події.** Правила на кшталт «коли хтось надсилає цей подарунок → програти звук / показати алерт / прочитати повідомлення / натиснути клавішу / перемкнути сцену в OBS».
- **Оверлеї для OBS.** Алерти, чат, цілі, таймер, таблиці лідерів тощо — усе як посилання для джерела «Браузер». Оберіть вбудовану тему або створіть власну за допомогою шаблонів HTML/CSS (імпорт і експорт `.sillytheme`).
- **Цілі, таймер стріму й бали.** Цілі за лайками, монетами чи фоловерами, таймер у стилі сабатону, бали для глядачів.
- **Таблиці лідерів.** Топ за монетами й лайками за стрім, день, тиждень, місяць або рік.
- **Команди чату.** Власні команди з відповідями (на платформах, де можна надсилати повідомлення в чат).
- **Окреме вікно чату.** Вікно чату поверх інших вікон з регульованою прозорістю та режимом, у якому клацання проходять крізь вікно.
- Інтерфейс **англійською та українською**.

## 💾 Завантаження

У кожному релізі є два файли:

| Файл | Що це |
|---|---|
| `SillyStream-Setup-<version>.exe` | **Інсталятор (рекомендовано).** Встановлює програму для вашого користувача, додає ярлики в меню «Пуск» і на робочий стіл та налаштовує адресу оверлеїв. |
| `SillyStream-<version>-portable.zip` | **Портативна версія.** Розпакуйте будь-куди й запустіть `SillyStream.exe`. Нічого не встановлюється. |

Обидві версії використовують ті самі налаштування й дані, тож між ними можна перемикатися.

## 🖥️ Вимоги

- Windows 10 або 11 (64-біт)
- Microsoft Edge WebView2 Runtime (уже є у Windows 11 і в більшості встановлень Windows 10; якщо його немає, інсталятор запропонує його додати)
- OBS Studio, якщо хочете показувати оверлеї на стрімі

## 🚀 Початок роботи

1. Завантажте й запустіть інсталятор (або розпакуйте портативну версію).
2. **Попередження Windows SmartScreen:** SillyStream поки що не має цифрового підпису, тому Windows
   може показати *«Windows захистила ваш ПК»*. Натисніть **Докладніше → Усе одно запустити**.
3. Відкрийте SillyStream і перейдіть до **Акаунтів**:
   - **Twitch:** натисніть *Увійти* та введіть код, показаний на twitch.tv/activate.
   - **TikTok:** введіть своє ім'я користувача TikTok. Події надходять лише тоді, коли ви в ефірі.
4. Налаштуйте озвучення, алерти й дії на панелі керування.
5. В OBS додайте джерело **«Браузер»** і вставте посилання на оверлей зі сторінки **«Оверлеї»**.

## 📁 Де зберігаються ваші дані

Усі налаштування, правила й статистика зберігаються локально на вашому ПК:
`%LOCALAPPDATA%\SillyStream`

Токени входу та API-ключі зберігаються в **Диспетчері облікових даних Windows**, а не у звичайних файлах.
SillyStream нікуди не надсилає ваші дані, окрім платформ і сервісів, які ви самі підключили.

## 🔄 Оновлення

Завантажте найновіший інсталятор і запустіть його поверх старої версії. Налаштування збережуться.
Для портативної версії замініть стару папку новою.

## ⚠️ Примітки

- Підтримка TikTok LIVE працює через неофіційне підключення лише **для читання**: SillyStream
  бачить чат і подарунки в TikTok, але не може надсилати повідомлення в чат TikTok.
- Якщо TikTok щось змінить на своєму боці, підключення до TikTok може перестати працювати до виходу оновлення.

## 🐞 Помилки та ідеї

Створіть [issue](https://github.com/YOUR-USER/sillystream-releases/issues) і вкажіть:
- версію SillyStream (її видно в Налаштуваннях),
- що ви зробили і що сталося,
- файл журналу, якщо він є (`%LOCALAPPDATA%\SillyStream\logs`).

---

SillyStream не пов'язаний з TikTok, ByteDance, Twitch чи Amazon.
