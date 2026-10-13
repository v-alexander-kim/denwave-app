# Denwave Roadmap

[Русский](#русский) · [English](#english)

## Русский

Обновлено: 13 октября 2026 года.

Denwave развивается как голосовой и текстовый чат, который можно развернуть на собственном сервере. Мы хотим сохранить простой запуск для небольших команд и постепенно расширять возможности общения и управления сообществом.

Это направления развития, а не календарь релизов. Ближайший фокус имеет приоритет; порядок остальных задач может меняться по результатам тестирования и обратной связи. Конкретные сроки и номера версий для будущих функций пока не назначены.

### Уже доступно

В [релизе r2](https://github.com/v-alexander-kim/denwave-app/releases/tag/r2): сервер **0.1.0**, клиент **0.2.0**.

- Голосовые каналы, локальное шумоподавление RNNoise, выбор устройств, громкость участников, push-to-talk и голосовая активация с порогом в dBFS.
- Общий чат, чаты голосовых каналов и личные сообщения; ответы, редактирование, упоминания и Markdown.
- Роли с рангами и правами, видимость и пароли каналов, баны и передача владения сервером.
- Клиент Windows 10/11; сервер Windows/Linux; локальные аккаунты, сохранённые серверы и HTTPS.

### Ближайший фокус: надёжная связь

- Проверка и улучшение голоса между разными сетями, при нестабильном соединении и после переподключения.
- Длительные голосовые сессии и частые входы/выходы участников без ухудшения работы канала.
- Настройка обработки звука: качество речи, шумоподавление, эхоподавление и удобная голосовая активация.
- Более понятные сообщения о проблемах подключения и инструкции для владельца сервера.

### В планах: удобство повседневного общения

Следующие кандидаты на разработку:

- **Каналы:** перемещение участников между каналами, категории и организация списка, отдельные текстовые каналы.
- **Чат:** реакции, вложения, ветки обсуждений и удобный учёт непрочитанных сообщений.
- **Уведомления:** свой звук уведомлений и переход к нужному чату по нажатию уведомления.
- **Языки интерфейса:** локализация клиента, выбор языка в настройках и постепенное добавление новых переводов, включая сообщения об ошибках и подсказки.
- **Управление сервером:** загружаемые иконки ролей, просмотр журнала действий и дополнительные инструменты модерации.
- **Обновления:** проверка новых версий и автоматическое обновление клиента с проверкой подлинности пакетов.

Эти функции ещё не доступны; их порядок будет уточняться. Они не обязаны выйти вместе в одном обновлении.

### Долгосрочные направления

- **Демонстрация экрана и камеры** в голосовых каналах.
- **Новые платформы:** проверка и выпуск клиента для macOS; поиск рабочего решения для Linux; мобильные клиенты позднее.
- **Более крупные серверы:** улучшение производительности, мониторинга, развёртывания и хранения данных при большей нагрузке.
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

Updated: October 13, 2026.

Denwave is growing as a voice and text chat you can host on your own server. We want to keep setup simple for small teams while gradually adding communication and community management features.

These are development directions, not a release calendar. The immediate focus takes priority; other tasks may change order based on testing and feedback. Future features do not have assigned dates or version numbers yet.

### Available now

[Release r2](https://github.com/v-alexander-kim/denwave-app/releases/tag/r2) includes server **0.1.0** and client **0.2.0**.

- Voice channels, local RNNoise suppression, device selection, per-user volume, push-to-talk and voice activation with a dBFS threshold.
- Server chat, voice-channel chats and direct messages; replies, editing, mentions and Markdown.
- Roles with ranks and permissions, channel visibility and passwords, bans and ownership transfer.
- Windows 10/11 client; Windows/Linux server; local accounts, saved servers and HTTPS.

### Immediate focus: reliable voice

- Test and improve voice across different networks, unstable connections and reconnects.
- Long voice sessions and frequent participant joins/leaves without degrading the channel.
- Refine speech quality, noise suppression, echo cancellation and voice activation controls.
- Clearer connection diagnostics and setup guidance for server owners.

### Planned improvements: everyday communication

Candidates for upcoming work:

- **Channels:** move participants between channels, categories and list organisation, dedicated text channels.
- **Chat:** reactions, attachments, discussion threads and better unread message tracking.
- **Notifications:** a dedicated notification sound and opening the relevant chat from a notification.
- **Interface languages:** client localisation, language selection in settings and gradually adding translations, including error messages and help text.
- **Server management:** uploaded role icons, an activity log viewer and more moderation tools.
- **Updates:** checking for new versions and automatic client updates with package authenticity checks.

These features are not available yet; their order will be refined. They do not need to ship together in one update.

### Longer-term directions

- **Screen sharing and cameras** in voice channels.
- **More platforms:** validate and release a macOS client; investigate a viable Linux solution; mobile clients later.
- **Larger servers:** better performance, monitoring, deployment and data storage under higher load.
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
