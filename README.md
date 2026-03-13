<div align="center">

<img src="https://github.com/Endscape-Coding/EN-OS/blob/main/Images/logofl.png" alt="EN-OS Utils Logo">

# 🖥️ EN-OS-Utils

**Центральный хаб утилит экосистемы EN-OS** <br>
***Central Hub for EN-OS Ecosystem Utilities***

</div>

<div align="center">

[![Rust](https://img.shields.io/badge/Rust-orange?style=for-the-badge&logo=rust)](#)
[![Python](https://img.shields.io/badge/Python-yellow?style=for-the-badge&logo=python)](#)
[![Status](https://img.shields.io/badge/🟢-Active%20Development-green?style=for-the-badge)](#)

</div>

<p align="center">
  <a href="#-русский">Русский</a> • <a href="#-english">English</a>
</p>

---
## 🇷🇺 Русский

<div align="center">

[О проекте](#-о-проекте) • [Каталог утилит](#-каталог-утилит) • [Безопасность](#-безопасность) • [Вклад в проект](#-вклад-в-проект) • [Статус компонентов](#-статус-компонентов) • [Контакты](#-контакты-и-сообщество)

</div>

### 📋 О проекте

**EN-OS-Utils** - это мета-репозиторий, объединяющий все утилиты и инструменты экосистемы **EN-OS**, современного Linux-дистрибутива на базе Arch Linux. Здесь вы найдёте ссылки на все компоненты системы с кратким описанием их назначения, технологий и текущего статуса.

> 💡 **Совет**: Используйте этот README как навигатор по экосистеме. Каждый репозиторий содержит подробную документацию, инструкции по сборке и использованию.

---

### 🗂️ Каталог утилит

#### 🔧 Системные утилиты
**[EN-OS-System-Manager](https://github.com/Endscape-Coding/EN-OS-System-Manager)** Графический центр управления системой: мониторинг, настройки, управление сервисами и пакетами.

**[EN-OS-Zram-Manager](https://github.com/Endscape-Coding/EN-OS-Zram-Manager)** Универсальный менеджер ZRam: настройка алгоритмов сжатия, размера swap, мониторинг использования памяти и CPU. Работает на любых systemd-дистрибутивах.

**[EN-OS-Pacman-Key-Manager](https://github.com/Endscape-Coding/EN-OS-Pacman-Key-Manager)** Утилита для управления ключами pacman: базовые операции с ключами репозиториев.

#### 🌐 Удалённое управление и автоматизация
**[EN-OS-Remote-Assistant](https://github.com/Endscape-Coding/EN-OS-Remote-Assistant)** Telegram-бот для удалённого управления ПК: выполнение команд, скриншоты, управление файлами. Поддержка X11/Wayland, эмуляция ввода через ydotool.

**[EN-OS-Live-Welcome](https://github.com/Endscape-Coding/EN-OS-Live-Welcome)** Приветственный GUI для Live-сессий EN-OS: быстрый запуск установки, справка, выбор языковых настроек.

#### 🛠️ Сборка и дистрибуция
**[EN-OS-Builds](https://github.com/Endscape-Coding/EN-OS-Builds)**. Скрипты и конфигурации для сборки программ EN-OS: профили сборок, автоматизация, управление версиями.

**[EN-OS-Calamares](https://github.com/Endscape-Coding/EN-OS-Calamares)** Кастомизированная конфигурация установщика Calamares для EN-OS: добавлены особые модули и многое другое.

**[EN-Repository](https://github.com/Endscape-Coding/EN-Repository)** | Конфигурация официального репозитория EN-OS: структура пакетов, управление версиями, зеркалирование.

#### 🎨 Интерфейс и персонализация
**[en-os-fastfetch](https://github.com/Endscape-Coding/en-os-fastfetch)** Fastfetch с логотипом EN-OS.

#### 📱 Для мобилок
**[EN-OS-termux](https://github.com/Endscape-Coding/EN-OS-termux)** Небольшой форк Termux desktop с улучшенным скриптом и обновленными пакетами.

---

### 🔐 Безопасность

- Некоторые утилиты требуют `sudo` и явно запрашивают подтверждение.
- Исходный код открыт: вы можете аудитировать любую утилиту перед использованием.
- На текущем этапе репозиторий не использует GPG-подпись пакетов — мы работаем над внедрением системы верификации в будущих релизах.
- При использовании `Remote-Assistant` (в разработке) обязательно настройте `.env` с `TELOXIDE_TOKEN` и `ID` для ограничения доступа.

---

### 🤝 Вклад в проект

EN-OS — проект с открытым исходным кодом, и мы приветствуем участие сообщества:

1. **Сообщите об ошибке**: [Issues](https://github.com/Endscape-Coding/EN-OS-Programs/issues)
2. **Предложите улучшение**: Обсудите идею в Issue перед PR
3. **Напишите код**: Следуйте [CONTRIBUTING.md](./CONTRIBUTING.md) (скоро)
4. **Протестируйте**: Особенно важны тесты на разном железе и в Live-режиме

#### 📌 Правила для PR
- ✅ Код на Rust должен проходить `cargo clippy` и `cargo fmt`
- ✅ Документация на русском и английском
- ✅ Тесты для новых функций (где применимо)
- ✅ Совместимость с systemd и Arch-based системами

---

### 📊 Статус компонентов

| Компонент | Статус | Доступность |
|-----------|--------|-------------|
| System-Manager | 🟢 Готов | ✅ В репозитории |
| EN-OS-Builds | ⚪ Работает | ✅ В репозитории |
| EN-Repository | ⚪ Работает | ✅ Работает |
| en-os-fastfetch | ⚪ Работает | ✅ В репозитории |
| Zram-Manager | 🟡 В разработке | 🔜 В Testing репозитории |
| Remote-Assistant | 🟡 В разработке | 🔜 Скоро |
| Live-Welcome | 🟡 В разработке | 🔜 В Testing репозитории |
| Pacman-Key-Manager | 🟡 В разработке | 🔜 В Testing репозитории |
| EN-OS-Calamares | ⚪ Работает | ✅ В репозитории |
| EN-OS-termux | 🧪 Эксперимент | 🔬 По приколу |

> 🔄 Все репозитории используют **rolling-release** модель: обновления доступны сразу после тестирования.

---

### 🌍 Поддержка языков

| Утилита | 🇷🇺 Русский | 🇬🇧 English | 🌐 Другие |
|---------|-----------|-----------|----------|
| System-Manager | ✅ | ✅ | Поддерживается большинство языков |
| Remote-Assistant | ✅ | ✅ | — |
| Live-Welcome | ✅ | ✅ | Поддерживается большинство языков |

---

### 📬 Контакты и сообщество

- **Telegram-канал**: [@Linux_EN_OS](https://t.me/Linux_EN_OS)
- **GitHub Issues**: [Сообщить об ошибке](https://github.com/Endscape-Coding/EN-OS-Programs/issues)
- **Email**: endscape.coding@gmail.com
- **Документация**: [Wiki (скоро)](https://github.com/Endscape-Coding/EN-OS-Programs/wiki)

---

### 📄 Лицензии

Большинство утилит распространяются под лицензиями:
- **AGPL-3.0** — для сетевых и удалённых компонентов
- **GPL-3.0** — для GUI и системных утилит

Полный текст лицензий находится в файле `LICENSE` каждого репозитория.

---

## 🇬🇧 English

<div align="center">

[About](#-about-the-project) • [Utilities Catalog](#-utilities-catalog) • [Security](#-security) • [Contributing](#-contributing) • [Component Status](#-component-status) • [Contacts](#-contacts--community)

</div>

### 📋 About the Project

**EN-OS-Utils** is a meta-repository that unites all utilities and tools of the **EN-OS** ecosystem, a modern Linux distribution based on Arch Linux. Here you will find links to all system components with brief descriptions of their purpose, technologies, and current status.

> 💡 **Tip**: Use this README as a navigator through the ecosystem. Each repository contains detailed documentation, build instructions, and usage guides.

---

### 🗂️ Utilities Catalog

#### 🔧 System Utilities

**[EN-OS-System-Manager](https://github.com/Endscape-Coding/EN-OS-System-Manager)**  
Graphical system control center: monitoring, settings, service and package management.

**[EN-OS-Zram-Manager](https://github.com/Endscape-Coding/EN-OS-Zram-Manager)**  
Universal ZRam manager: configure compression algorithms, swap size, monitor memory and CPU usage. Works on any systemd-based distribution.

**[EN-OS-Pacman-Key-Manager](https://github.com/Endscape-Coding/EN-OS-Pacman-Key-Manager)**  
Utility for managing pacman keys: basic operations with repository keys.

#### 🌐 Remote Control & Automation

**[EN-OS-Remote-Assistant](https://github.com/Endscape-Coding/EN-OS-Remote-Assistant)**  
Telegram bot for remote PC control: command execution, screenshots, file management. Supports X11/Wayland, input emulation via ydotool.

**[EN-OS-Live-Welcome](https://github.com/Endscape-Coding/EN-OS-Live-Welcome)**  
Welcome GUI for EN-OS Live sessions: quick installer launch, help, language settings selection.

#### 🛠️ Build & Distribution

**[EN-OS-Builds](https://github.com/Endscape-Coding/EN-OS-Builds)**  
Scripts and configurations for building EN-OS programs: build profiles, automation, version management.

**[EN-OS-Calamares](https://github.com/Endscape-Coding/EN-OS-Calamares)**  
Customized Calamares installer configuration for EN-OS: added custom modules and more.

**[EN-Repository](https://github.com/Endscape-Coding/EN-Repository)**  
Official EN-OS repository configuration: package structure, version management, mirroring.

#### 🎨 Interface & Personalization

**[en-os-fastfetch](https://github.com/Endscape-Coding/en-os-fastfetch)**  
Fastfetch with EN-OS logo.

#### 📱 For Mobile

**[EN-OS-termux](https://github.com/Endscape-Coding/EN-OS-termux)**  
A small Termux desktop fork with an improved script and updated packages.

---

### 🔐 Security

- Some utilities require `sudo` and explicitly request confirmation.
- Source code is open: you can audit any utility before use.
- At this stage, the repository does not use GPG package signing — we are working on implementing a verification system in future releases.
- When using `Remote-Assistant` (in development), be sure to configure `.env` with `TELOXIDE_TOKEN` and `ID` to restrict access.

---

### 🤝 Contributing

EN-OS is an open-source project, and we welcome community participation:

1. **Report a bug**: [Issues](https://github.com/Endscape-Coding/EN-OS-Programs/issues)
2. **Suggest an improvement**: Discuss your idea in an Issue before submitting a PR
3. **Write code**: Follow [CONTRIBUTING.md](./CONTRIBUTING.md) (coming soon)
4. **Test**: Tests on different hardware and in Live mode are especially valuable

#### 📌 PR Guidelines
- ✅ Rust code must pass `cargo clippy` and `cargo fmt`
- ✅ Documentation in both Russian and English
- ✅ Tests for new features (where applicable)
- ✅ Compatibility with systemd and Arch-based systems

---

### 📊 Component Status

| Component | Status | Availability |
|-----------|--------|--------------|
| System-Manager | 🟢 Ready | ✅ In repository |
| EN-OS-Builds | ⚪ Works | ✅ In repository |
| EN-Repository | ⚪ Works | ✅ Active |
| en-os-fastfetch | ⚪ Works | ✅ In repository |
| Zram-Manager | 🟡 In development | 🔜 In Testing repository |
| Remote-Assistant | 🟡 In development | 🔜 Coming soon |
| Live-Welcome | 🟡 In development | 🔜 In Testing repository |
| Pacman-Key-Manager | 🟡 In development | 🔜 In Testing repository |
| EN-OS-Calamares | ⚪ Works | ✅ In repository |
| EN-OS-termux | 🧪 Experimental | 🔬 For fun |

> 🔄 All repositories follow a **rolling-release** model: updates are available immediately after testing.

---

### 🌍 Language Support

| Utility | 🇷🇺 Russian | 🇬🇧 English | 🌐 Others |
|---------|-----------|-----------|----------|
| System-Manager | ✅ | ✅ | Most languages supported |
| Remote-Assistant | ✅ | ✅ | — |
| Live-Welcome | ✅ | ✅ | Most languages supported |

---

### 📬 Contacts & Community

- **Telegram channel**: [@Linux_EN_OS](https://t.me/Linux_EN_OS)
- **GitHub Issues**: [Report a bug](https://github.com/Endscape-Coding/EN-OS-Programs/issues)
- **Email**: endscape.coding@gmail.com
- **Documentation**: [Wiki (coming soon)](https://github.com/Endscape-Coding/EN-OS-Programs/wiki)

---

### 📄 Licenses

Most utilities are distributed under the following licenses:
- **AGPL-3.0** — for network and remote components
- **GPL-3.0** — for GUI and system utilities

Full license texts are located in the `LICENSE` file of each repository.

<div align="right">

[⬆ Back to Top](#-en-os-utils)

</div>

---

> 💬 *"EN-OS is not just a distribution — it's an ecosystem where every utility is designed for maximum flexibility, security, and simplicity. Welcome to the future of Linux."*  
> — Endscape

⭐ **Star the repo** if you find this project useful!  
🔁 **Fork it** to suggest improvements or adapt it to your needs.

---

*Last updated: March 2026*  
*Compatible with: Arch Linux, EN-OS, Arch-based distributions*
