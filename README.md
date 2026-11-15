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
- Камеры и демонстрация экрана в голосовых каналах.
- Режимы микрофона: постоянно, по голосу, push-to-talk; глобальные горячие клавиши.
- Чат сервера, чаты каналов и личные сообщения: реакции, треды, вложения, упоминания, Markdown, уведомления, команды (`/help`).
- Роли и права, иконки ролей, журнал аудита, каналы с паролем и видимостью по ролям, баны.
- Вход с паролем, «запомнить меня» (ключ хранится в системном хранилище), список серверов.
- HTTPS с автоматическим сертификатом Let's Encrypt или своими файлами.
- Обновление клиента из приложения.

### Скачать
Последняя версия — на странице [Releases](../../releases/latest):
- `Denwave-Client-<версия>-setup.exe` — клиент для Windows 10/11;
- `Denwave-Client-<версия>-macos-universal.dmg` — клиент для macOS (без подписи Apple: первый запуск через «Открыть»);
- `denwave-server-<версия>-windows-amd64.exe` и `denwave-server-<версия>-linux-amd64` — сервер.

Конфиг сервера создаётся при первом запуске — отдельный файл скачивать не нужно.

### Клиент
1. Запустите установщик. Windows может предупредить о неизвестном издателе: «Подробнее» → «Выполнить в любом случае».
2. Добавьте адрес сервера, который вам дал его владелец, и войдите или создайте аккаунт.

Новая версия ставится поверх старой, сохранённые серверы и настройки остаются. Устанавливайте именно установщиком: просто скопированный exe не показывает уведомления Windows.

### Сервер
1. Скачайте бинарник сервера в отдельную папку.
2. Запустите его:
   - Windows: `denwave-server-<версия>-windows-amd64.exe`
   - Linux: `chmod +x denwave-server-<версия>-linux-amd64 && ./denwave-server-<версия>-linux-amd64`
3. При первом запуске сервер спросит порт API, каталог данных и пароль сервера, затем создаст `config.simple.yaml` и файлы данных. Данные по умолчанию лежат рядом с бинарником; каталог можно выбрать.
4. В консоли появятся порты для брандмауэра/роутера (по умолчанию TCP 8080 и UDP 50000) и строки `Client address` — этот адрес нужно ввести в клиенте. На Windows, если клиенты не подключаются, выполните `denwave-server.exe firewall open` и подтвердите UAC.
5. Первый зарегистрированный пользователь становится владельцем сервера. Закройте регистрацию в конфиге или задайте пароль сервера, когда закончите настройку.
6. Для HTTPS включите `security.tls_mode` в `config.simple.yaml` (`auto` с доменом или `files` со своими сертификатами) и перезапустите сервер. Для `auto` нужен домен и доступный TCP 443.

### Совместимость
Клиент и сервер обновляются независимо. Если версии несовместимы, клиент ещё до входа подскажет, что обновить — клиент или сервер.

### Планы развития
Ближайшие улучшения и долгосрочные направления — в [roadmap](ROADMAP.md#русский). Уже выпущенные изменения — в [Releases](../../releases).

---

## English

**Denwave** is a voice and text chat for teams, communities and companies that runs on your own server. You run the server on your computer or a VPS, and members connect to it with the Denwave app. The server, accounts, messages and settings stay with you — no third-party cloud services.

### Features
- Low-latency voice channels (WebRTC) with noise suppression, echo cancellation and per-user volume.
- Cameras and screen sharing in voice channels.
- Microphone modes: continuous, voice activation, push-to-talk; global hotkeys.
- Server chat, channel chats and direct messages with reactions, threads, attachments, mentions, Markdown, notifications and commands (`/help`).
- Roles and permissions, role icons, audit log, password-protected channels and role-based visibility, bans.
- Password sign-in, "remember me" (the key lives in the OS credential store), saved server list.
- HTTPS with an automatic Let's Encrypt certificate or your own files.
- In-app client updates.

### Download
The latest version is on the [Releases](../../releases/latest) page:
- `Denwave-Client-<version>-setup.exe` — client for Windows 10/11;
- `Denwave-Client-<version>-macos-universal.dmg` — macOS client (not signed by Apple: first launch via Open);
- `denwave-server-<version>-windows-amd64.exe` and `denwave-server-<version>-linux-amd64` — server.

The server creates its config on first run; there is no separate config file to download.

### Client
1. Run the installer. Windows may warn about an unknown publisher: More info → Run anyway.
2. Add the server address you got from its owner, then sign in or create an account.

A newer version installs over the old one and keeps saved servers and settings. Use the installer: a copied exe cannot show Windows notifications.

### Server
1. Download the server binary into its own folder.
2. Run it:
   - Windows: `denwave-server-<version>-windows-amd64.exe`
   - Linux: `chmod +x denwave-server-<version>-linux-amd64 && ./denwave-server-<version>-linux-amd64`
3. On first start the server asks for the API port, data directory and server password, then creates `config.simple.yaml` and the data files. Data lives next to the binary by default; you can choose another directory.
4. The console lists the ports to allow/forward (TCP 8080 and UDP 50000 by default) and `Client address` lines — enter one of those addresses in the client. On Windows, if clients cannot connect, run `denwave-server.exe firewall open` and confirm UAC.
5. The first registered user becomes the server owner. Close registration in the config or set a server password when setup is done.
6. For HTTPS set `security.tls_mode` in `config.simple.yaml` (`auto` with a domain or `files` with your certificates) and restart. `auto` needs a domain and reachable TCP 443.

### Compatibility
Client and server are updated independently. If they are incompatible, the client tells you before sign-in whether the client or the server needs an update.

### Roadmap
See the [roadmap](ROADMAP.md#english) for upcoming improvements and longer-term directions. Shipped changes are listed in [Releases](../../releases).
