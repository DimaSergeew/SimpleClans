# 📘 Конфигурация

[Главный конфигурационный файл для SimpleClans можно найти здесь.](https://github.com/RoinujNosde/SimpleClans/blob/master/src/main/resources/config.yml)

## Главные настройки

| Опция                                | Описание                                                                                                                                                                                                                                                                              | По умолчанию                       |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| `enable-gui`                         | Включить GUI                                                                                                                                                                                                                                                                          | `true`                             |
| `disable-messages`                   | Отключить такие оповещения, как "Клан создан", "Клан расформирован", и другие                                                                                                                                                                                                         | `false`                            |
| `tameable-mobs-sharing`              | Если включено, то приручаемые мобы будут поделены с участниками вашего клана. Также отключает любой клановый урон, наносимый по ним                                                                                                                                                   | `false`                            |
| `teleport-blocks`                    | Мягкое телепортирование (блок стекла под ногами)                                                                                                                                                                                                                                      | `false`                            |
| `teleport-home-on-spawn`             | При возрождении игроки будут телепортированы на базу клана                                                                                                                                                                                                                            | <p><code>false</code><br></p>      |
| `drop-items-on-clan-home`            | При телепортации на базу клана, выкидывать предметы на землю                                                                                                                                                                                                                          | `false`                            |
| `keep-items-on-clan-hom`             | При телепортации на базу клана, оставлять предметы                                                                                                                                                                                                                                    | <p><code>false</code><br><br></p>  |
| `item-list`                          | Список предметов. Используется в связке с `keep-items-on-clan-home` и `drop-items-on-clan-home`                                                                                                                                                                                       | <p><code>[]</code><br></p>         |
| `show-debug-info`                    | Показать отладочную информацию в консоли                                                                                                                                                                                                                                              | `false`                            |
| `enable-auto-groups`                 | <p>Управляет группами автоматически. При условии, что у вас есть LuckPerms, а в ней создана любая из следующих групп:</p><ul><li>sc_leader</li><li>sc_trusted</li><li>sc_untrusted</li></ul><p>Будет автоматически закидывать игроков в эту группу</p>                                | <p><code>false</code><br><br></p>  |
| `chat-compatibility-mode`            | Режим совместимости с чатом. Если у вас есть какие-либо проблемы с чатом, попробуйте выключить этот параметр                                                                                                                                                                          | `true`                             |
| `rival-limit-percent`                | <p>Процент возможных соперников на клан.</p><p>Форумула: <code>(rivalsOfClan - 1) * rivalLimitPercent / 100</code></p>                                                                                                                                                                | <p><br><br><code>50</code><br></p> |
| `use-colorcode-from-prefix-for-name` | Использовать последний цветовой код в конце префикса                                                                                                                                                                                                                                  | <p><code>true</code><br></p>       |
| `display-chat-tags`                  | Отображать тег клана в чате                                                                                                                                                                                                                                                           | `true`                             |
| `unrivable-clans`                    | Список кланов, с которыми невозможно начать вражду                                                                                                                                                                                                                                    | `[]`                               |
| `show-unverified-on-list`            | Показывать **не** подтерждённые кланы в `/clan list`                                                                                                                                                                                                                                  | `false`                            |
| `blacklisted-worlds`                 | Список миров, где SimpleClans не будет работать                                                                                                                                                                                                                                       | `[]`                               |
| `banned-players`                     | Список игроков, которые не могут пользоваться командами плагина                                                                                                                                                                                                                       | <p><code>[]</code><br></p>         |
| `disallowed-tags`                    | Список запрещенных тегов                                                                                                                                                                                                                                                              | `[]`                               |
| `language`                           | Язык по умолчанию                                                                                                                                                                                                                                                                     | <p><code>en</code><br></p>         |
| `user-language-selector`             | Позволяет игрокам менять их язык                                                                                                                                                                                                                                                      | `true`                             |
| `disallowed-tag-colors`              | Список запрещенных цветовых кодов для тега                                                                                                                                                                                                                                            | <p><code>[]</code><br></p>         |
| `server-name`                        | Название вашего сервера                                                                                                                                                                                                                                                               | `&4SimpleClans`                    |
| `new-clan-verification-require`      | Должны ли новые кланы проходить верификацию?                                                                                                                                                                                                                                          | `true`                             |
| `allow-regroup-command`              | Разрешить ли команду для перегруппировки (телепортации игроков к себе/на базу)                                                                                                                                                                                                        | <p><code>true</code><br></p>       |
| `allow-reset-kdr`                    | <p>Разрешить сброс КДР <br>(соотношение убийств к смертям)</p>                                                                                                                                                                                                                        | `true`                             |
| `rejoin-cooldown`                    | Время в минутах, когда игрок сможет присоединиться к клану после выхода из него.                                                                                                                                                                                                      | `60`                               |
| `rejoin-cooldown-enabled`            | Должен ли быть включен таймер пере-присоединения включен?                                                                                                                                                                                                                             | `false`                            |
| `min-to-verify`                      | <p>Количество игроков в клане, чтобы можно было пройти подтверждение </p><p>(Модераторы могут обойти это ограничение)</p>                                                                                                                                                             |                                    |
| `ranking-type`                       | <p></p><p>Допустимые параметры: ORDINAL или DENSE</p><ul><li><code>DENSE</code>: Если у игроков будет одинаковый KDR, их ранговая позиция будет одинаковой. Пример: 12234</li><li><code>ORDINAL</code>: Каждый игрок будет иметь разную ранговую позицию. <br>Пример: 12345</li></ul> | `DENSE`                            |

### Пример

```yaml
settings:
    enable-gui: true
    disable-messages: false
    tameable-mobs-sharing: false
    teleport-blocks: false
    teleport-home-on-spawn: false
    drop-items-on-clan-home: false
    keep-items-on-clan-home: false
    item-list: []
    show-debug-info: false
    mchat-integration: true
    enable-auto-groups: false
    chat-compatibility-mode: true
    rival-limit-percent: 50
    use-colorcode-from-prefix-for-name: true
    display-chat-tags: true
    unrivable-clans:
    - admin
    - staff
    - mod
    show-unverified-on-list: false
    blacklisted-worlds: []
    banned-players: []
    disallowed-tags:
    - vip
    - clan
    language: en
    language-per-player: false
    disallowed-tag-colors:
    - '4'
    server-name: '&4SimpleClans'
    new-clan-verification-required: true
    allow-regroup-command: true
    allow-reset-kdr: false
    rejoin-cooldown: 60
    rejoin-cooldown-enabled: false
    min-to-verify: 1
    ranking-type: DENSE
```

## Формат тегов

#### Пример

* `default-color` - Цвет по-умолчанию
* `max-length` - Максимальная длинна
* `bracket` - Скобки
  * `color` - Цвет
  * `leader-color` - Цвет лидера
  * `left` - Слева
  * `right` - Справа
* `min-length` - Минимальная длина
* `separator` - Разделитель
  * `color` - Цвет
  * `leader-color` - Цвет лидера
  * `char` - Символ

```yaml
tag:
    default-color: '8'
    max-length: 5
    bracket:
        color: '8'
        leader-color: '4'
        left: ''
        right: ''
    min-length: 2
    separator:
        color: '8'
        leader-color: '4'
        char: ' .'
```

## Основные команды

В этой секции вы можете редактировать команды плагина. Если какой-то другой плагин уже занимает эти команды, включение `force-priority` на `true` должно помочь.

#### Пример

```yaml
commands:
    more: more
    ally: ally
    clan: clan
    accept: accept
    deny: deny
    global: global # Удаленная опция, в новых версиях не встретите.
    clan_chat: "."
    force-priority: true
```

## Защита от набивания KDR

* `enable-max-kills` - Включить максимальное количество убийств
* `max-kills-per-victim` - Максимальное количество убийств за жертву
* `enable-kill-delay` - Включить задержку перед убийствами
* `delay-between-kills` - Задержка перед убийствами

#### Пример

```yaml
kdr-grinding-prevention:
    enable-max-kills: false
    max-kills-per-victim: 10
    enable-kill-delay: false
    delay-between-kills: 5
```

## Экономика

* `creation-price` - Цена создания клана&#x20;
* `purchase-clan-create` - Брать ли денги за создание клана?
* `verification-price` - Цена подтверждения
* `purchase-clan-verify` - Брать ли денги за подтверждение клана?
* `invite-price` - Цена приглашения
* `purchase-clan-invite` - Брать ли денги за приглашение в клан?
* `home-teleport-price` - Цена телепортации на базу клана
* `purchase-home-teleport` - Брать ли денги за телепорт на базу клана?
* `home-teleport-set-price` - Цена установки точки базы клана
* `purchase-home-teleport-set` - Брать ли денги за установку точки базы клана?
* `home-regroup-price` - Цена перегруппировки на точку базы клана
* `purchase-home-regroup` - Брать ли денги за перегруппировку на точку базы клана?
* `unique-tax-on-regroup` - Если `false`, цена умножается на количество онлайн-членов клана.
* `issuer-pays-regroup` - Брать ли деньги с того, кто вызвал перегруппировку?
* `money-per-kill` - Награждать ли игроков за убийство?
* `money-per-kill-kdr-multipier` - Множитель убийства.
* `purchase-reset-kdr` - Брать ли денги за сброс KDR?
* `reset-kdr-price` - Цена сброса KDR.
* `purchase-member-fee-set` - Брать ли денги за перегруппировку на точку базы клана
* `member-fee-set-price` - Комиссия на участников.
* `member-fee-enabled` - Включить ли комиссию на участников?
* `max-member-fee` - Максимальная комиссия участников.
* `upkeep` - Коммисия на поддержание клана.
* `upkeep-enabled` - Включить ли комиссию на содержание клана?
* `multiply-upkeep-by-clan-size` - Должна ли комиссия на содержание зависеть от количества участников в клане?
* `charge-upkeep-only-if-member-fee-enabled` - Должна ли комиссия на содержание быть взята только у тех, кто её включил?

#### Пример

```yaml
economy:
    creation-price: 100.0
    purchase-clan-create: false
    verification-price: 1000.0
    purchase-clan-verify: false
    invite-price: 20.0
    purchase-clan-invite: false
    home-teleport-price: 5.0
    purchase-home-teleport: false
    home-teleport-set-price: 5.0
    purchase-home-teleport-set: false
    home-regroup-price: 5.0
    purchase-home-regroup: false
    unique-tax-on-regroup: true
    issuer-pays-regroup: true
    money-per-kill: false
    money-per-kill-kdr-multipier: 10
    purchase-reset-kdr: true
    reset-kdr-price: 10000.0
    purchase-member-fee-set: false
    member-fee-set-price: 1000.0
    member-fee-enabled: false
    max-member-fee: 200.0
    upkeep: 200.0
    upkeep-enabled: false
    multiply-upkeep-by-clan-size: false
    charge-upkeep-only-if-member-fee-enabled: true
```

## Вес убийств

Здесь вы можете установить вес каждого типа убийства. Вес также может быть отрицательным. Он используется для вычисления KDR следующим образом: \
`(Количество убийств * вес убийства) / Количество смертей = KDR`

#### Пример

```yaml
kill-weights:
    rival: 2.0 # соперник/противник
    civilian: 0.0 # мирный/без клана
    neutral: 1.0 # нейтральный
    deny-same-ip-kills: false # Отменять убийства с одного айпи адреса
```

## Настройки клана&#x20;

* `homebase-teleport-wait-secs` - Задержка перед телепортацией на точку базы клана
* `homebase-can-be-set-only-once` - Точка базы клана может быть установлена единожды
* `min-size-to-set-rival` - Минимальное количество участников клана для добавления соперников
* `max-length` - Максимальная длина названия клана.
* `max-description-length` - Максимальная длина описания клана
* `min-description-length` - Минимальная длина описания клана.
* `max-members` - Максимальное количество участников
* `confirmation-for-promote` - Должны ли другие лидеры подтвердить повышение участника?
* `trust-members-by-default` - Подтверждать участников по умолчанию?
* `confirmation-for-demote` - Должны ли другие лидеры подтвердить понижение участника?
* `percentage-online-to-demote` - Процент лидеров онлайн для понижения.
* `ff-on-by-default` - Глобальный "Огонь по своим" включен по умолчанию.
* `min-length` - Минимальная длина названия клана.
* `min-size-to-set-ally` - Минимальное количество участников клана для добавления союзников.
* `min-to-verify` - Клан должен иметь следующее число участников, чтобы подтвердить свой клан (модераторы могут обойти это)

#### Пример

```yaml
clan:
    homebase-teleport-wait-secs: 10
    homebase-can-be-set-only-once: true
    min-size-to-set-rival: 3
    max-length: 25
    max-description-length: 120
    min-description-length: 10
    max-members: 25
    confirmation-for-promote: false
    trust-members-by-default: false
    confirmation-for-demote: false
    percentage-online-to-demote: 100.0
    ff-on-by-default: false
    min-length: 2
    min-size-to-set-ally: 3
```

## Запланированные задачи

* `collect-upkeep` - Сбор комиссии на содержание клана
  * `hour` - час
  * `minute` - минуты
* `collect-upkeep-warning` - Предупреждение о сборе комисии на поддержание клана
  * `hour` - час&#x20;
  * `minute` - минуты&#x20;
* `collect-fee` - Сбор комиссии
  * `hour` - час
  * `minute` - минуты

#### Пример

```yaml
tasks:
    collect-upkeep:
        hour: 1
        minute: 30
    collect-upkeep-warning:
        hour: 12
        minute: 0
    collect-fee:
        hour: 1
        minute: 0
```

## Страницы

* `untrusted-color` - Цвет неподтвержденного клана
* `clan-name-color` - Цвет названия клана
* `subtitle-color` - Цвет подзаголовков
* `headings-color` - Цвет заголовков
* `trusted-color` - Цвет подтвержденного клана
* `leader-color` - Цвет лидера
* `separator` - Разделитель
* `size` - Размер

#### Пример

```yaml
page:
    untrusted-color: '8'
    clan-name-color: b
    subtitle-color: '7'
    headings-color: '8'
    trusted-color: f
    leader-color: '4'
    separator: '-'
    size: 100
```

## Чат клана

* `enable` - Включить клановый чат?
* `tag-based-clan-chat` - Если `true` командой для отправки сообщения в клановый чат станет ваш клан тег.
* `announcement-color` - Цвет, используемый для оповещений.
* `format` - Формат отображения чата
* `rank` - Формат отображения ранга
* `leader-color:` - Цвет лидера в чате
* `trusted-color` - Цвет подтвержденного участника в чате&#x20;
* `member-color` - Цвет участника в чате

#### Пример

```yaml
clanchat:
    enable: true
    tag-based-clan-chat: false
    announcement-color: e
    format: "&b[%clan%&b] &4<%nick-color%%player%&4> %rank%: &b%message%"
    rank: "&f[%rank%&f]"
    leader-color: '4'
    trusted-color: 'f'
    member-color: '7'
```

## Discord чат

Вы можете посмотреть описание конфигурации [здесь](../integracii/discordsrv.md#konfiguraciya).

## Запросы

* `message-color` - Цвет сообщений
* `ask-frequency-secs` - Интервал (в секундах) между сообщениями
* `max-asks-per-request` - Максимальное кол-во сообщений перед истечением срока запроса.

#### Пример

```yaml
request:
    message-color: b
    ask-frequency-secs: 60
    max-asks-per-request: 1440
```

## Доска объявлений клана

* `color` - Цвет
* `accent-color` - Цвет акцента
* `show-on-login` - Показывать при входе?
* `size` - Размер
* `login-size` - Размер на входе

#### Пример

```yaml
bb:
    color: e
    accent-color: '8'
    show-on-login: true
    size: 6
    login-size: 6
```

## Союзный чат

* `enable` - Включить союзный чат?
* `format` - Формат чата
* `rank` - Формат ранга
* `leader-color` - Цвет лидера
* `trusted-color` - Цвет подтвержденного участника
* `member-color` - Цвет участника

#### Пример

```yaml
allychat:
    enable: true
    format: "&b[Ally Chat] &4<%clan%&4> <%nick-color%%player%&4> %rank%: &b%message%"
    rank: "&f[%rank%&f]"
    leader-color: '4'
    trusted-color: 'f'
    member-color: '7'
```

## Очистка данных

* `inactive-player-data-days` - Через сколько дней будут очищены данные о неактивных игроках?
* `inactive-clan-days` - Через сколько дней будут очищены не активные кланы?
* `unverified-clan-days` - Через сколько дней будут очищены не активные и не подтвержденные кланы?

#### Пример

```yaml
purge:
    inactive-player-data-days: 30
    inactive-clan-days: 7
    unverified-clan-days: 2
```

## MySQL настройки

* `username` - Логин
* `host` - Хост
* `port` - Порт
* `enable` - Включить MySQL подключение?
* `password` - Пароль
* `database` - База данных

#### Пример

```yaml
mysql:
    username: ''
    host: localhost
    port: 3306
    enable: false
    password: ''
    database: ''
```

## Разрешения

* `auto-group-groupname` -&#x20;

#### Пример

```yaml
permissions:
  auto-group-groupname: false
  YourClanNameHere:
  - test.permission
```

## Производительность

* `save-periodically` - Плагин будет периодически сохранять данные, а не сразу.\
  **Рекомендуется** установить данный параметр на `true`.\

* `save-interval` - Интервал **в минутах**, в течение которого изменения записываются в базу данных.\

* `use-threads` - Плагин не будет использовать основной поток для подключения к БД.\
  **Рекомендуется** установить данный параметр на `true`.\

* `use-bungeecord` - Использовать bungeecord? (WIP)

#### Пример

```yaml
performance:
  save-periodically: true
  save-interval: 10
  use-threads: true
  use-bungeecord: false
```

## Защита мирных игроков

* `safe-civilians` - Мирные игроки(без клана) будут защищены от PVP.

#### Пример

```yaml
safe-civilians: false
```
