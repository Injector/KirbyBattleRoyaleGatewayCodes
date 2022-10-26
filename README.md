### Kirby: Battle Royale - Gateway codes

**[ENGLISH](https://github.com/Injector/KirbyBattleRoyaleGatewayCodes/blob/main/README_ENGLISH.md)**

V 1.0
Последнее обновление 27.10.2022

Мой первый опыт в создании Gateway кодов, все они протестированы в Citra Nightly билд 1797 и Citra на андроиде.
Эти коды должны работать и на Nintendo 3Ds.
Gateway коды созданы с помощью Cheat Engine Debugger (find out what writes to this address) и встроенный в андроид версии Memory Viewer от weihuoya.

Я начал данный проект что-бы разблокировать возможность играть за Рыцаря Топора, но затем решил делать коды которые затрагивают что-то другое.

## Заметки

По поводу с кодами "Играть за", они изменяют Вашу способность и других игроков в самой битве, не в меню.
Коды в Одиночной игре работают и в мультиплеерной, но **На стороне клиента**, это означает другие игроки не увидят вашу новую способность (наверное однажды я сделаю мультиплеерный код)
Они так-же могут десинхронизировать действия других игроков в мультиплеере. Так что не используйте их в мультиплеере.

Если у вас нету желаемой способности, перезапустите битву 1-3 раза, пока она не появится. Если все еще не появилось, перезапустите игру.

Избегайте использования кодов "Играть за" в одиночной и в тренировочном. Иначе они могут конфликтовать с другими кодами, и сломать игру.

Где ``YYYYYYYY``, вставьте ID из списка, смотрите в Список Ability ID и Список Color ID

## Играть за (Одиночная, не стори мод)

Этот код изменяет вашу способность в битве. Вы можете использовать его чтобы играть за неигровых персонажей (Б. У. Ди, Солдат Уоддл Ди, Рыцарь Топора)

```
D3000000 30000000
2062E298 YYYYYYYY
2062E2B4 YYYYYYYY
2062EEA4 YYYYYYYY
2062E2AC YYYYYYYY
D2000000 00000000
```

# Играть за (Cake Royale Стори мод)

```
D3000000 30000000
216E78C4 YYYYYYYY
D2000000 00000000
```

# Игрок 2 играет за (Одиночная)

```
D3000000 30000000
2062E334 YYYYYYYY
D2000000 00000000
```

# Игрок 3 играет за (Одиночная)

```
D3000000 30000000
2056E6D0 YYYYYYYY
2062E3D0 YYYYYYYY
D2000000 00000000
```

# Игрок 4 играет за (Одиночная)

```
D3000000 30000000
2062E46C YYYYYYYY
D2000000 00000000
```

# Играть в тренировочном (Одиночная, из меню)

```
D3000000 30000000
22204C50 YYYYYYYY
D2000000 00000000
```

# Установить цвет (Одиночная)

Используйте ID из Список Color ID

```
D3000000 30000000
2062E5EC YYYYYYYY
D2000000 00000000
```

## Играть за (Одиночная, альтернативный код)

```
D3000000 30000000
216E7880 YYYYYYYY
216E7920 YYYYYYYY
216E791C YYYYYYYY
D2000000 00000000
```

## Список Ability ID

| Способность | ID | Имя| Базированно на |
| ------ | ------ | ------ | ----- |
| Sword | ``00000000`` | Меч | |
| Bomb | ``00000001`` | Бомба | |
| Tornado | ``00000002`` | Торнадо  | |
| Ninja | ``00000003`` | Ниндзя | |
| Beetle | ``00000004`` | Жук | |
| Parasol | ``00000005`` | Зонтик | |
| Hammer | ``00000006`` | Кувалда | |
| Cutter | ``00000007`` | Клинок | |
| Doctor | ``00000008`` | Доктор | |
| Spear | ``00000009`` | Копье | |
| Ice | ``0000000A`` | Лёд | |
| Fighter | ``0000000B`` | Боец | |
| Whip | ``0000000C`` | Кнут | |
| WaddledeeParasol | ``0000000D`` | Уоддл Ди с Зонтиком | |
| Metaknight | ``0000000E`` | Мета Рыцарь | |
| Dedede | ``0000000F`` | Король Дидиди | |
| Mirror | ``00000010`` | Отражение | |
| Sleep | ``00000011`` | Сонливый | |
| WaddledeeBuddy | ``00000012`` | Уоддл Ди в Бандане | Уоддл Ди с Зонтиком |
| WaddledeeSpear | ``00000013`` | Солдат Уоддл Ди | Копье |
| AxeKnight | ``00000014`` | Рыцарь Топора | Клинок |

Вы можете посмотреть эти способности в ``mint/Default.bin.cmp`` класс ``Scn.Game.Hero.AbilityKind``

## Список Color ID

| Цвет | ID |
| ------ | ------ |
| Pink | ``00000000`` |
| Yellow | ``00000001`` |
| Green | ``00000002`` |
| Blue | ``00000003`` |
| Gray | ``00000004`` |
| Orange | ``00000005`` |

Вы можете посмотреть эти цвета в ``mint/Default.bin.cmp`` класс ``Scn.Game.Hero.ColorKind``