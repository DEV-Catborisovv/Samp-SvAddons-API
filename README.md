Функция	                                    Описание	                                                                  Returns

SetPlayerSpecialAction(playerid, actionid)	Устанавливает специальные действия.
Если специальные действия USECELLPHONE или STOPUSECELLPHONE, то обьект телефона будет автоманически при аттачен к персонажу.	1
IsPlayerInWater(playerid)или
IsPlayerSwimming(playerid)	Проверка на то - плавает ли игрок.	1 если игрок плавает, иначе 0.
SetPlayerPosEx(playerid, Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0, Float: angle = 0.0)	Устанавливает позицию игрока, виртуальный мир, интерьер, и угол	1
GetPlayersName(playerid)	получает имя игрока	имя игрока
GetPlayersNameEx(playerid)	получает имя игрока без подчеркивания	им игрока без подчеркивания
CrashPlayer(playerid)	краш игрока	1
GetPlayersIP(playerid)	получает ip игрока	Ip игрока
ExplodePlayer(playerid)	взрывает игрока	1
ExplodeVehicle(vehicleid)	взрывает авто	1
SetPlayerMoney(playerid, amount)	устанавливает игроку деньги.	1
GivePlayerJetpack(playerid)	дает игроку JetPack	1
IsPlayerSpawned(playerid)	заспавнен игрок или нет.	если заспавнен то 1 а если нет - 0
GetVehicleInfo(vehicleid, infoType)	получает информацию о статусе одного из параметра авто (для инфо-типа можно использовать VEHICLE_INFO_PARAMNAME)	состояние транспортногосредства
SetVehicleInfo(vehicleid, infoType, value)	Устанавливает значение одного из параметров авто	1
IsPlayerInVehicleFireMode(playerid)	проверка: является ли игрок пассажиром	1 если в качевстве пассажира, 0 в другом случае.
GetVehicleDriver(vehicleid)	получает ID водителя определенного авто	Id водителя
GetVehicleNumberPlate(vehicleid)	получает номерное знак авто	номерной знак
IsPlayerSpectating(playerid)	проверка на то, является ли игрок зрителем или нет	1 если является, 2 если нет.
GetPlayerObjectEditingState(playerid)	получает статус игрока редактирующего обьект	игрок в редактировании обьекта
RemovePlayerWeapon(playerid, weaponid)	удаляет оружие у игрока	1
ClosePlayerDialog(playerid)	закрывает диалоговое окно у игрока	1
SetPlayerDeathEffect(playerid, deffid)	устанавливает эффект смерти игрока(DEATH_EFFECT_NONE,
REDGAS,SMOKE,EXPLODE,
MINIEXPLODE,FIRE)	1
GetPlayerDeathEffect(playerid)	получает эффект смерти игрока.	эффект смерти игрока.
DisableSprunkMachines()	используется в OnGameMode init
удаляя все Sprunk аппараты с карты.	1
ChangeServerPassword(password[])	изменить пароль сервера	1
LoadFilterscript(scriptName[], bool: reload = false)	загрузка фильтр скрипта	1
UnloadFilterscript(scriptName[])	выгрузка фильтр скрипта	1
ChangeServerName(serverName[])	изменить имя сервера	1
SendServerRCONMessage(message[])	отправляет сообщение от RCON	1
ChangeServerWebsite(url[])	сменить ссылку в клиенте samp	1
ChangeMapName(mName[])	сменяет название карты, тоже в клиента	1
IsValidSkin(skinID)	проверка на скин игрока	1 если скин игрока(skinID), 2 если другой
ClearPlayersChat(playerid, bool: includeScrollingChat = false)	отчитска чата	1
TeleportPlayerToPlayer(playerid, giveplayerid, Float: offsetX = 1.0, Float: offsetY = 0.0, Float: offsetZ = 0.0)	телепорт игрока к другому игроку.	1
ClearAllPlayersChat(bool: includeScrollingChat = false)	отчистить чат у всех игроков.	1
StopVehicleMovement(vehicleid)	плавно останавливает движение автомобиля	1
GetVehicleSpeed(vehicleid)	получает скорость авто	скорость авто
GetVehicleModelName(modelID)	получает ID модели авто	ид модели авто
GetVehicleIDFromName(string[], bool: useFind = false)	получает ID машины от имени.	модель авто ID
GetWeaponID(weaponName[], bool: ignoreCase = true, bool: useFind = false)	Возвращает ид оружие от имени	ид оружия
GetPlayerIDFromIP(ip[], bool: useFind = false)	узнает ид игрока по его IP	ид игрока
CountTotalPlayers()	получает кол-во подключенных игроков	кол-во подключенных игроков
CountTotalRCONAdmins()	получает кол-во подключенных RCON админов	кол-во ркон админов
CountTotalNPCs()	получает общее кол-во подключенных ботов	кол-во ботов
CountTotalPausedPlayers()	получает кол-во игроков в афк	кол-во афкшников
GetVehiclesAngle(vehicleid)	получает угол поворота авто	угол поворота авто
GetVehiclesHealth(vehicleid)	возвращает хп авто	хп авто
GetPlayersHealth(playerid)	получает хп игрока	хп игрока
GetPlayersArmour(playerid)	получает хп брони игрока	хп брони
EnableWhitelist(mode = WHITELIST_MODE_ALLOWPLAYER, ip[] = " ")	включает вайт лист для RCON админов с несколькими режимами(WHITELIST_MODE_NONE,
ALLOWPLAYER,SPECIFICIP,IP_FIND)	1
GetWhitelistMode()	узнает вайтлист режим	режим вайт листа
AddPlayerToWhitelist(playerid)	добавляет игрока в вайт лист RCON	1
IsPlayerWhitelisted(playerid)	проверка, в RCON вайтлисте ли игрок	1, если игрок в вайт листе, 2 если нет
ShakePlayerScreen(playerid, duration = 1250)	заставляет экран игрока вибрировать(как при землетресении - duration - сила вибрации)	1
ReconnectPlayer(playerid)	повторное подключение игрока к серверу, не закрывая экран	1
GetVehicleInterior(vehicleid)	получает интерьер авто	интерьер авто
IsPlayerBehindVehicle(playerid, vehicleid)	проверка: находится ли игрок позади авто	1 если находится, 2 если нет
GetVehicleTrailerCount(vehicleid)	получает кол-во прицепов к авто	кол-во прицепов
GetFreeVehicleSeat(vehicleid)	получает следующее свободное место в авто	свободное место в авто
GetVehicleSpawnInfo(vehicleid, &Float: spawnX, &Float: spawnY, &Float: spawnZ, &Float: spawnR, &color1, &color2, &respawndelay)	получает сведения о спавне авто	если сиденье доступно получаем его ид в противном случае INVALID_VEHICLE_ID
CapitalizePlayerName(playerid)	прописное имя игрока(в том числе после подчеркивания)	1
GetPlayerTemporaryName(playerid)	получает временное имя игрока	временное имя игрока
GetStringCharacterCount(string[], character)	возвращает кол-во символов указанных в строке	кол-во символов
SetVehiclePosEx(vehicleid, Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0, Float: angle = 0.0)	устанавливает координаты авто вместе с интерьером и виртуальным миром	1
SendNearbyClientMessage(color, message[], Float: distance = 30.0, Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0)	посылает сообщение в чат всем кто рядом с указанной точкой	1
GameTextForNearbyPlayers(text[], time, style, Float: distance = 30.0, Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0)	посылает игровой текст на экране для игроков рядом с указанной точкой	1
ToggleNearbyPlayersControllable(bool: controllable, Float: distance = 30.0, Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0)	изменяет погоду игроков рядом с указанной точкой	1
TogglePlayerKickImmunity(playerid, bool: immune)	сам особо не понял, но вроде: запрещает кикать игрока	1
GetPlayerKickImmunity(playerid)	получает иммунитет от ударов игрока	иммунитет к кику
TogglePlayerBanImmunity(playerid, bool: immune)	запрещает игрока банить	1
GetPlayerBanImmunity(playerid)	получает иммунитет игрока к бану	имменитет к бану
CreateTriggerPoint(Float: posX, Float: posY, Float: posZ, interior = 0, virtualworld = 0)	устанавливает невидимый тригер ( что то типа пикапа, но невидимый)
функция при том когда игрок в триггере(в пабликеOnPlayerTouchTrigger)	ид тригера
StartCountdown(from = 3)	начинается обратный отсчет для всех	ид таймера
SendClientAudioMessage(playerid, message[], bool: withClientMessage = false, color = -1, language[] = "en")	отправляет игроку сообщение через аудио поток гугл транслейта	1
DealPlayerDamage(playerid, damage)	наносит игроку урон без всяких GetPlayerHealh.	1
CountTotalVehicles()	получает кол-во созданных авто	кол-во созданных авто
IsVehicleOccupied(vehicleid)	проверка если транспортное средство занято	0 если не занято, в другом случае 1

IsPlayerDrivingVehicle(playerid,vehicleid = INVALID_VEHICLE_ID)	проверка:водитель ли авто	0 если нет 1 если да
TeleportPlayerToVehicle(playerid, vehicleid, Float: offsetX = 1.0, Float: offsetY = 0.0, Float: offsetZ = 0.0)	телепортирует игрока на транспортном средстве	1
GetPickupPos(pickupid, &Float: X, &Float: Y, &Float: Z)	узнать позицию пикапа	1
GetPickupVirtualWorld(pickupid)	узнать вирт.мир пикапа	1
HideAllTextDraws()	скрывает все текстдравы для игроков	1
HideAllTextDrawsForPlayer(playerid)	скрывает все текстдравы для указ.игрока	1
GetSkinGender(skinid)	узнать пол скина	пол скина(женский-или мужской)
TogglePlayerWeaponSwitch(playerid, bool: togws)	может ли игрок переключить оружие или нет	1
IsMeleeWeapon(weaponid)	проверяет, является ли указанное оружие для ближнего боя	1, если оружие является оружием ближнего боя, иначе 0
IsPlayerPaused(playerid) или IsPlayerTabbed(playerid)	проверка, в афк ли игрок или нет	1 если игрок афк, 0 если нет
GetPlayerControllable(playerid)	узнать, может ли игрок управлять персонажем	1 если может, 0 если нет
divideRem(a, b, &answer, &remainder)	деление 2ух чисел с остатком	1
CountTotalObjects()	общее число созданых обьектов	число обьектов
GetServerStats(&connections, &kicks, &vehicles, &objects, &players, &totalvehicles, &totalobjects, &kills, &deaths, &totaldamage, mode = SERVER_STATS_UPTIME, bool: errorContinue = true)	получает статистику сервера

Колбек	                     Вызов
OnVehicleCreate(vehicleid)	создается когда автомобиль создан
(не заспавнен)
OnPlayerPausedUpdate(playerid, bool: paused)	вызывается когда игрок в афк
или вых него
OnPlayerWeaponUpdate(playerid, newgun, oldgun)	вызывается когда игрок меняет оружие.
OnReceiveClientMessage(playerid, color, message[])	Вызывается когда игрок получает сообщение
клиента(включает в себя аудио потока сообщений
и не включает SendClientMessageToAll
OnRconLoginBlocked(playerid, ip[], password[], success)	вызывается когда игрок блокируется
RCON вайт листом
OnPlayerWaterStatusUpdate(playerid, bool: inWater)	вызывается когда игрок входит и выходит из воды
OnPlayerSpecialActionChange(playerid, oldaction, newaction)	вызывается когда игрок меняет специальные действия
(пока-что не работают sprunk и сигары)
OnPlayerTouchTrigger(playerid, triggerid)	вызывается когда игрок касается триггера

Максимальные значения

MAX_INTEGER_LENGTH	12
MAX_IP_LENGTH	17
MAX_WEAPON_NAME	24
MAX_CLIENT_MESSAGE	128
MAX_WEAPON_AMMO	32767
MAX_INTEGER_VALUE	2147483647

Определение	Размер
S_IP[имя переменной]	17
S_Player[имя переменной]	MAX_PLAYER_NAME или 24
S_Weapon[имя переменной]	S_Weapon[variable name]
S_Chat[имя переменной]	MAX_CLIENT_MESSAGE (пользовательское определение) или 128
