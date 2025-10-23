# Map-maker
This is the public repository for an app to make maps for the team game mod. Working Exe file is downloadable. (this is vibe coded and ugly code, but it works) Wiki is in english, russian and chinese. Вики доступна на английском, русском и китайском языках. 维基提供英语、俄语和中文版本。

Download at : https://github.com/Jedfy/Map-maker/releases/tag/v1.0.0

# Wiki

## Add System
Click Add System, then left-click on the canvas to place a star.
A yellow dot appears; label shows the primary attribute once set.

## Modify System Coordinates
Click Modify System Coordinates → left-click a system → enter new X, Y.

## Build Hyperlane
Click Build Hyperlane → left-click first system, then second.
Regular is a normal hyperlane, midgame is a hyperlane that will appear at midgame (y30) and endgame is a hyperlane that will appear at endgame (y45)

## Build Wormhole
Click Build Hyperlane → left-click first system, then second.
Regular, midgame and endgame works the same.

## Add / Delete Attributes
Add Attributs → click a system → choose an index from systems_initializers.xlsx.
The first attribute in the set is the displayed label and the one used on export.
Delete Attributs → click a system to clear its attributes.

## Back / Cancel Back
Back: Undoes the last action (ctrl-z equivalent)
Cancel Back: Undoes the last undo (ctrl-y equivalent)

## Save Data / Load Data
Save Data: writes a .txt to save your project.
Load Data: reloads a saved project and redraws the galaxy.

## Symetry
Mirrors selected systems and their hyperlanes.
Options: horizontal (mirror Y), vertical (mirror X), center (180°).

## Copy-Paste
Duplicates selected systems/lines by an offset (dx, dy) you enter.

## Circular Symetry
Mirrors selected systems and their hyperlanes, but following a revolution pattern. You can either pick :
total angle + times : total angle of revolution and the amount of times your pattern appears (including the selected systems)
step angle + copy : you pick the angle between the copies, and the amount of copies.
You can also change the center of the symetry, this is for people wanting to do multiple clusters in different parts of galaxy separatly.

## Export Galaxy
Writes a complete static_galaxy_scenario file, given your current galaxy
It will export the galaxy for team game mod format. 
Put this galaxy file in : map\setup_scenarios
The settings are :
#### team format : 
xvxvx or xvyvz here (1v1, 8v8, 2v2, 4v4v4 or 3v4v5)
#### team layout : 
this is to automatically separate spawns so that spawn 1 is at the top left corner of galaxy for example. If doesn't work properly, tweak the generated capital_system_initializer_1 into capital_system_initializer_2 or else to fix which spawn is which. But it works most of the time.
#### how many teams :
select the amount of teams on the map. if it's a 1v1 map, select the 1v1 special mode. if it's 3v3, select 2 teams. 3v3v3 3 teams, 2v4v6v7 4 teams, 2v2v2v2v2 5 teams, etc.
The mod supports up to 20 players on 10 different teams.

## Delete
Removes selected systems and hyperlanes

## About solar systems initializers
You need the systems_initializers.xlsx file in the same folder for the solar systems initializers to work properly. You can add a vanilla one in the excel file, or even make your own solar system initializers. (they are in common\solar_system_initializers). If the initializer does not exist, an error will appear on the error.log and the system will instead be a random vanilla one.
Also, there can only be 2 garantees for a player at the moment, and they can be at max 2 jumps away from the capital.

# Вики

## Добавить систему
Нажмите Add System, затем щёлкните на холсте, чтобы поставить звезду. Появится жёлтая точка; подпись покажет основной атрибут после назначения.

## Изменить координаты системы
Нажмите Modify System Coordinates → щёлкните систему → введите новые X, Y.

## Построить гиперлинию
Нажмите Build Hyperlane → щёлкните первую систему, затем вторую.
Regular — обычная гиперлиния; midgame появляется к середине партии (y30); endgame появляется в поздней игре (y45).

## Построить червоточину
Нажмите Build Hyperlane → щёлкните первую систему, затем вторую.
Режимы regular, midgame и endgame работают так же.

## Добавить / удалить атрибуты
Add Attributs → щёлкните систему → выберите индекс из systems_initializers.xlsx.
Первый атрибут используется как подпись и при экспорте.
Delete Attributs → щёлкните систему, чтобы очистить атрибуты.

## Отменить / Повторить
Back: откат последнего действия (Ctrl+Z).
Cancel Back: откат отката (Ctrl+Y).

## Сохранить данные / Загрузить данные
Save Data: записывает .txt проекта.
Load Data: загружает сохранённый проект и перерисовывает галактику.

## Симметрия
Зеркалирует выбранные системы и гиперлинии.
Варианты: horizontal (ось Y), vertical (ось X), center (180°).

## Копировать-Вставить
Дублирует выбранные системы/линии со сдвигом (dx, dy).

## Круговая симметрия
Копирует выбранное по окружности.
— total angle + times: общий угол и число повторов (включая исходник).
— step angle + copy: шаг между копиями и количество копий.
Можно менять центр симметрии для отдельных кластеров.

## Экспорт галактики
Пишет static_galaxy_scenario по текущей карте.
Файл поместите в map\setup_scenarios.
Настройки:
#### team format:
xvxvx или xvyvz (напр. 1v1, 8v8, 2v2, 4v4v4, 3v4v5)
#### team layout:
Авто-развод спавнов; при необходимости замените capital_system_initializer_1 на _2 и т. д.
#### how many teams:
Выберите число команд. 1v1 — спецрежим 1v1; 3v3 — 2 команды; 3v3v3 — 3; 2v4v6v7 — 4; 2v2v2v2v2 — 5 и т. д.
Поддерживается до 20 игроков в 10 командах.

## Удалить
Удаляет выбранные системы и гиперлинии.

## Об инициализаторах звёздных систем
Нужен systems_initializers.xlsx в той же папке. Можно использовать ванильные или свои (common\solar_system_initializers).
Если инициализатор не найден, запись появится в error.log, а система станет случайной ванильной.
Сейчас поддерживаются максимум две «гарантии» для игрока, не дальше чем в двух прыжках от столицы.

# 维基

## 添加星系
点击【添加星系】，在画布上左键放置恒星。出现黄色圆点；设置属性后标签显示主要属性。

## 修改坐标
点击【修改坐标】→ 左键选中星系 → 输入新的 X、Y。

## 创建超空间航道
点击【创建超空间航道】→ 依次左键选择两个星系。  
为普通航道；在中期出现（y30）； 在后期出现（y45）。

## 创建虫洞
点击【创建虫洞】→ 依次左键选择两个星系。  
为普通航道、在中期出现、在后期出现 与航道一致。

## 添加属性 / 删除属性
点击【添加属性】→ 选星系 → 在 systems_initializers.xlsx 中选择索引。集合中的第一个属性用于标签与导出。  
点击【删除属性】→ 清空该星系属性。

## 撤销 / 重做
【撤销】：回退上一步（Ctrl+Z）。  
【重做】：撤销上一次回退（Ctrl+Y）。

## 保存数据 / 加载数据
【保存数据】：写出项目 .txt。  
【加载数据】：读取项目并重绘星系。

## 对称
点击【对称】→ 右键框选 → 选择 水平（Y 轴）、垂直（X 轴）、中心（180°）。仅在新镜像点之间生成连线。

## 复制-粘贴
点击【复制-粘贴】→ 右键框选 → 输入 (dx, dy) 复制所选星系与连线。

## 旋转对称
点击【旋转对称】→ 右键框选 → 选择：
- 总转角 + 重复次数：总转角与重复次数（含原图）。
- 角度步长 + 副本数：副本间角度与副本数量。  
可设置对称中心以在不同区域单独构建簇。

## 导出星系
点击【导出星系】→ 生成 static_galaxy_scenario（团队对战格式），放入 map\setup_scenarios。  
队伍格式：xvxvx 或 xvyvz（例 1v1、8v8、2v2、4v4v4、3v4v5）。  
队伍布局：自动分配刷新点；不理想时在导出文件中把 capital_system_initializer_1 改为 _2 等。  
队伍数量：按地图选择队伍数；最多 10 支队伍 / 20 名玩家。

## 删除
点击【删除】→ 移除所选星系与航道。

## 关于恒星系初始化
需要同目录 systems_initializers.xlsx；可用原版或自定义（common\solar_system_initializers）。不存在的初始化器会记入 error.log，系统回退为随机原版。玩家最多 2 项保障，距首都 ≤ 2 跳。
