# 🚦 Разрешения

## Супер-права

Эти права – быстрый способ настроить SimpleClans. Некоторые из них добавлены автоматически (см. приписку авто). Если вы хотите настроить каждое разрешение по отдельности (см. индивидуальные права), то сперва отрицайте эти права.

| Право                                 | Описание                    |
| ------------------------------------- | --------------------------- |
| `simpleclans.anyone.*` (Авто)         | Разрешения любого игрока    |
| `simpleclans.member.*` (Авто)         | Разрешения участников клана |
| `simpleclans.leader.*` (Авто)         | Разрешения лидеров клана    |
| `simpleclans.mod.*` (Авто к OP'кам)   | Разрешения модераторов      |
| `simpleclans.admin.*` (Авто к OP'кам) | Разрешения администраторов  |

## Индивидуальные права

Вам не нужно добавлять их, если они добавлены [автоматически ](permissions.md#superperms-prava-nekotorye-dobavlyayutsya-avtomaticheski)(супер-права).\
\
Индивидуальные права существуют только на тот случай, если вы хотите \
настроить разрешения _по отдельности._ \
\
Чтобы начать настройку прав, сперва отрицайте супер-право и установите нужное из этого списка на `false`.

**Пример №1**: мы хотим, чтобы никто не мог пользоваться командой `/clan list`\
``Для этого мы поставим `simpleclans.anyone.list` на`false` - всё, теперь никто не сможет пользоваться этой командой.

**Пример №2**: мы хотим настроить разрешения для лидеров по отдельности.\
Для этого сначала мы поставим `simpleclans.leader.*` на `false`, а уже потом будем настраивать каждое.

### Разрешения любого игрока

| Право                              | Описание                                                       |
| ---------------------------------- | -------------------------------------------------------------- |
| `simpleclans.anyone.alliances`     | Может просматривать список союзников всех кланов               |
| `simpleclans.anyone.leaderboard`   | Может посмотреть таблицу лидеров                               |
| `simpleclans.anyone.list`          | Может посмотреть список всех кланов                            |
| `simpleclans.anyone.lookup`        | Может посмотреть информацию об игроках                         |
| `simpleclans.anyone.profile`       | Может посматривать профили кланов                              |
| `simpleclans.anyone.rivalries`     | Может посмотреть список противников всех кланов                |
| `simpleclans.anyone.roster`        | Может посмотреть список участников кланов                      |
| `simpleclans.anyone.invite-toggle` | Может переключать возможность быть приглашённым в другие кланы |

### Разрешения участника

| Право                                           | Описание                                                      |
| ----------------------------------------------- | ------------------------------------------------------------- |
| `simpleclans.member.abstain`                    | Может воздержаться от участия                                 |
| `simpleclans.member.accept`                     | Может принять запрос                                          |
| `simpleclans.member.ally`                       | Может использовать союзный чат                                |
| `simpleclans.member.chat`                       | Может использовать чат клана                                  |
| `simpleclans.member.bank`                       | Может использовать банк клана                                 |
| `simpleclans.member.bb-add`                     | Может добавлять сообщения на доску объявлений                 |
| `simpleclans.member.bb-toggle`                  | Может переключать отображение доски объявлений его клана      |
| `simpleclans.member.bb`                         | Может видеть доску объявлений его клана                       |
| `simpleclans.member.can-join`                   | Может присоединяться к кланам                                 |
| `simpleclans.member.coords`                     | Может посмотреть координаты его клана                         |
| `simpleclans.member.deny`                       | Может отклонить запрос                                        |
| `simpleclans.member.ff`                         | Может переключать собственный "огонь по своим"                |
| `simpleclans.member.home`                       | Может телепортироваться на точку базы клана                   |
| `simpleclans.member.kills`                      | Может посмотреть убийства свои и других                       |
| `simpleclans.member.lookup`                     | Может посмотреть информацию о себе                            |
| `simpleclans.member.profile`                    | Может посмотреть информацию о своём клане                     |
| `simpleclans.member.resign`                     | Может покинуть свой клан                                      |
| `simpleclans.member.roster`                     | Может посмотреть список участников его клана                  |
| `simpleclans.member.stats`                      | Может посмотреть статистику его клана                         |
| `simpleclans.member.vitals`                     | Может посмотреть боеспособность его клана                     |
| `simpleclans.member.toggle.bb`                  | Может переключать видимость доски объявлений при входе в игру |
| `simpleclans.member.tag-toggle`                 | Может скрыть или показать клан тег                            |
| `simpleclans.member.fee-check`                  | Позволяет проверить включена ли комиссия и узнать её размер   |
| `simpleclans.member.bypass-fee`                 | Может обойти комиссию участника                               |
| `simpleclans.member.land`                       | Может использовать команду land                               |
| `simpleclans.member.land.allow.container`       | Может разрешить действие container                            |
| `simpleclans.member.land.allow.place`           | Может разрешить действие place                                |
| `simpleclans.member.land.allow.break`           | Может разрешить действие break                                |
| `simpleclans.member.land.allow.damage`          | Может разрешить действие damage                               |
| `simpleclans.member.land.allow.interact`        | Может разрешить действие interact                             |
| `simpleclans.member.land.allow.interact_entity` | Может разрешить действие interact\_entity                     |
| `simpleclans.member.land.block.container`       | Может заблокировать действие container                        |
| `simpleclans.member.land.block.place`           | Может заблокировать действие place                            |
| `simpleclans.member.land.block.damage`          | Может заблокировать действие damage                           |
| `simpleclans.member.land.block.break`           | Может заблокировать действие break                            |
| `simpleclans.member.land.block.interact`        | Может заблокировать действие interact                         |
| `simpleclans.member.land.block.interact_entity` | Может заблокировать действие interact\_entity                 |

### Разрешения лидеров

| Право                                           | Описание                                                                |
| ----------------------------------------------- | ----------------------------------------------------------------------- |
| `simpleclans.leader.fee`                        | Разрешает переключать комиссию клана и изменять её размер               |
| `simpleclans.leader.ally`                       | Может иметь союз с другим кланом                                        |
| `simpleclans.leader.create`                     | Может создавать кланы                                                   |
| `simpleclans.leader.verify`                     | Может подать заявку на подтверждение собственного клана                 |
| `simpleclans.leader.demote`                     | Может понизить лидера до участника                                      |
| `simpleclans.leader.disband`                    | Может расформировать собственный клан                                   |
| `simpleclans.leader.ff`                         | Может переключать "огонь по своим" у собственного клана                 |
| `simpleclans.leader.home-set`                   | Может установить точку базы клана                                       |
| `simpleclans.leader.regroup.me`                 | Может перегруппировать (телепортировать ) весь клан к себе              |
| `simpleclans.leader.regroup.home`               | Может перегруппировать (телепортировать ) весь клан на точку базы клана |
| `simpleclans.leader.invite`                     | Может приглашать игроков в собственный клан                             |
| `simpleclans.leader.kick`                       | Может выгнать (кикнуть) игроков с собственного клана                    |
| `simpleclans.leader.modtag`                     | Может изменять тег собственного клана                                   |
| `simpleclans.leader.description`                | Может изменять описание собственного клана                              |
| `simpleclans.leader.coloredtag`                 | Может использовать цветовые коды в тегах                                |
| `simpleclans.leader.coloredrank`                | Может использовать цветовые коды в отобр. имени ранга                   |
| `simpleclans.leader.promotable`                 | Может быть повышен до лидера клана                                      |
| `simpleclans.leader.promote`                    | Может повысить участника до лидера клана                                |
| `simpleclans.leader.rank.assign`                | Может назначить участнику ранг                                          |
| `simpleclans.leader.rank.unassign`              | Может забрать ранг у участника                                          |
| `simpleclans.leader.rank.create`                | Может создать новый ранг                                                |
| `simpleclans.leader.rank.delete`                | Может удалить существующий ранг                                         |
| `simpleclans.leader.rank.list`                  | Может посмотреть список рангов                                          |
| `simpleclans.leader.rank.setdisplayname`        | Может устанавливать отобр. имя ранга                                    |
| `simpleclans.leader.rank.permissions.add`       | Может добавить право к рангу                                            |
| `simpleclans.leader.rank.permissions.available` | Может посмотреть список доступных прав рангов                           |
| `simpleclans.leader.rank.permissions.list`      | Может посмотреть список прав рангов                                     |
| `simpleclans.leader.rank.permissions.remove`    | Может удалить права у ранга                                             |
| `simpleclans.leader.rival`                      | Может начать вражду с другими кланами                                   |
| `simpleclans.leader.settrust`                   | Может устанавливать уровень доверия участникам                          |
| `simpleclans.leader.war`                        | Может начать войну                                                      |
| `simpleclans.leader.setbanner`                  | Может устанавливать баннер собственного клана                           |
| `simpleclans.leader.withdraw-toggle`            | Может переключать вывод клана                                           |
| `simpleclans.leader.deposit-toggle`             | Может переключать взнос клана                                           |
| `simpleclans.leader.bb-clear`                   | Может очистить доску объявлений собственного клана                      |

### Разрешения модераторов

| Право                        | Описание                                                                                                                                                       |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `simpleclans.mod.ban`        | Может заблокировать игрока от использования команд плагина                                                                                                     |
| `simpleclans.mod.bypass`     | Может обойти любые ограничения                                                                                                                                 |
| `simpleclans.mod.disband`    | Может расформировать любой клан                                                                                                                                |
| `simpleclans.mod.globalff`   | Может выключить глобальный параметр "огонь по своим"                                                                                                           |
| `simpleclans.mod.home`       | Может ставить точку базы любому клану                                                                                                                          |
| `simpleclans.mod.hometp`     | Может телепортироваться на точку базы любого клана                                                                                                             |
| `simpleclans.mod.staffgui`   | Может открыть меню администратора                                                                                                                              |
| `simpleclans.mod.place`      | Может перемещать вручную игроков из одного клана в другой                                                                                                      |
| `simpleclans.mod.keep-items` | При перемещении на точку дома **не** выбрасывает вещи из [drop-items](https://simpleclans.gitbook.io/simpleclans/how-to-setup/configuration#general-settings). |
| `simpleclans.mod.mostkilled` | Может посмотреть список наибольших убийств у любого клана                                                                                                      |
| `simpleclans.mod.nopvpinwar` | Может обойти PvP разрешение в войнах                                                                                                                           |
| `simpleclans.mod.unban`      | Может разблокировать игрока от использования команд плагина                                                                                                    |
| `simpleclans.mod.verify`     | Может подтвердить клан                                                                                                                                         |

### Разрешешения администраторов

| Право                              | Описание                                  |
| ---------------------------------- | ----------------------------------------- |
| `simpleclans.admin.resetkdr`       | Может очистить KDR любого игрока          |
| `simpleclans.admin.purge`          | Может очистить данные об игроке           |
| `simpleclans.admin.demote`         | Может понизить игрока до участника        |
| `simpleclans.admin.promote`        | Может повышать игроков до лидера          |
| `simpleclans.admin.all-seeing-eye` | Может читать чаты всех кланов             |
| `simpleclans.admin.reload`         | Может перезагрузить конфигурацию          |
| `simpleclans.admin.permanent`      | Позволяет переключить перманентный статус |
| `simpleclans.admin.bank.status`    | Позволяет проверить баланс клана          |
| `simpleclans.admin.bank.take`      | Позволяет забрать деньги из баланса клана |
| `simpleclans.admin.bank.give`      | Позволяет выдать деньги в баланс клана    |
| `simpleclans.admin.bank.set`       | Позволяет установить баланс клана         |

### Другие разрешения

| Право                          | Описание                                                                      |
| ------------------------------ | ----------------------------------------------------------------------------- |
| `simpleclans.other.kdr-exempt` | KDR игрока не будет изменяться из-за смерти/убийства (см. известные проблемы) |
| `simpleclans.vip.resetkdr`     | Может очистить собственный KDR                                                |
