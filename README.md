<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/denwave-lockup-dark.svg">
    <img src="assets/denwave-lockup-light.svg" alt="Denwave" height="64">
  </picture>
</h1>

<p align="center"><a href="#русский">Русский</a> · <a href="#english">English</a></p>

---

## Русский

**Denwave** — голосовой и текстовый чат для команд, сообществ и компаний, который работает на вашем собственном сервере. Вы запускаете сервер на своём компьютере или VDS, участники подключаются к нему через приложение Denwave. Сервер, аккаунты, переписка и настройки остаются у вас — никаких сторонних облачных сервисов.

### Возможности
- Голосовые каналы с низкой задержкой (WebRTC): подавление шума, эхоподавление, громкость каждого участника.
- Режимы микрофона: постоянно, по голосу, push-to-talk; глобальные горячие клавиши.
- Чат сервера, чаты каналов и личные сообщения: упоминания, Markdown, уведомления, команды (`/help`).
- Роли и права, каналы с паролем и видимостью по ролям, баны.
- Вход с паролем, «запомнить меня» (ключ хранится в системном хранилище), список серверов.
- HTTPS с автоматическим сертификатом Let's Encrypt или своими файлами.

### Скачать
Последняя версия — на странице [Releases](../../releases/latest):
- `Denwave-Client-<версия>-setup.exe` — клиент для Windows 10/11;
- `denwave-server-<версия>-windows-amd64.exe` и `denwave-server-<версия>-linux-amd64` — сервер;
- `config.simple.yaml` — пример настроек сервера.

### Клиент
1. Запустите установщик. Windows может предупредить о неизвестном издателе: «Подробнее» → «Выполнить в любом случае».
2. Добавьте адрес сервера, который вам дал его владелец, и войдите или создайте аккаунт.

Новая версия ставится поверх старой, сохранённые серверы и настройки остаются. Устанавливайте именно установщиком: просто скопированный exe не показывает уведомления Windows.

### Сервер
1. Положите `denwave-server` и `config.simple.yaml` в одну папку.
2. Запустите:
   - Windows: `denwave-server-<версия>-windows-amd64.exe --config config.simple.yaml`
   - Linux: `chmod +x denwave-server-<версия>-linux-amd64 && ./denwave-server-<версия>-linux-amd64 --config config.simple.yaml`
3. В консоли сервер напишет, какие порты открыть и пробросить на роутере (по умолчанию TCP 8080 и UDP 50000) и по какому адресу подключаться. Внешний IP для голоса определяется автоматически.
4. Первый зарегистрированный пользователь становится владельцем сервера.

### Совместимость
Клиент и сервер обновляются независимо. Если версии несовместимы, клиент ещё до входа подскажет, что обновить — клиент или сервер.

### Планы развития
Ближайшие улучшения и долгосрочные направления — в [roadmap](ROADMAP.md#русский). Уже выпущенные изменения — в [Releases](../../releases).

---

## English

**Denwave** is a voice and text chat for teams, communities and companies that runs on your own server. You run the server on your computer or a VPS, and members connect to it with the Denwave app. The server, accounts, messages and settings stay with you — no third-party cloud services.

### Features
- Low-latency voice channels (WebRTC) with noise suppression, echo cancellation and per-user volume.
- Microphone modes: continuous, voice activation, push-to-talk; global hotkeys.
- Server chat, channel chats and direct messages with mentions, Markdown, notifications and commands (`/help`).
- Roles and permissions, password-protected channels and role-based visibility, bans.
- Password sign-in, "remember me" (the key lives in the OS credential store), saved server list.
- HTTPS with an automatic Let's Encrypt certificate or your own files.

### Download
The latest version is on the [Releases](../../releases/latest) page:
- `Denwave-Client-<version>-setup.exe` — client for Windows 10/11;
- `denwave-server-<version>-windows-amd64.exe` and `denwave-server-<version>-linux-amd64` — server;
- `config.simple.yaml` — sample server configuration.

### Client
1. Run the installer. Windows may warn about an unknown publisher: More info → Run anyway.
2. Add the server address you got from its owner, then sign in or create an account.

A newer version installs over the old one and keeps saved servers and settings. Use the installer: a copied exe cannot show Windows notifications.

### Server
1. Put `denwave-server` and `config.simple.yaml` in one folder.
2. Run:
   - Windows: `denwave-server-<version>-windows-amd64.exe --config config.simple.yaml`
   - Linux: `chmod +x denwave-server-<version>-linux-amd64 && ./denwave-server-<version>-linux-amd64 --config config.simple.yaml`
3. The console lists the ports to open and forward on your router (TCP 8080 and UDP 50000 by default) and the addresses to connect to. The external IP for voice is detected automatically.
4. The first registered user becomes the server owner.

### Compatibility
Client and server are updated independently. If they are incompatible, the client tells you before sign-in whether the client or the server needs an update.

### Roadmap
See the [roadmap](ROADMAP.md#english) for upcoming improvements and longer-term directions. Shipped changes are listed in [Releases](../../releases).
