Тема созданна на [Endless backrooms in Babylon.js! - Demos and projects - Babylon.js](https://forum.babylonjs.com/t/endless-backrooms-in-babylon-js/55544/45) но потом мой аккаунт удалили, и теперь пришлось писать всё здесь.

# Предисловие 

Сколько было попыток создать бэкрумс, и хочу отметить что до сих пор так никому, и не удалось полноценно реализовать идею бэкрумса! Ведь что такое бэкрумс!? Бэкрумс это в первую очередь идея бесконеченого лабиринта куда что-то, или кто-то случайно выпадает из реальности, и попадая в этот бесконечный лабиринт оно пытается там выжить и выбраться оттуда, и вся суть в том что чем больше от туда кто-то пытаются выбраться тем больше  становиться тех кто туда случайно выпадает из реальности, и при каждой последующей итерации того как кто-то оттуда выбирается это место становиться все более сломанным, и тем больше выбраться оттуда становиться всё более сложнее, и в конечном итоге окажется так что весь мир, а то и вся вселенная навечно провалится в бэкрумс, и все будут бесконечно блуждать в бесконечном лабиринте бесконечно долго пока вся эта бесконечность не придет к какому-то общему знаменателю но к какому!?

# Версия ПК 

Я создал бэкрумс на движке babylon перемещаться с помощью стрелок ←, →, ↑, ↓ на клавиатуре и мыши.

## Оригинальный бэкрумс 

В нулевой версии я добавил бесконечный процедурно генерируемый ковер.

[Backrooms in Babylon.js (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#BM5M6A)

В первой версии я добавил случайно сгенерированные, и случайно повернутые стены на этом процедурно сгенерированном ковре.

[Backrooms in Babylon.js (Version 1) | Babylon.js Playground](https://playground.babylonjs.com/#VBRJ0Y)

Во второй версии я добавил бесконечный процедурно генерируемые потолок.

[Backrooms in Babylon.js (Version 2) | Babylon.js Playground](https://playground.babylonjs.com/#NGAD7L)

В третьей версии я добавил бесконечно генерируемые процедурно равномерно расположенные лампы.

[Backrooms in Babylon.js (Version 3) | Babylon.js Playground](https://playground.babylonjs.com/#1XXCMX#1)

В четвертой версии я сделал так что-бы лампы генерировались с вероятность 50 процентов, и так же добавил поля телепорта.

[Backrooms in Babylon.js (Version 4) | Babylon.js Playground](https://playground.babylonjs.com/#HUS6UR#2)

В пятой версии я сделал генерацию стен по лабиринту ведь бэкрумс это не случайно расположенные стены в случайных местах а бесконечный лабиринт. 

[Backrooms in Babylon.js (Version 5) | Babylon.js Playground](https://playground.babylonjs.com/#XNSPM5#2)

В шестой версии я сделал бесконечную процедурную генерацию стен по картинкам, и там где есть чёрное на картинке там стены а там где белое там не генируются стены.

[Backrooms in Babylon.js (Version 6) | Babylon.js Playground](https://playground.babylonjs.com/#Q926I8#0)

В седьмой версии я сделал маркер там где есть определённая картинка на бесконечном ковре из картинок то там генерируется стена в ином случае нет.

[Backrooms in Babylon.js (Version 7) | Babylon.js Playground](https://playground.babylonjs.com/#74JVEN#0)

## Версия Кейна Пикселя

В первой версии я добавил возможность генерации структуры на основе граней и массивов вершин. Вам просто нужно немного отклониться в сторону, чтобы увидеть генерацию.

[Kane Pixel’s Backrooms in Babylon.js (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#CBZ7JF)

Во второй версии я добавил разные биомы, и теперь генерируется не один биом, а много.

[Kane Pixel’s Backrooms in Babylon.js (Version 1 - multybiom generation) | Babylon.js Playground](https://playground.babylonjs.com/#RSODNR)

Но чего-то все еще не хватает, потому что подсобные помещения Kane Pixel представляют собой бесконечный многоуровневый пирог из случайно сгенерированных процедурно взаимосвязанных пространств.

[Kane Pixel’s Backrooms in Babylon.js (Version 2 - Multistory multibiome generation) | Babylon.js Playground](https://playground.babylonjs.com/#AWLGMD)

Теперь нужно сделать разные текстуры для стены, пол, и потолка каждого биома.

[Kane Pixel’s Backrooms in Babylon.js (Version 3 - Different textures) | Babylon.js Playground](https://playground.babylonjs.com/#9ZJ0XW#0)

Теперь нужно задать сид для определенной заранее заданной случайно генерацией мира которая бы как в майнкрафте выдовала при вводе этого сида всегда выдовала бы одни, и те же биомы коридоров, и комнат.

[Kanе Pixel’s Backrooms in Babylon.js (Version 4 - Seed of the world) | Babylon.js Playground](http://playground.babylonjs.com/#5R1MLK#1)

# Мобильная версия

## Оригинальная мобильная версия бэкрумс

Но, просматривая свои подсобные помещения со смартфона, я обнаружил проблему, заключающуюся в том, что я не могу перемещаться по своему телефону, и поэтому в мобильную версию подсобных помещений я добавил стрелки с помощью которых я могу перемещаться.

[Backrooms on Babylon.js (Mobile version 3) | Babylon.js Playground](https://playground.babylonjs.com/#25EV8E)

Теперь нужно заменить стрелки на джойстики что-бы можно было вращать камеру игрока на 360 градуссов.

[Backrooms on Babylon.js (Mobile version 4) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#KBLZJ1#1)

## Мобильная версия Кейна Пикселя

Но просматривая свою версию бэкрумс на своём смартфоне я обнаружил что я не могу перемещаться на нём теперь давайте сделаем стрелки картинки что-бы можно было перемещаться на мобильной версии.

[Kane Pixel’s Backrooms on Babylon.js (Mobile version 2) | Babylon.js Playground](https://playground.babylonjs.com/#1GXGH8)

Теперь нужно убрать дебильные стрелки, и добавить джойстик что-бы можно было перемещаться на 360 градуссов.

[Kane Pixel’s Backrooms on Babylon.js (Mobile version 3) | Babylon.js Playground](https://playground.babylonjs.com/#HLQRG6#1)

Теперь нужно сделать так что джойстик мог перемещать камеру на 360 градуссов, и перемещатьься туда куда направленна камера.

[Kane Pixel’s Backrooms on Babylon.js (Mobile version 4) | Babylon.js Playground](https://playground.babylonjs.com/#NNNQS4#1)

## Опциональные версии бэкрумс

Бесконечный процедуирно генерируемый пол, и на нём столбы разного размера равномерно друг от друга расположенные, и так до бесконечности.

[Backrooms in Babylon.js (Optional version - The infernal Valley of pillars) | Babylon.js Playground](https://playground.babylonjs.com/#1P97PV#0)

Представим бэкрумс но в нём есть автоматическая камера котормая летает бесконечно случайно летает по случайным коридорам.

[Backrooms in Babylon.js (Optional version - Backrooms flying into the sky) | Babylon.js Playground](https://playground.babylonjs.com/#34X9YU#0)

Помните приложение рандонавтика его суть в том что есть карта Google на которой войды, и полноты, и в случайных зонах полнот генерируются точки аномальности где есть что-то типа странное, и необычное.

[Backrooms in Babylonjs(Optional version-Biome generation is like in a randonautica with zones of fullness and emptiness) | Babylon.js Playground](https://playground.babylonjs.com/#Y3TM2F#0)

Бэкрумс в котором бесконченый ковёр, и мы можем через поле ввода изменить этот ковёр на новую текстуру.

[Backrooms in Babylon.js(Optional version-The carpet is endless, but the texture can be changed through the input field) | Babylon.js Playground](https://playground.babylonjs.com/#AHP53D#0)

Представьте бэкрумс в котором есть только потолок, и пол а стен нету! Это именно то.

[Backrooms in Babylon.js (Optional version - no walls) | Babylon.js Playground](https://playground.babylonjs.com/#T7SDF5#0)

Бэкрумс но эта ловушка когда мы приближаемся к кордиорам выходы начинаются меняться.

[Backrooms in Babylon.js (Optional version - Trap) | Babylon.js Playground](https://playground.babylonjs.com/#GU5ZOU#0)

Представим что в бэкрумс есть много разных измерений, и в разных измерениях разные наборы биомов.

[Backrooms in Babylon.js (Optional version - In different dimensions, sets from different biomes XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#KQXD6E#0)

Представим что есть бесконечный процедурно генерируемый XYZ бэкрумс но генерация биомов происходит по маскам скажем 0 - это отсутвие комнаты 1 - это какая-то структура OBJ и так до бесконечности.

[Backrooms in Babylon.js (Optional version - Generating biomes by masks) | Babylon.js Playground](https://playground.babylonjs.com/#6M3H3Y#0)

Бесконечный процедурно генерируемый бэкрумс по XZ но в нём круглые стены случайно повернутые на 360 градуссов, и расположенные в случайных местах.

[Backrooms in Babylon.js (Optional version - Endless space XZ of round walls) | Babylon.js Playground](https://playground.babylonjs.com/#JEULSV#0)

Бесконечный процедурно генерируемый бэкрумс по XZ но в нём квадратные стены случайно повернутые на 360 градуссов, и расположенные в случайных местах.

[Backrooms in Babylon.js (Optional version - Endless hanging walls XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#5R23Z2#0)

Бесконечный процедурно генерируемый бэкрумс по XYZ но в нём квадратные стены случайного размера, и случайно повернутые на 360 градуссов, и расположенные в случайных местах равномерно что будто напомниает бесконечное разрушенное здание под завалами.

[Backrooms in Babylon.js (Optional version - Endless Ruined Building XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#IG2UMF#0)

Бесконечный процедурно генерируемый бэкрумс по XYZ но в нём квадратные стены случайного размера, и случайно повернутые на ровное количество градуссов в случайные стороны, и расположенные в случайных местах равномерно что будто напомниает бесконечное здание под завалами.

[Backrooms in Babylon.js (Optional version - Endless Building XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#3US01K#0)

Бесконечный процедурно генерируемый бэкрумс но в одном измерении один биом, в другом измерении другой биом, и так пока измерения не закончятся.

[Backrooms in Babylon.js (Optional version - Different dimensions with the same different biomes but in XYZ coordinates) | Babylon.js Playground](https://playground.babylonjs.com/#FMT8P7#0)

Новый челендж пробежаться по полу из обрезков случайных винтялиционных труб, и выжить.

[Backrooms in Babylon.js (Optional version - Endless trimming of ventilation pipes XZ version) | Babylon.js Playground.js](https://playground.babylonjs.com/#Z6EBKY#0)

Бэкрумс с множеством измерений где в каждом измерении свой отдельный биом но есть поле ввода для переключения между измерениями.

[Backrooms in Babylon.js (Optional version - Multiple dimensions with a switching field XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#0WCJ5W#0)

Хаос из понатыканых случайно друг в друга комнат, и коридоров, и так до бесконечности по XYZ незнаю зачем это ну пускай будет.

[Backrooms in Babylon.js (Optional version - Generating biomes by masks pre-alpha version) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#P4J1CZ#0)

Бэкрумс с бесконечной поверхностью вглубь где по бесконченой процедурной генерации по XZ, и с исключительной бесконечной генерацией по -Y а в вверх ничего не генерируется.

[Backrooms in Babylon.js (Optional version - Multi-storey multibiome generation, but only at -Y height in depth) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#V0MU79#0)

Представи пустое пространство в нём линия по XZ уходящая в случайные направления, и она ломанная и по ней генерирутся как по дороге различные биомы структур комнат, и коридоров.

[Backrooms in Babylon.js (Optional version - Generating structures along an infinite procedurally generated XZ line) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#VSYOND#0)

Представим что есть бесконченое пустое пространство, и в нём ломанная линии которая отклоняется в случайную сторону, и по этой ломанной линии XYZ генерируется структуры комнат, и коридоров.

[Backrooms in Babylon.js(Optional version-Generating structures along an infinite procedurally generated broken XYZ line) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#OHNQ3B#0)

Бэкрумс с бесконченой процедурной генерации по XZ, и с фиксированной по Y где есть определенное количество этажей скажем 3.

[Backrooms in Babylon.js (Optional version - Generating biomes by masks with a fixed number of floors in height) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#SSHIOZ#0)

Бэкрумс с бесконченой процедурной генерации по XZ, и с случайной от до бесконечности по Y этажей.

[Backrooms in Babylon.js (Optional version - Generating biomes by masks with a endless number of floors in height) | Babylon.js Playground](https://playground.babylonjs.com/#W5IHYX)

Отрицательный питфалс по сути кубы с расположеными между ними узкими ямами.

[negative pitfalls | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#Y4NELR#0)

С загрузкой OBJ, и замена все структур по XYZ на загруженную модель, и даже если выбран второй файл OBJ через эту кнопку то все структуры заменяются везде на второй OBJ. 

[Backrooms in Babylon.js (Optional version - With OBJ loading and replacing all XYZ structures with the loaded model) | Babylon.js Playground](https://playground.babylonjs.com/#2JR60S)

С загрузкой OBJ структур, и заменой случайных структур OBJ в XYZ на случайные загруженные структуры в случайных местах.

[Backrooms in Babylon.js(Optional version - With OBJ loading, and XYZ structures replacing with random loaded structures) | Babylon.js Playground](https://playground.babylonjs.com/#K0G096)

Бесконечная библиотека где бесконечно процедурно генерируются случайные буквы по XZ координатам.

[Backrooms in Babylon.js (Optional version - Endless library Russian version) | Babylon.js Playground](https://playground.babylonjs.com/#1V702E)

Бесконечный ковёр простирающийся от -Y до +Y.

[Backrooms in Babylon.js (Optional version - An infinitely generated wall) | Babylon.js Playground](https://playground.babylonjs.com/#IP4D7B)

Бесконечное количество генерируемых процедурно ковров простирающийся снизу вверх от -Y до +Y равномерно расположеных друг от друга по XZ.

[Backrooms in Babylon.js (Optional version - Infinitely generated from each other endless high-rise walls) | Babylon.js Playground](https://playground.babylonjs.com/#5HU3BZ)

Бесконечно генерируемые многоэтажные ковры.

[Backrooms in Babylon.js (Optional version - Infinitely generated infinitely multi-storey carpets) | Babylon.js Playground](https://playground.babylonjs.com/#1VBEPK)

Представьте что бэкрумс это бесконечный куб заполненый замкнутыми кубами! Вот с чего надо было начать...

[Backrooms in Babylon.js (Optional version - Infinite dense space of cubes XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#RM8AZ7)

Теперь нужно вырезать в этом бесконченом бетоном кубе коридоры, и комнаты пустот что-бы сделать бэкрумс но получилось какое-то кубические пещеры.

[Backrooms in Babylon.js (Optional version - Endless Cubic Caves XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#P9WI82)

После долгих мучений, и страданий с бэкрумс я все таки решил вернуться к своей изначальной задумке которую мне не удалось реализовать изначально но пытаясь сново пойти старыми путями случайно создал уровень Black Zone где на половину сломанные помещения, и комнаты висящие в пустоте.

[Backrooms in Babylon.js (Optional version - Black zone) | Babylon.js Playground](https://playground.babylonjs.com/#OB1SG3)

Версия от моего давнего приятеля CodingCrusader [оригинал комментария](https://forum.babylonjs.com/t/coding-crusaders/44765/382) но мой аккаунт к сожалению был удален модератором... Вообще его версия это просто бесконечные кубиклы но он не залил её на плошадку бабилона так что я переписал его код без html.

[Backrooms in Babylon.js (Optional version - Endless Cubicles CodingCrusader) | Babylon.js Playground](https://playground.babylonjs.com/#IQ407T)

Бесконечная процедурная генерация GLB структур по XZ.

[Backrooms in Babylon.js (Optional version - Endless procedural generation of GLB structures by XZ) | Babylon.js Playground](https://playground.babylonjs.com/#3XBMAI#2)

## Процедурные генерации в бэкрумс онлайн версии

Я хотел конвертировать [свои процедурные генерации бэкрумс](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python) с python на babylon.js что-бы внести финальную лепту в бэкрумс Кейна Пикселя.

[Procedural generation of the backrooms (The most accurate version) | Babylon.js Playground](https://playground.babylonjs.com/#774AAM)

## Kane Pixel’s Backrooms in Babylon.js - Optional version

Представим что бэкрумс это пирог где на одном этаже один биом, на втором этаже другой биом, и так когда цикл количества биомов завершается он повторяется снова, и так до бесконечности.

[Kane Pixel’s Backrooms in Babylon.js (Optional version - Cake multi-storey biome generation) | Babylon.js Playground](https://playground.babylonjs.com/#LS4GSZ#0)

Версия бэкрумс где есть один биом который между всеми биомами, и в нём кубы биомов разного размера.

[Kane Pixel’s Backrooms in Babylon.js (Optional version - Cubic multi-storey biome generation) | Babylon.js Playground](https://playground.babylonjs.com/#945FVB#0)

## Бэкрумс на изурфейсах

[Backrooms on isurfaces (version 0 - Themezzanine 2) | Babylon.js Playground](https://playground.babylonjs.com/#YCI2DG#3)

## Бэкрумс + Гонки

[![Zapis-2024-12-14-03-55-58-220.gif](https://i.postimg.cc/2ST2Z3qv/Zapis-2024-12-14-03-55-58-220.gif)](https://postimg.cc/JsDNwr54)

[PhysicsV2 Car Simulation Example (Endless carpet) | Babylon.js Playground](https://playground.babylonjs.com/#LO1E72#2)

[![Zapis-2024-12-14-08-34-07-590-1.gif](https://i.postimg.cc/DzPr0ZMb/Zapis-2024-12-14-08-34-07-590-1.gif)](https://postimg.cc/wt3yb6H6)

[PhysicsV2 Car Simulation Example (Endless backrooms) | Babylon.js Playground](https://playground.babylonjs.com/#9ZO5H6#1)

![Zapis-2024-12-14-06-35-54-915](https://github.com/user-attachments/assets/39db0c90-9866-4d52-a847-6d6961f194d1)

[PhysicsV2 Car Simulation Example (The broken floor) | Babylon.js Playground](https://playground.babylonjs.com/#24VH6Q#1)

![Запись_2025_12_06_19_45_02_309](https://github.com/user-attachments/assets/64515dd7-dea7-4c02-bb1c-3c94ca284709)

[PhysicsV2 Car Simulation Example (Endless carpet 2) | Babylon.js Playground](https://playground.babylonjs.com/#JNPQCL#1)

## Бэкрумс в Babylon.js — стены по сеткам линий

Бэкрумс но мы сделали сетки из линий по маскам и по этим сеткам делаем стены, и так получается бесконечный лабиринт, и заранее заданных масок стен.

[Backrooms in Babylon.js (Walls on grids of lines - Endless procedural generation of walls based on masks of lines) | Babylon.js Playground](https://playground.babylonjs.com/#TFUHZL#0)

Теперь добавляем пол к стенам по маскам.

[Backrooms in Babylon.js(Walls on grids of lines-Endless procedural generation of walls based on masks of lines + carpet) | Babylon.js Playground](https://playground.babylonjs.com/#F0O9DA)

После долгих размышлений на тему бэкрумса я понял что что-бы создать бэкрумс это больше про работу с сетками - нужно просто взять сетку из линий, и в случайном процентном соотношении удалить случайные отрезки линий, и тогда по этим линиям провести стены, и легко получится лабиринт бэкрумс.

[Backrooms in Babylon.js (Walls on grids of lines - The endless grid with diagonals is broken) | Babylon.js Playground](https://playground.babylonjs.com/#39Z59A#0)

И как продолжение предыдущего диалога была мысль сделать четыре линии ветки с асимптотой в определённой диапазон отклонения, и по линиям раставить точки разного цвета которые как маркер помечают места других линий, и по ним сделать OBJ разных форматов, и так получается полноценный бэкрумс!

[Backrooms in Babylon.js(Walls on grids of lines-The endless grid with diagonals is broken+4 branch lines+OBJ on lines) | Babylon.js Playground](https://playground.babylonjs.com/#PBWP6O#3)

# Бэкрумс другие уровни

## Уровень 11 — Бесконечный город

Бесконечный город с заданным количество одних и тех де зданий где здания прилегают к друг к другу тык в притык.

[Backrooms in Babylon.js level 11 - The Endless Sity (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#D14H1M#0)

Бесконечный город на бесконечной плоской земле равномерно друг от друга здания.

[Backrooms in Babylon.js level 11 - The Endless Sity (Version 1) | Babylon.js Playground](https://playground.babylonjs.com/#N96KG5#0)

Теперь нужно сделать генерацию зданий по маскам.

[Backrooms in Babylon.js level 11 - The Endless Sity (Version 2) | Babylon.js Playground](https://playground.babylonjs.com/#2NVEV2#1)

## Уровень - Бесконечное небо

Бэкрумс уровень бесконечное небо с бесконечно процедурно генерирумымм молниями.

[Backrooms in Babylon.js (Optional version - Endless sky with lightnings) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#V2MVHL)

Теперь нужно убрать молнии что-бы просто оставить процедурно генерируемый бесконечный туман.

[Backrooms in Babylon.js (Optional version - Endless sky) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#G14EV7)

Теперь сделаем бесконечно процедурно генерируемый туман с бесконечно процедруно генерируемым снегом.

[Backrooms in Babylon.js (Optional version - Endless sky with fog and snow) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#XSO03M)

## Уровень -9223372036854775808

Хотел сделать бесконечный океан глюка типа как уровень монохром как его чаще называют [Backrooms Level -9223372036854775808](https://sketchfab.com/3d-models/backrooms-level-9223372036854775808-5e0a01f01cf44cffacb7ae56750ea099), и сделал бесконечно процедурно генерируемые микро шумы:

[Endless procedurally generated micro noise | Babylon.js Playground](https://playground.babylonjs.com/#2AETZY#0)

Бесконечный океан цветного глитча первая версия.

[Backrooms in Babylon.js (Optional version - An endless ocean of colored foam) | Babylon.js Playground](https://playground.babylonjs.com/#NYGRIF)

Теперь мне нужно заставить их колебаться.

[Backrooms in Babylon.js (Optional version - Dancing thorns) | Babylon.js Playground](https://playground.babylonjs.com/#NH56YZ)

Но мне не нужно что-бы они танцевали нужно что-бы они флуктуировали.

[Backrooms in Babylon.js (Optional version - Endless fluctuating ocean of colored noise) | Babylon.js Playground](https://playground.babylonjs.com/#07SF66)

## Уровень - Бесконечное море цветного шума

Но вот теперь осталось лишь сделать бесконечную процедурно генерируемую плосокость цветного шума, и это уже похоже на уровень монохрома.

[Backrooms in Babylon.js (Optional version - Endless colored noises) | Babylon.js Playground](https://playground.babylonjs.com/#3Z112L)

## Уровень - Матрица

Кто нибудь помнит фильм такой 'Матрица: Начало'? Так вот там был в начале такой [цифровой дождь из символов](https://youtu.be/liFjsSDj1eM?si=0WwII9Ifju1I3UNr) я сделал так же! 

[Backrooms in Babylon.js (Optional version - The Matrix English version + Numbers) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#F1G34G)

Теперь нужно сделать матрицу из разных символов Русского алфавита.

[Backrooms in Babylon.js (Optional version - The Matrix Russian version) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#9GK0IB)

Та же матрица, и я решил сделать так же только с анимацией.

[Backrooms in Babylon.js (Optional version - The Matrix Russian version with animation) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#QSNV5N)

Бесконечная библиотека где бесконечно процедурно генерируются случайные буквы по XZ координатам включая табло координат полей ввода что-бы перемещаться по XYZ.

[Backrooms in Babylon.js (Optional version - The Matrix Endless Library Russian version + Coordinate board) | Babylon.js Playground](https://playground.babylonjs.com/#14XFIB)

В этом дожде из матрице есть однозначно какой-то глубиный смысл только нужно понять какой... Ведь как известно там где высоко там снизу вселенная лишь многомерится меняя лишь эталон, и меру.

## P.S.

Теперь это полноценное закулисное пространство! Возможно, кто-то придумает какие-то новые проекты, и проект будет развиваться.
