Наборы FPS игр бэкрумс в стиле свободного мира с бесконечной процедурной генерации включающий 134 кода(ов) созданные мной.

Тема созданна на [Endless backrooms in Babylon.js! - Demos and projects - Babylon.js](https://forum.babylonjs.com/t/endless-backrooms-in-babylon-js/55544/45) но потом мой аккаунт удалили, и теперь пришлось писать всё здесь.

# Предисловие 

Сколько было попыток создать бэкрумс, и хочу отметить что до сих пор так никому, и не удалось полноценно реализовать идею бэкрумса! Ведь что такое бэкрумс!? Бэкрумс это в первую очередь идея бесконечного лабиринта куда что-то, или кто-то случайно выпадает из реальности, и попадая в этот бесконечный лабиринт оно пытается там выжить и выбраться оттуда, и вся суть в том что чем больше от туда кто-то пытаются выбраться тем больше  становиться тех кто туда случайно выпадает из реальности, и при каждой последующей итерации того как кто-то оттуда выбирается это место становиться все более сломанным, и тем больше выбраться оттуда становиться всё более сложнее, и в конечном итоге окажется так что весь мир, а то и вся вселенная навечно провалится в бэкрумс, и все будут бесконечно блуждать в бесконечном лабиринте бесконечно долго пока вся эта бесконечность не придет к какому-то общему знаменателю но к какому!?

# Бэкрумс что это!?

Бэкрумсом может считаться то что попадает под следующие категории общего образа:

1.	Лиминальность – Это повторяемость, и однообразность каких-либо помещений, коридоров, комнат и т.д. Которые соответствуют определённому образу. Места, которые вызывают ностальгию.
  
2.	Монострузность – Огромность, гигантизм, либо же бесконечность простираемых пространств.
  
3.	Дримкор – Это места из сновидений олицетворяющие какие-то места, и действия, происходящие в этих снах. 

# Типы процедурной генерации

## Класическая процедурная генерация

Как вообще работает процедурная генерация? На примере игры Starbound самая такая обычная процедурная генерация, вот на примере дома, вот нам нужно сделать процедурную генерацию дома в игре как это делается? Берется делается 20 типов крыш, 20 типов дверей, 20 там типов окон, т.д. И делается всевозможная вариация всевозможных комбинаций элементов этого дома, и получается огромное число домов так работает класическая процедурная генерация.

## Каноническая процедурная генерация

Каноническая процедурная генерация это самая хардкорная процедурная генерация из всех она отличается от других тем что в ней генерируются уровень только строго согласно образу этому уровню к примеру, если это уровень 0, то в нём есть только желтые ковры, только желтые обои, только люминесцентные ламп, и только белая потолочная плитка типа Армстронг-Байкал, за исключением подуровней, которые являются переходом в другие уровни.

## Биомная процедурная генерация 

Биомная процедурная генерация подразумевает под собой определенное количество биомов, и в каждом биоме генерируется специально заданная структура генерации.

## Мультибиомная процедурная генерация

Мультибиомная процедурная генерация подразумевает под собой определенное количество биомов скажем 12 биомов, и всевозможные вариации комбинаций этих биомов, которые генерируется как куб случайного размера.

## Пирог неевклидового пространства

Процедурная генерация по Кейну Пикселю это бесконечный слоённый пирог неевклидового пространства к примеру, сначала идет 100 метров нулевого уровня помещения заканчивается, и потом идут 200 метров пятого уровня, и так до бесконечности… Каждый размер пространства генерации уровня генерируется случайно. 

## С зонами нормальностей, и зонами аномальностей

С зонами нормальностей, и зонами аномальностей отличается от других тем что в классической процедурной генерации пространство разделяется на зоны нормальности, и анормальности.

Процедурная генерация с зонами нормальностей, и зонами аномальностей в бекрумсе разделяется на:

1.	Зона нормальность – В зоне нормальности процедурная генерация генерируется соответствуя общепринятому образу этого уровня от 0 до 1 по градиенту, и чем ближе оно к единице, тем больше соответствует этому образу, и если оно равно 1 значит оно полностью олицетворяет этот образ, к примеру нулевую уровень состоит из определенного типа жёлтых обоев, ковра, люминесцентных ламп, и белой потолочной плитке типа Армстронг-Байкал, то есть это трехмерное пространство полностью заполненное процедурно сгенерированными комнатами-помещения словно как дырки в сыре.
   
2.	Зона анормальности - В зоне анормальности процедурная генерация генерируется, отклоняясь от общепринятого образа этого уровня от 0 до -1 по градиенту, и чем ближе оно к -1, тем больше оно противоположно этому образу, и, если оно равно -1 значит оно полностью противоположно этому образу, к примеру, если зона равна -0.2 то в ней изредка начинают генерироваться различные предметы типа стула, стола, и т.д. В том же духе… Если зона к примеру, равна -0.5 то отсутствуют люминесцентные лампы, ковер, либо же люминесцентные лампы генерируются, но не работают, другие обои на стенах, или комната может быть перевернутой сверху-вниз, и т.д. Если же зона анормальности равна -1 то в ней обязательно генерируется локация, переход на другой подуровень, уровень, а также может быть различные сущности.
   
Территория зоны может генерироваться по-разному обычно она генерируется равномерно, неравномерно, или стохастично. Равномерное генерация — это когда к примеру, на куб в 100 километров процедурно сгенерированного пространства половина зона анормальности, а остальная половина зона нормальности. Неравномерная генерация — это когда к примеру, на куб в 100 километров процедурно сгенерированного пространства 35 километров это зона анормальности, а остальное это зона нормальности. Обычно территория зоны генерируется неравномерно в пользу нормальности.

## Процедурная генерация уровней

Есть какой-то общепринятый образ какого-то уровня к примеру, берётся какое-либо здание, например - супермаркет, и дальше этот образ разделяется на элементы из которого этот образ состоит, и методом математической комбинаторики делается всевозможные перестановки, и комбинации-добавления-удаления элементов на которые был разложен этот образ, и таким образом получается бесконечное число уровней этого образа.
Процедурная генерация объектов в уровнях

Есть какой-то общепринятый образ того какие объекты могу наполнять этот уровень, и какого-то количества этих объектов, берётся какое-либо здание например - супермаркет, и дальше разделяться на частоту размещения этих объектов в уровне чтобы на каждый куб пространства этого уровня размеров 1 километр на 1 километр приходилось случайное количество объектов от примерно 0 до 1000. К примеру, если это зона анормальности, то шанс на количество объектов в этой зоне повышается, и становиться от 500 до 1000.  А если это зона нормальности, то шанс на выпадения случайного количества объектов в нем понижается, и становиться от 0 до 1000. На каждом уровне на каждый куб пространства в этом уровне количество случайных объектов, расположенных в этом уровне соответственно разное скажем если уровень 0, то в нём на 1 кубический километр пространства будет от 0 до 1000 объектов, а если это другой уровень, то там уже скажем от 1000 до 2000, и т.д.

## Процедурная генерация сущностей в уровнях

Сущности в бэкрумсе олицетворяют сами уровни, в которых они существует ведь бэкрумс это место куда выпадают из реальности, например, если уровень из себя бесконечный магазин телевизоров, то и соответственно сущность представляет из себя гуманоида у которого вместе головы телевизор. Сама процедурная генерация сущностей генерирует нейронная сеть, которая совмещает два каких-то образа существа, и создает таким образом какой-то новый образ, и так до бесконечности.

# Версия ПК 

Я создал бэкрумс на движке babylon.js перемещаться с помощью стрелок ←, →, ↑, ↓ на клавиатуре и мыши.

# Оригинальный бэкрумс 

По оригинальному канону бэкрумс - это место, расположенное под текстурами реальности, представляющее однообразные пространства уровней процедурно сгенерированного мира из неиспользуемого и вырезанного контента. Вещи, которые либо не подходили, либо были недостаточно хороши для их создания. Вырезка для реального мира. К примеру, если это уровень 0, то в нём только жёлтые ковры, только жёлтые обои, только люминесцентные ламп, и только белая потолочная плитка типа Армстронг-Байкал, и так до бесконечности.

## Бэкрумс по канону 	

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

# Версия Кейна Пикселя

В понимании Кейна Пикселя, бэкрумс - это место, расположенное под текстурами реальности, представляющее один бесконечный слоённый пирог пространства состоящий из разных уровней процедурно сгенерированного мира неиспользуемого и вырезанного контента. Вещи, которые либо не подходили, либо были недостаточно хороши для их создания. Вырезка для реального мира. К примеру, сначала идет 100 метров нулевого уровня помещения заканчивается, и потом идут 100 метров пятого уровня, и так до бесконечности…

## Бэкрумс по Кейну Пикселю

В первой версии я добавил возможность генерации структуры на основе граней и массивов вершин. Вам просто нужно немного отклониться в сторону, чтобы увидеть генерацию.

[Kane Pixel’s Backrooms in Babylon.js (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#CBZ7JF)

Во второй версии я добавил разные биомы, и теперь генерируется не один биом, а много.

[Kane Pixel’s Backrooms in Babylon.js (Version 1 - multybiom generation) | Babylon.js Playground](https://playground.babylonjs.com/#RSODNR)

Но чего-то все ещё не хватает, потому что подсобные помещения Kane Pixel представляют собой бесконечный многоуровневый пирог из случайно сгенерированных процедурно взаимосвязанных пространств.

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

Бесконечный процедурно генерируемый пол, и на нём столбы разного размера равномерно друг от друга расположенные, и так до бесконечности.

[Backrooms in Babylon.js (Optional version - The infernal Valley of pillars) | Babylon.js Playground](https://playground.babylonjs.com/#1P97PV#0)

Представим бэкрумс но в нём есть автоматическая камера котормая летает бесконечно случайно летает по случайным коридорам.

[Backrooms in Babylon.js (Optional version - Backrooms flying into the sky) | Babylon.js Playground](https://playground.babylonjs.com/#34X9YU#0)

Помните приложение рандонавтика его суть в том что есть карта Google на которой войды, и полноты, и в случайных зонах полнот генерируются точки аномальности где есть что-то типа странное, и необычное.

[Backrooms in Babylonjs(Optional version-Biome generation is like in a randonautica with zones of fullness and emptiness) | Babylon.js Playground](https://playground.babylonjs.com/#Y3TM2F#0)

Бэкрумс в котором бесконченый ковёр, и мы можем через поле ввода изменить этот ковёр на новую текстуру.

[Backrooms in Babylon.js(Optional version-The carpet is endless, but the texture can be changed through the input field) | Babylon.js Playground](https://playground.babylonjs.com/#AHP53D#0)

Представьте бэкрумс в котором есть только потолок, пол, и люминисцентные лампы а стен нету! Это именно то.

[Backrooms in Babylon.js (Optional version - no walls) | Babylon.js Playground](https://playground.babylonjs.com/#T7SDF5#0)

Бэкрумс но эта ловушка когда мы приближаемся к кордиорам выходы начинаются меняться.

[Backrooms in Babylon.js (Optional version - Trap) | Babylon.js Playground](https://playground.babylonjs.com/#GU5ZOU#0)

Представим что в бэкрумс есть много разных измерений, и в разных измерениях разные наборы биомов.

[Backrooms in Babylon.js (Optional version - In different dimensions, sets from different biomes XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#KQXD6E#0)

Представим что есть бесконечный процедурно генерируемый XYZ бэкрумс но генерация биомов происходит по маскам скажем 0 - это отсутвие комнаты, 1 - это какая-то структура OBJ, и так до бесконечности.

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

Бэкрумс с бесконечной процедурной генерации по XZ, и с фиксированной по Y где есть определенное количество этажей скажем 3.

[Backrooms in Babylon.js (Optional version - Generating biomes by masks with a fixed number of floors in height) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#SSHIOZ#0)

Бэкрумс с бесконечной процедурной генерации по XZ, и с случайной от до бесконечности по Y этажей.

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

Представим бэкрумс но есть только потолок, и пол. 

[Backrooms in Babylon.js (Optional version - no walls just endless carpet and endless ceiling) | Babylon.js Playground](https://playground.babylonjs.com/#N10Q92)

Представим бэкрумс но есть бесконечные многоэтажные помещения без стен из бесконечных потолков, и бесконечных полов.

[Backrooms in Babylon.js (Optional version - endless generated endless multi-storey carpets and ceilings) | Babylon.js Playground](https://playground.babylonjs.com/#8K5E4U)

Отлично наконец я решил проблему с CSG я сделал бесконечную версию XZ.

[Backrooms in Babylon.js (Optional version - The most accurate endless XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#774AAM#2)

Бесконечные процедурные трубы ковёр XZ версия.

[Backrooms in Babylon.js (Optional version - Endless procedural pipes XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#UL25WX)

Представьте бэкрумс бесконечный но эта стена которая простирается с -Y по +Y бесконечно с полем ввода которая изменяет текстуру на URL картинку этой стены.

[Backrooms in Babylon.js (Optional version - An infinitely generated -Y +Y wall + image URL input field) | Babylon.js Playground](https://playground.babylonjs.com/#OFVLEP)

Тоже что и The most accurate endless XZ version версия только с телепортом. 

[Backrooms in Babylon.js (Optional version - The most accurate endless XZ version + teleport) | Babylon.js Playground](https://playground.babylonjs.com/#8QMAW9)

Реализация уровня [The Hub](https://sketchfab.com/3d-models/backrooms-level-thehub-canone-c36d56a2e38743f0837b8e0bd790d900) с бесконечным дорожным туннелем подземным по бокам которых двери на разные уровни.

[Backrooms in Babylon.js (Optional version - Level The Hub) | Babylon.js Playground](https://playground.babylonjs.com/#EET6L1#1)

По сути тоже самое что, и бесконечный ковёр только здесь текстура RGB а не из URL.

[Backrooms in Babylon.js (Optional version - Endless Carpet XZ version but no URL just RGB Image) | Babylon.js Playground](https://playground.babylonjs.com/#CRW33S#1)

## Другие процедурные генераторы в бэкрумс

Голографическая версия многоэтажных басеинов залов перевод с [Multy storey poolrooms](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/multi-storey-poolrooms.py) пайтон версии... Типа кто помнит что когда вращаешь камеру с одной стороны есть с другой нету это типа такое многомерное пространство получается или типа случайно как-то поялвяется при вращаение случайная структура...

[Procedural generation of the backrooms (Multi-storey-poolrooms) | Babylon.js Playground](https://playground.babylonjs.com/#ELI45L)

Процедурный генератор небоскрёба.

[Procedural generation of the backrooms (Multi-storey Skyscraper Procedural Generation) | Babylon.js Playground](https://playground.babylonjs.com/#L9HFKV#2)

Процедурный генератор бруталиских руин.

[Procedural generation of the backrooms (Procedural Building Ruins Generator - Brutal ruins) | Babylon.js Playground](https://playground.babylonjs.com/#SEDQ30#1)

Процедурный генератор бруталиских зданий для паркура.

[Procedural generation of the backrooms (Procedural Parkour Building Generator - Brutalist parkour) | Babylon.js Playground](https://playground.babylonjs.com/#JBELT4#1)

Странные комнаты с стенами на поверхностях странных обрезанных ландшафтов.

[Procedural generation of the backrooms (A procedural generator of strange the backrooms - Strange rooms) | Babylon.js Playground](https://playground.babylonjs.com/#XEEUEY)

Упрощённый бруталиский паркур ввиде одного здания.

[Procedural generation of the backrooms (Procedural Parkour Building Generator - Simplified brutalist parkour) | Babylon.js Playground](https://playground.babylonjs.com/#A7EDOY)

## Kane Pixel’s Backrooms in Babylon.js - Optional version

Представим что бэкрумс это пирог где на одном этаже один биом, на втором этаже другой биом, и так когда цикл количества биомов завершается он повторяется снова, и так до бесконечности.

[Kane Pixel’s Backrooms in Babylon.js (Optional version - Cake multi-storey biome generation) | Babylon.js Playground](https://playground.babylonjs.com/#LS4GSZ#0)

Версия бэкрумс где есть один биом который между всеми биомами, и в нём кубы биомов разного размера.

[Kane Pixel’s Backrooms in Babylon.js (Optional version - Cubic multi-storey biome generation) | Babylon.js Playground](https://playground.babylonjs.com/#945FVB#0)

Версия XZ бэкрумса Кейна Пикселя со смятыми коридорами, и комнатами бескнечно процедурно генерируемая.

[Kane Pixel’s Backrooms in Babylon.js (Optional version - Endless XZ multybioms crumpled version) | Babylon.js Playground](https://playground.babylonjs.com/#5ADFJW)

## Бэкрумс на изурфейсах

Я хотел конвертировать [свои процедурные генерации бэкрумс](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python) с python на babylon.js что-бы внести финальную лепту в бэкрумс Кейна Пикселя. 

Хотел переписать код с python [Procedural-generation-of-the-backrooms-python/With-polygons/themezzanine2.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/themezzanine2.py) на Babylon.js но получилось в отдельном чанке комнаты изурфейсов.

[Backrooms on isurfaces (version 0 - Themezzanine 2) | Babylon.js Playground](https://playground.babylonjs.com/#YCI2DG#5) 

Теперь хочу переписать [Multi-storey-curved-corridor.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-curved-corridor.py) на Babylon.js и вот что получилось:

[Backrooms on isurfaces (version 1 - Wormholes) | Babylon.js Playground](https://playground.babylonjs.com/#3GSN00#1)

Теперь нужно сделать в одном чанке этот код [multi storey hell.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/multi-storey-hell.py).

[Backrooms on isurfaces (version 2 - Multi-storey-hell in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#7VUKJ2#1)

Ну вот в одном чанке сделаем этот код [Multi storey poolroms just coridors](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-poolrooms-just-coridors.py) 

[Backrooms on isurfaces (version 3 - Multi storey poolrooms just corridors in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#2BW5WL)

Изурфейсная wireframe сетка версия многоэтажных басеинов залов перевод с [Multy storey poolrooms](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/multi-storey-poolrooms.py) пайтон версии...

[Backrooms on isurfaces (version 4 - Multi-storey-poolrooms in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#D85Z0S)

Тоже что и предыдущая только с кнопкой скачать OBJ.

[Backrooms on isurfaces (version 5 - Multi-storey-poolrooms in One chunk + Download button) | Babylon.js Playground](https://playground.babylonjs.com/#W1J8E9)

Теперь нужно сделать уровни с горизонтально положенными комнами и соиденния ввиде вертикальных стволов между ними как в этом коде [Multi-storey-poolrooms-fixed-height-one-connection.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-poolrooms-fixed-height-one-connection.py) 

[Backrooms on isurfaces (version 6 - Multi-storey poolrooms fixed height one connection + Download button) | Babylon.js Playground](https://playground.babylonjs.com/#2Y8A5H)

Переписал с python код [Multi-storey poolrooms smooth.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/multi-storey-poolrooms-smooth.py) на Babylon.js.

[Backrooms on isurfaces (version 7 - Multi-storey poolrooms smooth + Download button) | Babylon.js Playground](https://playground.babylonjs.com/#94Z2PF)

Многоэтажные туннели вертикальных пещер.

[Backrooms on isurfaces (version 8 - Multi-storey tunnels of vertical caves in One chunk + Download button) | Babylon.js Playground](https://playground.babylonjs.com/#42BZNW)

Бесконечные пещеры XYZ версия на изурфейсах.

[Backrooms on isurfaces (version 9 - Endless Caves XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#AN50SK)

Перевод самой точной версии бэкрумс [The most accurate version.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/The%20most%20accurate%20version.py) с python на babylon.js...

[Backrooms on isurfaces (version 10 - The most accurate version in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#JQI83H)

Перевод версии с ровными поворотами [The most accurate version but they are turned exactly.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/The%20most%20accurate%20version%20but%20they%20are%20turned%20exactly.py)

[Backrooms on isurfaces (version 11 - The most accurate version but they are turned exactly in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#GDWKAZ)

Перевод версии с [The angular corridors of the backrooms are hollow.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/The%20angular%20corridors%20of%20the%20backrooms%20are%20hollow.py) на Babylon.js

[Backrooms on isurfaces (version 12 -The angular corridors of the backrooms are hollow in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#GSB3M7)

Перевод с версии [Sharp-angled hollow corridors backrooms with rooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/Sharp-angled%20hollow%20corridors%20backrooms%20with%20rooms.py)

[Backrooms on isurfaces (version 13 - Sharp-angled hollow corridors backrooms with rooms on One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#4C9DP7)

Перевод с версии гиперкуба [Hypercube poolrooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Hypercube-poolrooms.py) только с острыми углами а не тупыми.

[Backrooms on isurfaces (version 14 - Hypercube) | Babylon.js Playground](https://playground.babylonjs.com/#439KYS#2)

Перевод с версии [Single storey poolrooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/single-storey-poolrooms.py) на Babylon.js

[Backrooms on isurfaces (version 15 - Single-storey poolrooms) | Babylon.js Playground](https://playground.babylonjs.com/#GLJ3DZ)

Тоже что и предыдущая только я положил на бок генерацию что-бы генерировать с XZ осях.

[Backrooms on isurfaces (version 16 - Single-storey poolrooms XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#ZUPQG1)

Перевод с версии [Single storey poolrooms smooth.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/single-storey-poolrooms-smooth.py) на Babylon.js

[Backrooms on isurfaces (version 17 - Single-storey poolrooms smooth XZ in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#0RSVQX#1)

То же что, и 16 версия бэкрумса на изурфейсах только бесконечно процедурно генерируемая.

[Backrooms on isurfaces (version 18 - Single-storey poolrooms endless procedural XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#FIN4ON#1)

То же что, и 13 версия только повернута по XZ а не снизу вверх как-та самая версия.

[Backrooms on isurfaces (version 19 - Sharp-angled hollow corridors backrooms with rooms on One chunk XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#FJ528J)

Тоже что, и 12 версия только повернута по XZ а не снизу вверх как-та самая версия.

[Backrooms on isurfaces (version 20 -The angular corridors of the backrooms are hollow in One chunk XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#3AHFKT)

Теперь сделаем ту же версию с повернутыми на 360 градуссов помещениями я переписал из [The most accurate version randomly rotated on 360 ](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/The%20most%20accurate%20version%20randomly%20rotated%20on%20360.py).

[Backrooms on isurfaces (version 21 - The most accurate version randomly rotated on 360 in One chunk XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#T9XNEB#1)

Перепишем многоэтажный комплекс соединенный лифтовыми шахтами за основу взято -> [Corridors backrooms is sharp multi-storey.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/Corridors%20backrooms%20is%20sharp%20multi-storey.py)

[Backrooms on isurfaces (version 22 - Corridors backrooms is sharp multi-storey in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#7EA8DB)

Чем-то напоминает далёкие земли бэкрумса где генерация типа настолько сломанна что это же неполносвязнные коридоры, и комнаты висящие где в пустоте отдельно друг от друга, и хотя далёкие земли бэкрумса это просто каша из глюков то есть скорее было-бы коректнее назвать это преддалёкими землями бэкрумса что-то типа в таком духе...

[Backrooms on isurfaces (version 23 - Endless Dark Zone XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#AU1RDG)

Перевод с версии [Multi-storey-poolrooms-just-coridors.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-poolrooms-just-coridors.py) моя самая любимая версия.

[Backrooms on isurfaces (version 25 - Multi-storey poolrooms just corridors)) | Babylon.js Playground](https://playground.babylonjs.com/#U5QGRN)

Теперь нужно сделать снизу-вверх версию а то слева-направо.

[Backrooms on isurfaces (version 26 - Multi-storey poolrooms just corridors in One chunk XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#GL3ZJW)

Перевод с версии [Multi-storey-poolrooms-combined.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-poolrooms-combined.py).

[Backrooms on isurfaces (version 27 - Multi-storey-poolrooms-combined) | Babylon.js Playground](https://playground.babylonjs.com/#H95KY7)

Перевод с версии [Hypercube-poolrooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Hypercube-poolrooms.py)

[Backrooms on isurfaces (version 28 - Hypercube poolrooms) | Babylon.js Playground](https://playground.babylonjs.com/#HYIAS9)

Перевод с версии [Multi-storey-poolrooms-mega-coridors.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/multi-storey-poolrooms-mega-coridors.py)

[Backrooms on isurfaces (version 29 - multi-storey-poolrooms-mega-corridors) | Babylon.js Playground](https://playground.babylonjs.com/#AF7NM8)

Перевод с версии [Multi-storey-curved-corridor.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-curved-corridor.py)

[Backrooms on isurfaces (version 30 - Multi-storey-curved-corridor) | Babylon.js Playground](https://playground.babylonjs.com/#U05M6G#1)

Перевод с версии [From-room-to-room-multistory.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/From-room-to-room-multistory.py)

[Backrooms on isurfaces (version 31 - From-room-to-room-multistory) | Babylon.js Playground](https://playground.babylonjs.com/#W0050K#1)

Перевод с версии [Hypercube-without-rooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Hypercube-without-rooms.py)

[Backrooms on isurfaces (version 32 - Hypercube-without-rooms) | Babylon.js Playground](https://playground.babylonjs.com/#2OTRRH#2)

Перевод с версии [Corridor-multi-storey-chaos-poolrooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Corridor-multi-storey-chaos-poolrooms.py)

[Backrooms on isurfaces (version 33 - Corridors-multi-storey-chaos-poolrooms) | Babylon.js Playground](https://playground.babylonjs.com/#BQMC0D)

Перевод с версии [Multi-storey-poolrooms-askew.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Multi-storey-poolrooms-askew.py)

[Backrooms on isurfaces (version 34 - Multi-storey-poolrooms-askew) | Babylon.js Playground](https://playground.babylonjs.com/#VP0S93)

Перевод с версии [Hypercube-spherical.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Hypercube-spherical.py)

[Backrooms on isurfaces (version 35 - Hypercube-spherical) | Babylon.js Playground](https://playground.babylonjs.com/#QAC35T)

Перевод с версии [Single-storey-corridors-without-poolrooms.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/With-polygons/Single-storey-corridors-without-poolrooms.py)

[Backrooms on isurfaces (version 36 - Single-storey-corridors-without-poolrooms) | Babylon.js Playground](https://playground.babylonjs.com/#7M8FQI)

Тоже что и предыдущий код только XZ версия.

[Backrooms on isurfaces (version 37 - Single-storey-corridors-without-poolrooms in One chunk XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#DS0DW1)

Тоже что и 33 версия только за место нормальных изурфейсов мишура изурфейсов.

[Backrooms on isurfaces (version 38 - Corridors-multi-storey-chaos-poolrooms tinsel from isurfaces) | Babylon.js Playground](https://playground.babylonjs.com/#7G4WNN)

Тоже что и Wormholes только в одном чанке а не бесконечно.

[Backrooms on isurfaces (version 39 - Corridors-multi-storey-chaos-poolrooms random rotated 360 in One chunk XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#WWOFK7)

Версия с вертикальными шахтами с проходами к случайным таким же шахтам.

[Backrooms on isurfaces (version 40 - Vertical, and horizontal wormholes in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#370JOG)

Чисто вертикальные стволы шахт.

[Backrooms on isurfaces (version 41 - Vertical pillars) | Babylon.js Playground](https://playground.babylonjs.com/#GNFT2W)

Тоже что и предыдущая только столбы от самого низа до самого вверха.

[Backrooms on isurfaces (version 42 - Vertical pillars from the very bottom to the very top) | Babylon.js Playground](https://playground.babylonjs.com/#R43RXI)

Тоже что и предыдущая только без плоскостей сверху и низу.

[Backrooms on isurfaces (version 43 - Vertical pillars from the very bottom to the very top but no ground) | Babylon.js Playground](https://playground.babylonjs.com/#RJ9YQD)

Перевод с версии [Standard-corridors.py](https://github.com/MakarovDs777/Procedural-generation-of-the-backrooms-python/blob/main/Trimesh/Standard-corridors.py)

[Backrooms on isurfaces (version 44 - Standard-corridors) | Babylon.js Playground](https://playground.babylonjs.com/#C5B2CU)

Тоже что и предыдущая только снизу вверх вертикально.

[Backrooms on isurfaces (version 45 - Standard-corridors vertical version) | Babylon.js Playground](https://playground.babylonjs.com/#BLXF9Y)

Теперь сделаем их много и случайно повернутыми на 360 градуссов.

[Backrooms on isurfaces (version 46 - Multiple Standard-corridors 360 degrees rotated version) | Babylon.js Playground](https://playground.babylonjs.com/#ZJV3SM#2)

Просто кубическое бруталиское пустое здание из острых углов.

[Backrooms on isurfaces (version 47 - Brutalist buildings) | Babylon.js Playground](https://playground.babylonjs.com/#LLLXHY)

Случайно расположенные и повернутые случайно на 360 градуссов пустые комнаты зданий.

[Backrooms on isurfaces (version 48 - Empty rooms 360 degrees rotated version) | Babylon.js Playground](https://playground.babylonjs.com/#43YAOT)

Кубические клетки разного размера.

[Backrooms on isurfaces (version 49 - Cubic cage of different sizes) | Babylon.js Playground](https://playground.babylonjs.com/#4BNW0Y)

Бесконечный гиперкуб с острыми гранями.

[Backrooms on isurfaces (version 50 - Endless hypercube trimesh version) | Babylon.js Playground](https://playground.babylonjs.com/#8I37KB#2)

Тоже что и 17 версия только с острыми углами комнат и гладким краями соединенний.

[Backrooms on isurfaces (version 51 - Single-storey poolrooms smooth XZ in One chunk pseudovoxels) | Babylon.js Playground](https://playground.babylonjs.com/#0RSVQX#2)

Хаос коридоров но только с острыми гранями.

[Backrooms on isurfaces (version 52 - Corridors-multi-storey-chaos-poolrooms pseudovoxels) | Babylon.js Playground](https://playground.babylonjs.com/#J9PA8Z)

Тоже что и 42 версия только бесконечная по XZ.

[Backrooms on isurfaces (version 53 - Vertical pillars from the very bottom to the very top endless XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#IRX5VI)

Тоже что и предыдущая только без прозрачности, и с одинаковым цветом везде.

[Backrooms on isurfaces (version 54 - Endless Moria XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#D38F76)

Тоже что и предыдущая только с коробками дырок от пуль.

[Backrooms on isurfaces (version 55 - Boxes of isurfaces with bullet holes XZ endless version) | Babylon.js Playground](https://playground.babylonjs.com/#GZU5RM)

Тоже что и Мория только с ровными полом, и потолком.

[Backrooms on isurfaces (version 56 - Endless Moria XZ version but smooth carpet and ceilings) | Babylon.js Playground](https://playground.babylonjs.com/#2M7TAV)

Бесконечная многоэтажная процедурно генерируемая Мория.

[Backrooms on isurfaces (version 57 - Endless Moria XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#UDN40B)

Бесконечные столбы.

[Backrooms on isurfaces (version 58 - Endless Pillars XYZ version) | Babylon.js Playground](https://playground.babylonjs.com/#MD2XDX)

Процедурный генератор водорослей.

[Backrooms on isurfaces (version 59 - Seaweed in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#93LIXU)

Водоросли только сверху вниз.

[Backrooms on isurfaces (version 60 - Seaweed in One chunk from top to bottom) | Babylon.js Playground](https://playground.babylonjs.com/#4E5JWV)

Водоросли только снизу вверх.

[Backrooms on isurfaces (version 61 - Seaweed in One chunk bottom-up) | Babylon.js Playground](https://playground.babylonjs.com/#WI5TU8)

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

Добавим поля телепорта.

[Backrooms in Babylon.js level 11 - The Endless Sity (Version 3) | Babylon.js Playground](https://playground.babylonjs.com/#6KLFTE)

## Бесконечное небо

Бэкрумс уровень бесконечное небо с бесконечно процедурно генерирумымм молниями.

[Backrooms in Babylon.js (Optional version - Endless sky with lightnings) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#V2MVHL)

Теперь нужно убрать молнии что-бы просто оставить процедурно генерируемый бесконечный туман.

[Backrooms in Babylon.js (Optional version - Endless sky) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#G14EV7)

Теперь сделаем бесконечно процедурно генерируемый туман с бесконечно процедруно генерируемым снегом.

[Backrooms in Babylon.js (Optional version - Endless sky with fog and snow) | Babylon.js Playground](https://playground.babylonjs.com/?inspectorv2=true#XSO03M)

## -9223372036854775808

Хотел сделать бесконечный океан глюка типа как уровень монохром как его чаще называют [Backrooms Level -9223372036854775808](https://sketchfab.com/3d-models/backrooms-level-9223372036854775808-5e0a01f01cf44cffacb7ae56750ea099), и сделал бесконечно процедурно генерируемые микро шумы:

[Endless procedurally generated micro noise | Babylon.js Playground](https://playground.babylonjs.com/#2AETZY#0)

Бесконечный океан цветного глитча первая версия.

[Backrooms in Babylon.js (Optional version - An endless ocean of colored foam) | Babylon.js Playground](https://playground.babylonjs.com/#NYGRIF)

Теперь мне нужно заставить их колебаться.

[Backrooms in Babylon.js (Optional version - Dancing thorns) | Babylon.js Playground](https://playground.babylonjs.com/#NH56YZ)

Но мне не нужно что-бы они танцевали нужно что-бы они флуктуировали.

[Backrooms in Babylon.js (Optional version - Endless fluctuating ocean of colored noise) | Babylon.js Playground](https://playground.babylonjs.com/#07SF66)

## Уровень - Бесконечное море цветного шума

Но вот теперь осталось лишь сделать бесконечную процедурно генерируемую плоскость цветного шума, и это уже похоже на уровень монохрома.

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

В этом дожде из матрице есть однозначно какой-то глубинный смысл только нужно понять какой... Ведь как известно там где высоко там снизу вселенная лишь многомерится меняя лишь эталон, и меру.

[Backrooms in Babylon.js (Optional version - The Matrix an endless library of words English version + Coordinate board) | Babylon.js Playground](https://playground.babylonjs.com/#5P5Z74#1)

Теперь заменим буквы на случайные слова, и сделаем бесконечную процедурную XZ версию.

## Уровень -1 000 007 Бесконечные небоскребы

Уровень бесконечных небоскребов – это -1 000 007 уровень в бэкрумсе, это уровень который я придумал по сути уровень представляет из себя огромное темное пустое пространство из которого выходят небоскребы различного типа, высоты, и ширины, расположенные друг от друга на различное расстояние. Предположительно уровень имеет бесконечную высоту, ширину, и длину, однако этого точно никто не знает. Попытки узнать, и установить, что находиться в нижнем темном пространстве, оканчивались неудачей, люди, и предметы, попадавшие туда просто пропадали из виду, и исчезали. Было замечены различные аномальные случаи, как целые небоскребы вырывались вверх, двигаясь с большой скоростью из нижнего темного пространства, и даже сталкиваясь тем самым с другими небоскребами, и также загадочно быстро исчезали проваливаясь туда, были замечены случаи как небоскребы стояли прямо на небе, генерировались на ходу, находились склеенными, налепленные друг на друга, состояли из городов, и имели бесконечную высоту. На уровне так же наблюдались различные атмосферные, и погодные явления, такие осадки как (дождь, морось, снег, град, гроза, зарница, огни святого Эльма, и т.д.) и так же сопровождаемые этими атмосферными явлениями наземные гидрометеоры (роса, иней, ледяные иглы, изморозь (кристаллическая и зернистая), твёрдый налёт, гололёд, гололедица), различные оптические явления (радуга, гало, мираж, солнечный столб, заря, глория), и даже такие явления как (ураган, смерч, шквал, вихрь, циклон, мгла, и т.д.) на уровне также есть смена дня и ночи, и ночью уровень становиться крайне опасным, он полностью окутывается тьмой и лишь тусклое освещение света из окон других небоскребов пробивается через темную дымку, а так же становиться наполнен различными сущностями, появляются голоса говорящий из неоткуда, а так же сопровождаемые этим слуховые, тактильные, и визуальные галлюцинации.

<img width="400" height="400" alt="Случайно_висящие_небоскрёбы_в_пустоте_и_повернуты_случайно" src="https://github.com/user-attachments/assets/3d3f2161-0be6-47e1-a38d-392752a93451" />

[Backrooms in Babylon.js level -1000007 - Infinite Skyscrapers (Version 0 - randomly hanging skyscrapers) | Babylon.js Playground](https://playground.babylonjs.com/#CEHD7X)

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве" src="https://github.com/user-attachments/assets/3ba4ba1b-6518-4401-b246-4b9613b6118c" />

[Backrooms in Babylon.js level -1000007 - Infinite Skyscrapers (Version 1 - One endless skyscraper) | Babylon.js Playground](https://playground.babylonjs.com/#ECB8UT)

<img width="400" height="400" alt="Небоскребы_из_небоскребов" src="https://github.com/user-attachments/assets/da8d5150-abeb-40f4-b249-5d59ff30caaa" />

<img width="400" height="400" alt="Бесконечные_небоскребы_до_определённой_высоты" src="https://github.com/user-attachments/assets/911796f1-ade9-417f-aff2-fb1ab65e7cbd" />

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве_2" src="https://github.com/user-attachments/assets/4a823e6b-b4ee-4e4b-874b-7ca403c37779" />

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве_1" src="https://github.com/user-attachments/assets/415fb38c-6415-4254-b4e0-d3175f9158e1" />

<img width="400" height="400" alt="Инфернальные_хрющёвки" src="https://github.com/user-attachments/assets/ea478c2a-070b-4e76-a420-32be9ec2c18f" />

## Уровень - Бесконечный ковёр 

Представляет из себя бесконечный жёлтый ковёр расположенный в пустоте полностью заполненный огромным ворсянистым рельефом словно увеличенном в тысячи раз размером ковром.

[Backrooms in Babylon.js level Endless fleecy carpet! (Version 0 - FINAL version) | Babylon.js Playground](https://playground.babylonjs.com/#4SJR2Q#1)

# Теории заговоров о бэкрумсе

Оглавление:

1.	Теории заговоров о бекрумсе
   
1.1.	Бэкрумс - это закулисье так что же сцена!?
  	
1.2.	Пропавшие без вести

1.3.	Квантовое туннелирование

1.4.	Центр закулисья

1.5.	Бэкрумс и симуляция вселенной.

1.6.	Бэкрумс – это случайная ошибка в исходном коде программы.

1.7.	Бэкрумс – это место выявления ошибок.

1.8.	Дата создания бэкрумса.

1.9.	Бэкрумс как место неиспользуемых моделей.

1.10.	Глючные объекты

1.11.	Сущностей не существует

1.12.	Типология уровней бэкрумса

1.13.	Другие входы в закулисье

1.14.	Первый человек в закулисье

1.15.	Граница бэкрумс

1.16.	Закулисье зависит от человека

1.17.	Эффект бабочки

1.18.	Гелиоцентрический бэкрумс

1.19.	Чёрные уровни

1.20.	Уровни матрёшки 

1.21.	Гипотеза о нестабильности, вызванной экспериментами A-Sync

1.22.	Бэкрумс это сущность которая пытается скопировать реальный мир

1.23.	Вход через осознанные сны

1.24.	Мы все были в закулисье

1.25.	Отличие экстерьера и интерьера

1.26.	Генерация уровней

1.27.	Край уровней закулисья

1.28.	Бэкрумс - это баг который был создан для того чтобы выбраться из бесконечной рекурсии симуляции вселенных.

## Бэкрумс - это закулисье так что же сцена!?

Если бэкрумс это закулисье, а вселенная это сцена — значит где-то должен существовать зрительный зал, должно быть зрительный зал — это потусторонний мир куда попадают после смерти где существуют боги и высшие силы которые наблюдают за нами, но они не видят то что происходит в закулисье должно быть бэкрумс скрыт от их глаз.
А если развить теорию дальше, то можно подумать, что бэкрумс это скорее оперный театр, чем просто театр, то можно сказать что есть ещё и ложи, бельэтажи, бенуары, галёрки, партеры и чем они являются можно только догадываться.

## Пропавшие без вести

Мы знаем, что ежегодно пропадает миллионы людей без вести, а самая страшное что многие из них не будут найдены может быть кто-то из них утонул в болоте, а кто-то с инсценировал свою смерть тем не менее многие склоняются к тому люди проваливаются в закулисье, и им остаётся лишь бродить по бесконечному лабиринту в надежде найти выход, которого нигде нет.

## Квантовое туннелированние
Это очень сложное явление в квантовой физике предполагается что у частиц есть некий барьер, который не дает другим частицам пройти через него, то есть если вы будете обладать достаточной энергией, то вы можете преодолеть барьер, и пройти сквозь неё как вы догадались так можно достичь noclip, и раз некоторые люди проваливаются сквозь текстуры нашего мира то это вполне можно объяснить явлением квантового тунеллирования.

## Центр закулисья 

Существует ли центр у закулисья? И что в нём находится?

## Бэкрумс – это ошибка в случайном коде программы.

Мы уже говорили о том, что бекрумс - это своего рода смоделированная альтернативная реальность, которая является продолжением идеи трилогии фильмов матрицы, но что, если я скажу вам, что если этот мир не был создан намеренно, а был ошибкой в исходном коде? На самом деле, это выглядит логично, потому что большинство уровней характеризуются странными вещами, которые не подчиняются законам физики, так что эта теория также может быть связана с центром подсобных помещений, где центр - это место, откуда вышла основная ошибка, которая повлияла на несколько строк кода, тем самым образовав подсобные помещения. И остается только догадываться что послужило причинной этой случайной ошибки.

## Бэкрумс – это место выявления ошибок.

При создание какой-либо программы всегда появляются ошибка после чего её исправляют, однако бывают такие случаи, когда причины не совсем понятны тогда приходится проводить опыты создавать различные условия, и варианты события дабы выстроить цепочку на пути к ответу, и как вы поняли если наш мир матрица, то таким местом выявления ошибок является закулисье это объясняет, то почему оно такое нестабильное, и неестественная 

## Дата создания бэкрумса.

Почему до вступление первого человека на мир жёлтых комнат не было известно абсолютно ничего? Либо закулисье было создано относительно недавно в течение последних 50 лет, ибо раньше этих интерьеров жёлтых обоев не могло существовать либо этот мир стар как наша вселенная, и существовала всегда тогда где-то должны быть его упоминания, и скорее всего они есть, есть во многих местах только в переработанном контексте как тот же рай и, ад, но скорее всего нам никогда не удастся найти ответ на этот вопрос…

## Бэкрумс заставляет вас взять на себя неиспользуемые модели.

Если закулисные комнаты действительно предназначены для загрузки реальности как предполагают некоторые, то возможно ли, что модели каждого человека, и животного так же могут располагаться в закулисье, то есть представьте, что пространство — это место всех текстур нашего мира где хранятся миллионы миллионы объектов человеческих тел, стоящих в т позе животных, и так далее, а что касается сущностей, обитающих в закулисных коридорах то возможно они созданы для охраны этого хранилища дабы случайно попавшие люди не сломали бы эту систему…

## Глючные объекты

В закулисье можно часто встретить странные объекты коими являются стулья они могу иметь необычные свойства что бы это не было взаимодействие с ними отправит вас на случайный уровень или даже выбросит в пустоту, их так же в очень редком случае возможно можно встретить и на Земле которые как вы поняли выбросит вас в бесконечные коридоры…

## Сущностей не существует

В оригинальном посте о закулисье нет не единого слова о том, что там кто-то обитает да есть упоминание о том, что вы можете кого-то услышать, однако это может быть лишь намёк на галлюцинации наша теория предполагает то что все сущности, о которых мы знаем не существуют ведь логический сам факт их существования вызывает множество вопросов, например, есть ли у них пищевая цепочка и как она устроена если у них она невозможна почему они находится именно в закулисье в месте которое является хламом не использованных локаций, и почему-то не одного из них нельзя встретить на Земле да и сама концепция лиминальных пространств никак не состыковывается с ними.

## Типология уровней бэкрумса

Уровни в бэкрумсе подразделятся на положительные уровни, и отрицательные уровни, а также на подуровни уровней, и аномальные уровни которые ни отрицательные, и не положительные словно Deep Web где есть сайты, которые есть, но они не индексируются поисковиком.

Но понимания того как на самом деле устроена типология уровне в закулисье до сих пор неизвестно.

## Другие входы в закулисье 

Самым распространённым способом попасть в закулисье конечно же является noclipping но на самом деле их огромное количество большинство из которых мы наверное ещё не знаем один из которых являются техника осознанного сновидения однако я могу вам рассказать ещё о некоторых способах как например игра в лифт известная в народе как ‘лифт в астрал’ возможно если лифт 9 здания прокатиться в определённой последовательности то он приедет в другой мир которым является закулисье, думаю не стоит останавливаться на этом методе ровно так же и на способе заключающемся в использование опасных, и запрещенных галлюциногенных веществ. 

## Первый человек в закулисье 	

Пожалей это тоже навсегда останется тайной точно так же как, как и с тем, когда было создано закулисье, и как минимум потому что время в нём течет совсем по-другому, а возможно оно вообще не зависит от него, мы лишь можем предполагать, как давно ступила нога человека ступил на мокрый ковер бесконечных коридоров, а возможно этот самый человек ещё жив.

## Граница бэкрумс 

Это теория говорит о том, что где-то во вселенной есть места куда не может добраться материя, и свет из-за чего мы никогда не сможем достичь этого потому что она просто недостижимо так называемая альтернативная реальность, которая возможно является закулисье не известно насколько массивным может быть объект тем не менее множество различных факторов говорит об этом как например большое количество далёких уровней, представляющих собой край закулисного мира, за которым находится лишь пустота.

## Закулисье зависит от человека

Мы имеем множество источников информации о закулисье от множество разных людей из разных частей света, и всё-таки есть одна вещь которая заставляет задуматься! Если попытаться выстроить общую картинку коридоров, то порой может выходить множество не состыковок, и если с нулевым более-менее одинаково, то остальные имеют разные представления почему это так происходит? Возможно закулисье зависти от каждого человека лично каждая новая локация выстраивается, и воспринимает по-разному если они вообще являются правдой, а не очередными галлюцинациями так, например, в базах данных каждый человек имел иную обстановку в частности пол из песка, земли, и покрыт туманом или травой, а у кого-то это был обычный холодный бетон.

## Эффект бабочки

Эффект бабочки — это свойства некоторых хаотичных систем, когда незначительное влияние на систему оказывает большие, и непредсказуемые последствия, в том числе в совершенно другом месте, когда в одном месте бабочка делает взмахи крыльев на другом происходит ураганы к закулисье это относится к тому факту что малейшие изменения на уровнях, могут изменить сам как уровень, так и само закулисье в целом.

## Гелиоцентрический бэкрумс

Согласно гелиоцентричной модели мира в центре всего находится планета Земля вокруг которой вращается всё остальное планеты другие звёзды, и так до бесконечности… Мы можем представить бэкрумс тоже как гелиоцентрическую модель мира где в самом центре некий недосягаемый центр глюк/глитч/ошибка которая породила всё этакий эпицентр абсолютного хаоса в котором бэкрумс становится настолько хаотичным, и непредсказуемым что уже никто никогда не сможет понять что-то там а чем дальше мы отходим от центра тем более наоборот мир становится всё более нормальным пока мы полностью не попадаем на самое последнее кольцо в котором просто бесконечная плоскость тянущиеся на бесконечное количество пространства, или же наоборот типа центр это оазис в пустыне а всё вокруг него бесконечный океан хаоса только не как какие-то ограниченные кольца определённого размера а скорее как неевклидовое пространство с положительной бесконечной кривизной где каждое кольцо бесконечно хотя может быть кольца имею и какие-то ограниченные размеры.

## Чёрные уровни

Существует легенда что в бэкрумсе существует чёрные уровни — это место куда можно попасть, но откуда уже невозможна выбраться этакая тюрьма для рецидивистов.

## Уровни матрёшки 

Уровень матрёшки — это те уровни где есть отдельный бэкрумс внутри бэкрумса этакая ошибка внутри ошибки.

## Гипотеза о нестабильности, вызванной экспериментами A-Sync

Также у меня есть небольшая гипотеза о нестабильности, вызванной экспериментами A-Sync. Суть идеи в том, что если представить обычную реальность в виде воздуха, покрытого слоем воды, то вода - это подсобные помещения. Мы, люди, - насекомые, летающие в воздухе. Обычно насекомые застревают в слое поверхностного натяжения между воздухом и водой, если насекомое падает в воду. Обычно это препятствует попаданию насекомого в воду (подсобные помещения). Учитывая силу тяжести, насекомое либо остается в пограничном слое, либо тонет в воде. Компания A-Sync создала сифон, проделав отверстие в межпространственном резервуаре для воды ниже естественного уровня воды. Создавая водовороты на поверхности воды, которые засасывают предметы с поверхности воды глубоко под воду вместе с закрученным столбом воздуха (реальность). Это то, что люди исследуют, этот искривленный пласт реальности, созданный межпространственным водоворотом. Вот почему единственный способ вернуться в реальный мир - это вернуться через портал A-Sync facility. Потому что именно там все течет.

## Бэкрумс – это сущность которая пытается скопировать реальный мир.

Знаешь мне иногда кажется, что где-то там в глубине бесконечности всех этих коридоров, помещений, и уровней обитает некое такое мистическая многомерная сверхъестественная сущность! И вот эта вот сущность для чего-то… Пытается дотянуться до материальности, до физической вселенной, пытается её объять, скопировать наш мир! Но раз за разом у неё ничего не получается, каждая её копия получается битой, и уродливой… Будто-бы она пытается собрать какую-то мозаику… Она проделала бесконечную дыру в пространстве, и времени… Заполнив её бесконечным невпопад случайно неправильно собранной мозаикой уродливых разбитых осколков нашей вселенной... Говорят, что бекрумс это глюк, ошибка в матрице вселенского мироздания… 

А для тех, кто здесь впервые объясняю - бекрумс это глюк реальности, сбой в матрице вселенского мироздания, ошибка! Которой не должно быть… сверхъестественное явление, и от него можно ожидать абсолютно всего чего угодно, так что будьте готовы ко всему законы по которым он существует, и функционирует вообще не поддается какому-либо описанию, объяснению, и логике… Все попытки описать какую-либо логику законов, по которым он существует претерпели крах. Сам факт его существования является невозможным в принципе он противоречит всем законам физики, он противоречит мироустройству всего сущего. Однако он существует каким-то загадочным образом, и это факт. 

## Вход через осознанные сны.

Осознанный сон отличается от обычного тем что в нём все происходящее вы осознаете, что вы спите, и можете контролировать всё происходящие, то есть делать во сне всё что захотите, и это действительно круто потому что таким образом можно бывать в абсолютно любых локациях, которые можно только себе представить делать всё что захочешь, и многое другое нет никаких ограничений пока не проснёшься.
Тебе лучше почитать в интернете статьи на эту тему ведь техника попадания в осознанный сон довольно сложна, и на вряд ли у тебя получится это сделать с первой попытки тем не менее ровно таким способом во сне вы можете оказаться в закулисье но нельзя быть полностью уверенным что вы в безопасности поскольку есть маленькая вероятность на яву проснутся в закулисье. 

## Мы все были в закулисье

Мы уже знакомы с таким явлением как лиминальнное пространство, а самое главное, что чувство ностальгии в основном вызывают именно картинки, а не видео тоже самое относиться к изображениям нулевого уровня возможно, что мы уже сотни раз были в этих местах когда-то давно, и возможно это так и есть все мы были в закулисье только воспоминания об этих местах хранятся очень глубоко в конце концов единственный способ восстановить память — это снова посетить эти локации.

## Отличие экстерьера от интерьера

Снаружи дом выглядит ненастоящим, как театральная декорация. Обратите внимание, что перед ним "кусты" из бумаги и дерева? Хотя внутри все выглядит как обычно. 
Моя теория заключается в том, что, когда портал был разрушен и открыт, какой бы инопланетный/искусственный интеллект/алгоритм ни отвечал за строительство подсобных помещений, он мог взять только часть информации с другой стороны портала и, следовательно, должен был создавать внешний вид дома с нуля, поэтому интерьер не соответствует внешнему виду.

## Генерация уровней

Многие теории предполагают, что закулисье это некая симуляция, запущенная на неком компьютере, и множество фактов подтверждают данное высказывание неевклидовое, и бесконечные свойства коридоров говорят о процедурных генерациях уровней, которые часто используются в многих уровней, например, на уровне 0 где, пройдя несколько метров в одном направлении, а возвращаясь обратно ты как будто-бы оказываешься совсем в другом месте это сделано для того чтобы снизить нагрузку сервера, и не забивать память компьютера а отсюда процедурные генерации вполне логичны алгоритм прост сначала создается прямоугольник игрового поля затем он рандомно делится на две части рекурсивно это проделывается несколько раз до некоторого предела потом в каждом прямоугольнике выбирается комната либо такого же размера либо чуть поменьше, в конец некоторые из них соединится коридорами не всё так идеально в этом мире а в закулисье так тем более поэтому не редко можно встретить баги, и ошибки в некоторых местах странные тупики или некорректно сгенерированный карьер.

## Край уровней закулисья

Та самая картинка из которой зародилась вся история гласит примерно о примерной площади жёлтых коридоров которой, и не совсем бесконечны 600 квадратных миль одиночества, и безумия нет не одной фотографии не одного очевидца или иного доказательства края закулисья, и видимо никогда не будет остаётся лишь гадать о том, как это выглядит пропасть в бесконечную пустоту или стена, однако отдаляясь всё дальше будет возникать всё больше багов и некорректных генераций прям как в майнкрафт где пройдя миллионы блоков игра ломается под собственным весом ровно по этой причине у вас не получится достичь границ мира ибо аномалии и точки nooclipe покончат с вашим путешествием раньше времени.

## Бэкрумс - это баг который был создан для того чтобы выбраться из бесконечной рекурсии симуляции вселенных.

Согласно этой теории, вселенная это компьютерная симуляция, которая была создана в компьютерной симуляции и так до бесконечности вплоть до самой первой симуляции вселенной, а бэкрумс это дыра проделанная в пространстве под текстурами нашей реальности, бесконечной рекурсии симуляции вселенных баг, который намеренно создало кто-то или что-то для того чтобы выйти за рамки бесконечности рекурсий симуляции вселенных, и попасть в реальную реальность, и чем ближе мы подходим к центру тем глубже мы погружаемся в бэкрумс тем более глючным, и лаганным он становиться… Остается только догадываться что расположено там в настоящей реальной реальности, должно быть это мир хаотичного хаоса – гиперкосмос в котором законы мироустройства настолько бесконечны сложны что бесконечно неописуемые, настолько хаотично хаотичный хаос что вызывает дикий ужас первородного мироздания вселенной перед истинной формой существование всего сущего.

## P.S.

Теперь это полноценное закулисное пространство! Возможно, кто-то придумает какие-то новые проекты, и проект будет развиваться.
