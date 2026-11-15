# Denwave Roadmap

[Русский](#русский) · [English](#english)

## Русский

Обновлено: 15 ноября 2026 года.

Denwave развивается как голосовой и текстовый чат, который можно развернуть на собственном сервере. Мы хотим сохранить простой запуск для небольших команд и постепенно расширять возможности общения и управления сообществом.

Это направления развития, а не календарь релизов. Ближайший фокус имеет приоритет; порядок остальных задач может меняться по результатам тестирования и обратной связи. Конкретные сроки и номера версий для будущих функций пока не назначены.

### Уже доступно

В [релизе r30](https://github.com/v-alexander-kim/denwave-app/releases/tag/r30): сервер **0.17.0**, клиент **0.20.2**.

- Голосовые каналы, локальное шумоподавление, выбор устройств, громкость участников, push-to-talk и голосовая активация.
- Камеры и демонстрация экрана в голосовых каналах.
- Чат сервера, чаты каналов и личные сообщения: ответы, редактирование, треды, реакции, вложения, упоминания, Markdown и команды.
- Роли с рангами и правами, иконки ролей, аудит, категории и перемещение участников, видимость и пароли каналов, баны и передача владения сервером.
- Клиент Windows 10/11 и macOS; сервер Windows/Linux; локальные аккаунты, trusted devices, сохранённые серверы и HTTPS.
- Обновление клиента из приложения и простой первый запуск сервера: один бинарник, короткий опросник и готовые адреса для клиента.

### Ближайший фокус: надёжная связь и запуск

- Проверка и улучшение голоса между разными сетями, при нестабильном соединении и после переподключения.
- Длительные голосовые сессии, частые входы/выходы и проверка видео/демонстрации экрана на Windows и macOS.
- Понятная диагностика подключения и инструкции для владельца сервера.
- Шлифовка первого запуска и обновлений сервера.

### В планах

Следующие кандидаты на разработку:

- **Языки интерфейса:** локализация клиента, выбор языка в настройках и постепенное добавление переводов.
- **Уведомления:** улучшение поведения уведомлений на macOS и переход к нужному чату.
- **Управление сервером:** названия рангов, IP-баны, хранение и экспорт аудита, больше инструментов модерации.
- **Мобильные клиенты** после стабилизации Windows и macOS.

Эти функции ещё не доступны; их порядок будет уточняться. Они не обязаны выйти вместе в одном обновлении.

### Долгосрочные направления

- **Более крупные серверы:** PostgreSQL/Redis, мониторинг, развёртывание и хранение данных при большей нагрузке.
- **Новые платформы:** рабочий клиент для Linux; мобильные клиенты позднее.
- **Сложные сети:** дополнительные способы подключения там, где текущему голосовому соединению мешают ограничения сети.

Для этих направлений сначала нужны технические проверки. Поддержка платформы или функции будет объявлена только после появления проверенного выпуска.

### Что останется основой проекта

- Сервер и пользовательские данные находятся под контролем владельца сервера.
- Простой вариант запуска останется доступен; более сложный серверный режим не должен стать обязательным для маленьких команд.
- Клиент и сервер могут обновляться независимо; изменения совместимости будут указаны в описании релиза.
- Для работы голосового чата не требуется аккаунт в стороннем облачном сервисе.

### Как следить за развитием

Готовые изменения перечисляются в [Releases](https://github.com/v-alexander-kim/denwave-app/releases). Этот roadmap описывает намерения, а не возможности установленной версии.
Для предложений и ошибок используйте [Issues](https://github.com/v-alexander-kim/denwave-app/issues). При описании проблемы со звуком укажите версии клиента/сервера, выбранные режимы обработки, устройства и условия подключения.

---

## English

Updated: November 15, 2026.

Denwave is growing as a voice and text chat you can host on your own server. We want to keep setup simple for small teams while gradually adding communication and community management features.

These are development directions, not a release calendar. The immediate focus takes priority; other tasks may change order based on testing and feedback. Future features do not have assigned dates or version numbers yet.

### Available now

[Release r30](https://github.com/v-alexander-kim/denwave-app/releases/tag/r30) includes server **0.17.0** and client **0.20.2**.

- Voice channels, local noise suppression, device selection, per-user volume, push-to-talk and voice activation.
- Cameras and screen sharing in voice channels.
- Server chat, channel chats and direct messages with replies, editing, threads, reactions, attachments, mentions, Markdown and commands.
- Roles with ranks and permissions, role icons, audit log, categories and participant moves, channel visibility and passwords, bans and ownership transfer.
- Windows 10/11 and macOS clients; Windows/Linux server; local accounts, trusted devices, saved servers and HTTPS.
- In-app client updates and a simple server first run: one binary, a short questionnaire and ready-to-use client addresses.

### Immediate focus: reliable voice and onboarding

- Test and improve voice across different networks, unstable connections and reconnects.
- Long voice sessions, frequent joins/leaves, and video/screen sharing validation on Windows and macOS.
- Clear connection diagnostics and server-owner guidance.
- Polish the first server run and update flow.

### Planned improvements

Candidates for upcoming work:

- **Interface languages:** client localisation, language selection in settings and gradual translation coverage.
- **Notifications:** better macOS notification behaviour and opening the relevant chat.
- **Server management:** rank names, IP bans, audit retention/export and more moderation tools.
- **Mobile clients** after Windows and macOS stabilise.

These features are not available yet; their order will be refined. They do not need to ship together in one update.

### Longer-term directions

- **Larger servers:** PostgreSQL/Redis, monitoring, deployment and data storage under higher load.
- **More platforms:** a viable Linux client; mobile clients later.
- **Restrictive networks:** additional connection options where network restrictions prevent the current voice connection from working.

These directions need technical validation first. Support for a platform or feature will be announced when a tested release is available.

### Principles we want to preserve

- The server owner stays in control of the server and user data.
- Simple deployment remains available; small teams should not need a complex server setup.
- Client and server can update independently; compatibility changes will be described in release notes.
- Voice chat does not require an account with a third-party cloud service.

### Follow progress

Shipped changes are listed in [Releases](https://github.com/v-alexander-kim/denwave-app/releases). This roadmap describes intentions, not the capabilities of your installed version.
Use [Issues](https://github.com/v-alexander-kim/denwave-app/issues) for suggestions and bugs. For audio problems, include client/server versions, processing modes, audio devices and connection conditions.
