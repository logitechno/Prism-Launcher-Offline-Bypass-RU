# Об этом проекте
Обход проверки наличия у пользователя аккаунта Microsoft<br>
⚠️ Только в образовательных и экспериментальных целях. Не для коммерческого использования. ⚠️

# Перед установкой
Если у вас есть сохраненные аккаунты, то выполнение этого скрипта приведёт к их удалению!

# Как использовать
- Установите Prism Launcher
- Выполните быструю настройку
- ЗАКРОЙТЕ ЛАУНЧЕР
- Выполните команду для обхода (смотрите [ниже](#использование-для-установщика))
- Создайте оффлайн аккаунт
- Установить созданный аккаунт по умолчанию
- Радуйтесь!

# Чего нестоит делать
Не удаляйте "Нет профиля", это нарушит работу обхода!

# Как это работает?
Лаунчер использует файл "accounts.json", в котором хранится информация об учётных записях пользователей. В нём также указывается, владеет ли пользователь лицензией Minecraft. Эта функция позволяет игрокам играть в Minecraft, даже если они находятся в оффлайне, например, на Steam Deck посреди леса. Эту функцию можно использовать для получения доступа к лаунчеру и ресурсам Minecraft.

# Как поставить пользовательский скин?
Для этого вы можете воспользоваться Ely.by в [ElyPrismLauncher](https://github.com/Octol1ttle/ElyPrismLauncher)

# Использование для установщика
Загрузите последнюю версию [Prism Launcher](https://prismlauncher.org/), установите ее, выполните быструю настройку, закройте программу запуска, затем выполните эту команду в терминале:
### Windows CMD:
```
echo {"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3} > %appdata%/PrismLauncher/accounts.json
```
### Linux Shell:
```
echo '{"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3}' > ~/.local/share/PrismLauncher/accounts.json
```
### Linux Shell (flatpak):
```
echo '{"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3}' > ~/.var/app/org.prismlauncher.PrismLauncher/data/PrismLauncher/accounts.json
```
### macOS
```
echo '{"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3}' > ~/Library/Application\ Support/PrismLauncher/accounts.json
```

# Использование для портативной версии
Загрузите портативную версию [Prism Launcher](https://prismlauncher.org/), запустите ее, выполните быструю настройку, закройте программу запуска, затем выполните эту команду в терминале:
### Windows Portable (в корневом каталоге лаунчера) CMD:
```
echo {"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3} > accounts.json
```
### Linux Portable (в корневом каталоге лаунчера) Shell:
```
echo '{"accounts": [{"entitlement": {"canPlayMinecraft": true,"ownsMinecraft": true},"type": "MSA"}],"formatVersion": 3}' > accounts.json
```

# Ручная установка
Скачайте файл под названием [accounts.json](https://github.com/logitechno/Prism-Launcher-Offline-Bypass-RU/blob/main/accounts.json) и вставить его по этому пути:
### Установщик
* Windows: `%appdata%/PrismLauncher/`
* Linux: `~/.local/share/PrismLauncher/`
* Linux (flatpak): `~/.var/app/org.prismlauncher.PrismLauncher/data/PrismLauncher/`
* macOS: `~/Library/Application\ Support/PrismLauncher/`

### Портативная
В корневом каталоге лаунчера

## Официальный репозиторий: [ТЫК](https://github.com/antunnitraj/Prism-Launcher-PolyMC-Offline-Bypass/tree/main)
