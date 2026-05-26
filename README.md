Наборы FPS игр бэкрумс в стиле свободного мира с бесконечной процедурной генерации включающий 147 кода(ов) созданные мной.

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

Кубаполостие в одном чанке.

[Backrooms on isurfaces (version 62 - Cubapolostie XZ version in One chunk) | Babylon.js Playground](https://playground.babylonjs.com/#SMUJY1)

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

# Мои уровни

Все эти уровни я придумал когда-то давно писал какие-то из них на фандоме закулисья потом ещё много где но их все удалили, и решили реалищовать и написать их все здесь.

## Уровень -1 000 007 Бесконечные небоскребы

Уровень бесконечных небоскребов – это -1 000 007 уровень в бэкрумсе, это уровень который я придумал по сути уровень представляет из себя огромное темное пустое пространство из которого выходят небоскребы различного типа, высоты, и ширины, расположенные друг от друга на различное расстояние. Предположительно уровень имеет бесконечную высоту, ширину, и длину, однако этого точно никто не знает. Попытки узнать, и установить, что находиться в нижнем темном пространстве, оканчивались неудачей, люди, и предметы, попадавшие туда просто пропадали из виду, и исчезали. Было замечены различные аномальные случаи, как целые небоскребы вырывались вверх, двигаясь с большой скоростью из нижнего темного пространства, и даже сталкиваясь тем самым с другими небоскребами, и также загадочно быстро исчезали проваливаясь туда, были замечены случаи как небоскребы стояли прямо на небе, генерировались на ходу, находились склеенными, налепленные друг на друга, состояли из городов, и имели бесконечную высоту. На уровне так же наблюдались различные атмосферные, и погодные явления, такие осадки как (дождь, морось, снег, град, гроза, зарница, огни святого Эльма, и т.д.) и так же сопровождаемые этими атмосферными явлениями наземные гидрометеоры (роса, иней, ледяные иглы, изморозь (кристаллическая и зернистая), твёрдый налёт, гололёд, гололедица), различные оптические явления (радуга, гало, мираж, солнечный столб, заря, глория), и даже такие явления как (ураган, смерч, шквал, вихрь, циклон, мгла, и т.д.) на уровне также есть смена дня и ночи, и ночью уровень становиться крайне опасным, он полностью окутывается тьмой и лишь тусклое освещение света из окон других небоскребов пробивается через темную дымку, а так же становиться наполнен различными сущностями, появляются голоса говорящий из неоткуда, а так же сопровождаемые этим слуховые, тактильные, и визуальные галлюцинации.

<img width="400" height="400" alt="Случайно_висящие_небоскрёбы_в_пустоте_и_повернуты_случайно" src="https://github.com/user-attachments/assets/3d3f2161-0be6-47e1-a38d-392752a93451" />

[Backrooms in Babylon.js level -1000007 - Infinite Skyscrapers (Version 0 - randomly hanging skyscrapers) | Babylon.js Playground](https://playground.babylonjs.com/#CEHD7X)

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве" src="https://github.com/user-attachments/assets/3ba4ba1b-6518-4401-b246-4b9613b6118c" />

[Backrooms in Babylon.js level -1000007 - Infinite Skyscrapers (Version 1 - One endless skyscraper) | Babylon.js Playground](https://playground.babylonjs.com/#ECB8UT)

<img width="400" height="400" alt="Небоскребы_из_небоскребов" src="https://github.com/user-attachments/assets/da8d5150-abeb-40f4-b249-5d59ff30caaa" />

[]()

<img width="400" height="400" alt="Бесконечные_небоскребы_до_определённой_высоты" src="https://github.com/user-attachments/assets/911796f1-ade9-417f-aff2-fb1ab65e7cbd" />

[]()

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве_2" src="https://github.com/user-attachments/assets/4a823e6b-b4ee-4e4b-874b-7ca403c37779" />

[]()

<img width="400" height="400" alt="Небоскрёб_в_пустом_пространстве_1" src="https://github.com/user-attachments/assets/415fb38c-6415-4254-b4e0-d3175f9158e1" />

[]()

<img width="400" height="400" alt="Инфернальные_хрющёвки" src="https://github.com/user-attachments/assets/ea478c2a-070b-4e76-a420-32be9ec2c18f" />

## Уровень - Бесконечный ковёр 

Представляет из себя бесконечный жёлтый ковёр расположенный в пустоте полностью заполненный огромным ворсянистым рельефом словно увеличенном в тысячи раз размером ковром.

[Backrooms in Babylon.js level Endless fleecy carpet! (Version 0 - FINAL version) | Babylon.js Playground](https://playground.babylonjs.com/#4SJR2Q#1)

## Уровень - Бесконечная гора

The Backrooms – Бесконечная гора  

Уровень Бесконечная гора – это 999 999 998 уровень в бэкрумсе, который представляет из себя бесконечную гору, уходящую бесконечно вверх, и бесконечно вниз в бескрайнем небе, расположение облаков, и космоса которого недостижимо, и на этой бесконечной горе растут джунгли, а также периодический можно встретить самые разные строения, и здания. 
 
Сущности:

{NO DATE}

Колонии и Аванпосты:

Центральной аванпост B.I.G находится в маяке на высоком утесе.

Входы и выходы:

Входы:

•	Noclipping, иногда может привести вас сюда.

•	Одна из дверей на уровне The Hub.

•	Имеется множество входов на этот уровень, так как попасть на этот уровень можно с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

Выходы:

•	Имеется множество выходов с этого уровня, так как выйти с этого уровня можно с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

[Backrooms in Babylon.js level Endless mountain (Version 0 - FINAL version) | Babylon.js Playground](https://playground.babylonjs.com/#IUM4RW#1)

## Уровень - Зона Долонгов

Зона Долонгов – это 82382383281238328 уровень в бекрумсе я его придумал, этот уровень представляет из себя локацию “Зона Долонгов” из советского мультфильма “Властелины времени” это бесконечный дырчатый красный лес когда смотрел в детстве, и до сих пор когда вспомниаю испытываю психатронные флешбеки когда комар кусает в шею в конце фильма пацана этого бедного.

[Backrooms in Babylon.js level Dolonge Zone (Version 0 - Endless XZ version) | Babylon.js Playground](https://playground.babylonjs.com/#96HADW)

## Уровень – ВЕЛИКИЕ ФРАКТАЛЫ БЕКРУМСА 

Великие фракталы бекрумса – это -88888888 уровень в бекрумсе, предположительно уровень имеет бесконечный размер в высоту, длину, и ширину, уровень представляет из себя пустое космическое пространство, в котором плавают различные виды фракталы имеющие различный размер, в высоту, длину, и ширину, фракталы могут быть радиусом в 1 метр, и даже размером с галактику, и больше… Фракталы имеют так же различную длину число звеньев генератора, и различное число сжимающего отображения трехмерной области. Самоподобие которых состоит из различных областей пространства, скопированных с разных уровней бекрумса различными формами областей, из всего периода времени которое в них происходило. 

Типы структур:
1.	Динамические фракталы - Имеют различную длину число звеньев генератора, и различное число сжимающего отображения трехмерной области, самоподобие которой состоит из какого-то случайного места случайного уровня в бекрумсе, самоподобие области скопированного пространства скопированы какой-то случайной фигурой, будь то треугольник, многогранник, или просто хаотичная аморфная фигура.
2.	Хаотичные фракталы - При каждой последующей последовательности итерации число звеньев генератора, их случайное место, случайный уровень, размер самоподобия формы скопированной области пространства, самоподобие формы скопированной области пространства, число, и размер сжимающего отображения трехмерной области - меняется. Имеют различный размер, в высоту, длину, и ширину.
3.	Стохастичные фракталы - Имеют различную длину число звеньев генератора, различное число сжимающего отображения трехмерной области, самоподобие состоит из какого-то случайного места случайного уровня в бекрумсе, самоподобие скопированного пространства являются комбинацией, случайного числа различных скопированных областей с различных мест, и уровней бекрумса, скопированных какой-то случайной формой, будь то треугольник, многогранник, или просто хаотичная аморфная фигура.
4.	Аморфная структура – Является хаотично скрепленной структурной случайного размера, состоящей из различных областей, скопированных с различных мест, и уровней бекрумса, каждая скопированная область которой скопирована какой-то случайной формой, будь то треугольник, многогранник, или просто хаотичная аморфная фигура.
5.	Неизведанные структуры - Иногда разные фракталы, и структуры могут генерировать в друг друга, образуя новые ранее неизведанные структуры. А также иногда структуры, и фракталы могут сталкиваться с друг другом разлетаясь на множество различных кусков, и даже соединяясь таким образом с друг другом образую тем самым новые неизведанные структуры.

<img width="400" height="400" alt="1" src="https://github.com/user-attachments/assets/768a5d24-9a2b-481f-965b-a3527fe802ca" />

[Backrooms in Babylon.js level The great backrooms fractals (Version 0 - Lines fractals) | Babylon.js Playground](https://playground.babylonjs.com/#Z62TPJ)

<img width="400" height="400" alt="2" src="https://github.com/user-attachments/assets/94c028a8-32df-4e56-b3ba-6464837f8467" />

[]()

<img width="400" height="400" alt="3" src="https://github.com/user-attachments/assets/485a7ddd-1cc9-4330-8d4c-bcc542c8d5f8" />

[]()

<img width="400" height="400" alt="4" src="https://github.com/user-attachments/assets/fd7aede4-22e3-4b71-a8b7-8fbf29c604be" />

[]()

<img width="400" height="400" alt="5" src="https://github.com/user-attachments/assets/94864373-7458-4642-ba2a-d5a8105f9f8c" />

[]()

<img width="400" height="400" alt="6" src="https://github.com/user-attachments/assets/aed7e2af-fc11-456c-8a02-0054a380106b" />

[]()

<img width="400" height="400" alt="7" src="https://github.com/user-attachments/assets/eae6add1-1d50-411a-9c6e-f74747096ea0" />

Изображения на этих картинках, это огромные фракталы в миллиарды километров диаметром состоящие их помещений, и коридоров с нетривиальной геометрией,только можете себе представьте это!! ( ͡ʘ ͜ʖ ͡ʘ)

Типы зон:

Каждая структура-фрактал состоит из зон случайного размера, каждая из которых работает по определенным правилам, и каждый фрактал-структура плавно переходит в друг друга.
1.	Белая зона – Это обычная зона, в ней действует привычные нам законы физики, в ней не может происходить ничего паранормального, и сверхъестественного.
2.	Красная зона – Полный антипод белой, законы физики здесь работаю по-другому, течение времени в таких областях может меняться, свет, материя, электромагнитное излучение, может браться из неоткуда, гравитация в таких областях может быть хаотичной, и притяжение гравитации может быть то от потолка, то от пола, а также меняться с течением времени, и т.д.
3.	Черная зона – Это просто пустые территории, разного размера, лишённые каких-либо структур, и фракталов.
   
Сущности:

Сущности очень распространены на этом уровне, особенно в открытых частях, поэтому избегайте больших открытых пространств. На уровне обитают все сущности со всех уровней, так как уровень представляет из себя нарезку изо всех областей пространства всех уровней из которых созданы фракталы, но из-за большой монструозности уровня, и раскиданности пространств встретиться с ними довольно трудно.

Колонии и Аванпосты:

Было предпринято множество попыток сформировать колонии на этом уровне, но все они потерпели неудачу из-за суровой природы этого уровня. В результате уровень был заброшен. Однако некоторые из заброшенных аванпостов все еще можно найти, а в некоторых могут быть припасы, но они, скорее всего, будут пустыми или содержат незначительное количество.

Входы и выходы:

Входы
•	Noclipping, иногда может привести вас сюда.
•	Одна из дверей на уровне The Hub.
•	Имеется множество входов на этот уровень, так как этот уровень является склейкой разных мест, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

Выходы
•	Имеется множество выходов с этого уровеня, так как этот уровень является склейкой разных мест, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

## The Backrooms – УРОВЕНЬ СИНГУЛЯРНОСТЬ ХАОСА

Сингулярность хаоса – это -9999999999999999999 уровень в бекрумсе, представляет из себя бесконечное неевклидовое пространство с положительной кривизной в самом центре которого находиться гигантская сфера диаметром -9999999999999999999 километров в которой происходит абсолютное применение всех всевозможных существующих вещей, ко всем всевозможным существующим вещам всеми возможными способами. Как правило достичь центра сингулярности хаоса невозможно, в силу равной бесконечной удаленности от 0 точки координаты аппликат по прямой линии, и чем ближе мы приближаемся к центру, тем больше применений от всего ко всему всеми способами происходит, и тем быстрее по экспоненте мы падаем к центру.

[Backrooms in Babylon.js level The Singularity of Chaos (Version 0 - By fragmented version) | Babylon.js Playground](https://playground.babylonjs.com/#0MXQO1)


[Backrooms in Babylon.js level The Singularity of Chaos (Version 1 - Not animation) | Babylon.js Playground](https://playground.babylonjs.com/#6MAU8Y)


[Backrooms in Babylon.js level The Singularity of Chaos (Version 2 - Final version) | Babylon.js Playground](https://playground.babylonjs.com/#G9508O)

Сущности:

{NO DATE}

Колонии и Аванпосты:

{NO DATE}

Входы и выходы:

Входы

•	Имеется множество входов на этот уровень.

Выходы

•	Имеется множество выходов с этого уровня.

## Уровень космических шаров

Уровень космических шаров – это -1 000 000 уровень в бекрумсе, уровень представляет из себя огромное темное пустое пространство на котором (предположительно) расположено бесконечное количество гигантских размеров шарообразных металлических структур как правило находящихся в одной плоскости пространства, размеры которых варьируются от звёзд размером с солнце до целых галактик, и больше.

[Backrooms in Babylon.js level The Space Spheres (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#SGP0N9)

##  The Backrooms – УРОВЕНЬ “ВЕЧНЫЙ ПУТЬ”

Уровень “Вечный путь” - это -7629888 уровень в бекрумсе, уровень представляет из себя пустыню, на которой расположена дорога как на картинке, где на самом вверху небо постоянно изменяется каждую секунду. 

[Backrooms in Babylon.js level The Endless Way (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#87JUU0)
 
Сущности:

{NO DATE}

Колонии и Аванпосты:

{NO DATE}

Входы и выходы

Входы

•	Noclipping, иногда может привести вас сюда.

•	Одна из дверей на уровне The Hub.

•	Имеется множество входов, но эти входы могут появляется, и так же загадочно исчезать, так же на этот уровень можно попасть с уровня 88888888, так как этот уровень является бесконечной склейкой психоделических переживаний, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

Выходы

•	Имеется множество выходов с этого уровня, так как этот уровень является бесконечным психоделическим сновидением. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

## Уровень - “ДОЛИНА ПЛАСТИКА”

Вы никогда не задумывались ли о том что если пробит фальшивый купол звёздного неба в бэкрумс что там будет?! Если попытаться найти в красной зоне небесный купол, и попытаться его пробить можно попасть на огромное бесконечное пространство заполненное странными сюриалистческими структурами...

Уровень “Долина пластика” - это 111000 уровень в бекрумсе, уровень представляет из себя холмистое пространство, полностью состоящие из скользкого пластика белого цвета и небо вместо которое постоянное освещенное светом белое пространство, на котором время от времени встречаются сюрреалистичные строения, состоящие полностью из белого пластика.

[Backrooms in Babylon.js level The Valley of Plastic (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#TY4OWN)

Сущности

Колонии и Аванпосты

{NO DATE}

Входы и выходы

Входы

•	Noclipping, иногда может привести вас сюда.

•	Одна из дверей на уровне [The Hub](https://backrooms.fandom.com/wiki/The_Hub).

•	Имеется множество входов, но эти входы могут появляется, и так же загадочно исчезать, так же на этот уровень можно попасть с уровня 88888888, так как этот уровень является бесконечной склейкой психоделических переживаний, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.
Выходы

•	Имеется множество выходов с этого уровня, так как этот уровень является бесконечным психоделическим сновидением. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

## ДОЛИНА КВАНТОВОЙ ПЕНЫ 

<img width="400" height="400" alt="QuantumFoaValley" src="https://github.com/user-attachments/assets/8b2b4f0b-ea70-493d-b366-d487eef1f309" />

Сущности

{NO DATE}

Колонии и Аванпосты

{NO DATE}

Входы и выходы

Входы
•	Noclipping, иногда может привести вас сюда.
•	Одна из дверей на уровне The Hub.
•	Имеется множество входов на этот уровень, так как этот уровень является склейкой разных мест, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

Выходы
•	Имеется множество выходов с этого уровня, так как этот уровень является склейкой разных мест, с различных уровней в бекрумсе. И поэтому остерегайтесь опасностей, здесь очень легко заблудиться.

[Backrooms in Babylon.js level The Valley of Quantum foam (Version 0 - Valley of the Lunar Craters) | Babylon.js Playground](https://playground.babylonjs.com/#11UL9H)

Теперь нужно все параметры GUI из квантовой пены [MakarovDs777/Quantum-foam-generator-online-on-babylon.js](https://github.com/MakarovDs777/Quantum-foam-generator-online-on-babylon.js)

[Backrooms in Babylon.js level The Valley of Quantum foam (Version 1 - Final version) | Babylon.js Playground](https://playground.babylonjs.com/#BP5V9R)

## The Backrooms – Имплозия 

Это -112 загадочный уровень в бекрумсе, уровень представляет из себя пространство - заполненное коридорами, комнатами, и помещениями по мере движение в котором изменяется само окружение этого уровне, комнаты, помещения, коридоры, так по мере движения человека или объекта могут перемещаться, сжиматься, растягивать, удлиняться, утолщаться, утончатся, становиться выпуклым, в общем принимать самую разнообразную форму - стены, потолок, пол, и т.д. Так было замечено что по мере движения в этом уровне менялся сам материал из которого состоит уровень. Поэтому исследования уровня затрудненно так как топологию карты уровня составит из-за этого крайне тяжело - уровень остается самым загадочным во всем бекрумсе.

Сущности

{NO DATE}

Колонии и Аванпосты

{NO DATE}

Входы и выходы

Входы

•	{NO DATE}

Выходы

•	{NO DATE}

Сначала сделаем случайное растягивание стен по мере движения камеры.

[Backrooms in Babylon.js level The Impluzia (Version 0 - Accidental stretching of walls) | Babylon.js Playground](https://playground.babylonjs.com/#1HS12C)

Теперь сделаем это с полом, лампами, потолком, и получится нужная версия.

[Backrooms in Babylon.js level The Impluzia (Version 1 - Final version) | Babylon.js Playground](https://playground.babylonjs.com/#GIXUAO)

Короче в любом случае это интереснная идея для развития!

## The Backrooms – ОКЕАН ВОЗДУШНЫХ ШАРОВ

Представляет из себя бесконечный в глубину, и ширину бассейн, неровно полностью заполненный различными видами воздушных шаров.

[Backrooms in Babylon.js level Ocean of balls (Version 0) | Babylon.js Playground](https://playground.babylonjs.com/#ETZVJH)

## The Backrooms – ОКЕАН КОНФЕТ

Представляет из себя бесконечный в глубину, и ширину бассейн, неровно полностью заполненный различными видами конфет.

[Backrooms in Babylon.js level Ocean of sweets (Version 0)](https://playground.babylonjs.com/#10NOYK)

## The Backrooms – Пространство лифтов 

Пространство лифтов – это -100000 уровень в бекрумсе, уровень представляет из себя огромное темное пустое пространство куда сходятся огромное количество различных шахт лифтов из разных уровней бекрумса, и на котором расположено множество различных лифтов, на уровне постоянно существует нулевая температура по цельсию. Какие-то лифты идут далеко вниз, переходя на другие уровни, некоторые шахты лифты просто обрываться в пустоту, а некоторые шахты лифтов хаотично завихряются идя куда-то вниз, неизвестно куда, и даже хаотично запутываться вместе с друг другом. 

[![Prostranstvo-Liftov.jpg](https://i.postimg.cc/xTTLwQF0/Prostranstvo-Liftov.jpg)](https://postimg.cc/QVwB723P)

Сущности:

{NO DATE}

Колонии и Аванпосты:

{NO DATE}

Входы и выходы:

Входы:

•	Имеется множество входов на этот уровень, так как этот уровень является местом всех лифтов со всех уровней

Выходы:

•	Имеется множество выходов с этого уровня, так как этот уровень является местом всех лифтов со всех уровней

[Backrooms in Babylon.js level Elevators Space (Version 0 - Endless random cropped posts) | Babylon.js Playground](https://playground.babylonjs.com/#O187Z7)

# Теории заговоров о бэкрумсе

Оглавление:

0.	Старое Солнце
   
1.	Бэкрумс - это закулисье так что же сцена!?
  	
2.	Пропавшие без вести

3.	Квантовое туннелирование

4.	Кем или чем является Натюрморт?

5.	Бэкрумс и симуляция вселенной.

6.	Бэкрумс – это случайная ошибка в исходном коде программы.

7.	Бэкрумс – это место выявления ошибок.

8.	Дата создания бэкрумса.

9.	Бэкрумс как место неиспользуемых моделей.

10.	Глючные объекты

11.	Сущностей не существует

12.	Типология уровней бэкрумса

13.	Другие входы в закулисье

14.	Первый человек в закулисье

15.	Граница бэкрумс

16.	Закулисье зависит от человека

17.	Эффект бабочки

18.	Гелиоцентрический бэкрумс

19.	Чёрные уровни

20.	Уровни матрёшки 

21.	Гипотеза о нестабильности, вызванной экспериментами A-Sync

22.	Бэкрумс это место которое пытается копировать реальный мир

23.	Вход через осознанные сны

24.	Мы все были в закулисье

25.	Отличие экстерьера и интерьера

26.	Генерация уровней

27.	Край уровней закулисья

28. Теория об агрессивности закулисья

29. Бэкрумс - это баг который был создан для того чтобы выбраться из бесконечной рекурсии симуляции вселенных.

30. Бэкрумс это сущность которая пытается скопировать реальный мир

31. Центр закулисья

## Старое Солнце

<img width="487" height="487" alt="Сохраненное изображение 2026-5-26_14-55-9 705" src="https://github.com/user-attachments/assets/202c14fd-da40-4da6-a678-942787646b31" />

И вот мы подошли к этому моменту с тех пор как мы оказались в бэкрумсе мы снова, и снова видим изображения Солнца небесная карта из [домашнего видео](https://www.youtube.com/watch?v=Kq6l9yCO9rI&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=16&pp=iAQB) которая прикрепленна к фильму [Found Footage 2](https://www.youtube.com/watch?v=sA5PxGHqpTo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=15&pp=iAQB0gcJCQYLAYcqIYzv) которую вы видели во вступлении где есть картина которую видит главный герой [Found Footage 2](https://www.youtube.com/watch?v=sA5PxGHqpTo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=15&pp=iAQB0gcJCQYLAYcqIYzv) видит а потом когда вы смотрите другое видео то видите то эта картина висела в другой гостиной - Итак моя основаня догадка и теория таковы я хочу обсудить что мы уже видели концовку и о том какой может быть эта концовка, и как она связана с Солнцем я считаю что Солнце может давать нам жизнь так и отбирать её это ограниченный источние энергии но для человечества он может казаться бесконечным итак если вернуться в далёкое прошлое к [Pitfalls](https://www.youtube.com/watch?v=0XwlWXtpaCM&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=10&pp=iAQB) одному из моих любимых эпизодов то бедный Марвин несчастный человек он ечрез многое прошел, и я искрене надеюсь что ему найдется хоть какое-то утешение так ему пришлось не легко так вот в [Pitfalls](https://www.youtube.com/watch?v=0XwlWXtpaCM&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=10&pp=iAQB) он проваливается в дыру до этого произошло кое что важное дверь открывается и мы видим зелёный свет помните этот момент!? Всегда помните о зелёном свете никогда не забываёте о нём это провод источника этого света это связанно с Солнцем у нас есть подовдные камни Марвин проваливается попадает во вторичную зона затем в красную зону, у нас есть карсные районы где всё вокруг красное мы подтвирдили что этот треск связан с попадание солнечной волны в спутник, он звучит как [whistler Mode Waves 2 - Johns Hopkins Applied Physics Laboratory (Captured by Nasa's Parker Solar Probe which flew straight into the sun's)](https://soundcloud.com/jhu-apl/psp-whistler-mode-waves-2) corona итак у нас есть красный свет знаете когда слышишь этот треск и когда понмаешь что это не человек и это происходит то это очень странно, итак вы слышите треск и это подтверждает что мы имеем дело с чем-то космическим если пресмотреть к красным света то можно увидеть звёзды и пустое пространство, и сейчас мы переёдем к [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) а что мы выяснили Рави так зовут главного героя [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) это сокращенного имя переводится Рави с индийского хинди как Солнце, и по всему видео [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) разбросанны плакаты с улыбающимся Солнцем оно упомниается в самых разных ввида, формах и так далее... А потом появляются красные города это что-то потрясающие потому что это не просто красные район в [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) это не проосто какие то квартал а целые небоскрёбы в космосе это безумие! Даже у Рави самая понятная реакция на то что он видит вокруг себя даже знак у дороги это момент из разряда чё за чёрт мы слышим тот самый звук а ещё эти районы ну когда он в конце умирает камера гаснет, и всё такое мы слшыим в конце скрипичную музыку вся это сцена просто потрясающая есть ещё один трогательный момент в [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) поднимается тема путешествий во времени где мы видим плакат с надписью 2022 что является самым отдаленым моментом в видео Кейна Пикселя это просто безумие мы в полное заднице ещё один пример путешествия во времени Питер Тенчь переносится в будущем что заканчивается катастрофический я не знаю жив ли он но факт что он подзакальзнулися, и умер ударвшись об камень вот так совпадение! Откуда взялся этот камень знаете я буду это повторять это просто очень кстати но как бы то ни было он перенёся в будущие и увидел новый центр управление, и тут всё пошло на перекосяк но самое важное что путешествия во времени существую в находках, или что я хочу обсудить карманы это места из разных временных отрезках в находках есть концепция что Солнце было перенсенно из [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv), [Found Footage 2](https://www.youtube.com/watch?v=sA5PxGHqpTo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=15&pp=iAQB0gcJCQYLAYcqIYzv), и домашнего видео которое к ним прилагается а так же из ловушек [Pitfalls](https://www.youtube.com/watch?v=0XwlWXtpaCM&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=10&pp=iAQB), и так о чём это нам говорит мне было очевидно о том как в комнатх отображались красные районы что-то не так всё было неправильно всё выглядело странно вверх ногами не на своём месте, и конечно небо с ними было всё не так хотя небо было просто ясно звёзды казалсись больше чем обычно как будто мы находимся в космической станции понимиает? Не на земле! И то как изображенно космическое небо это наталкнуло меня на мысль мы уже знаем каким был финал мы это видели, и финал не самое важное во всей этой истории, дойти до конца не цель всё это истории я считаю что финал это инструмент который позволяет расказать историю так что финал это не совсем финал я искренне вверю что солнце сыграет главную роль в гибели человечества но произойдет это очень, очень, очень не скоро хорошо что если закулисье введёт за пределы конца? Что если они ввидут из будущего за пределы конца, и что если из нашего настоящего и прошлого объеденяя их воединно, и тогда мы получим безумный мир в котором нет смысла вы знаете что такое бэкрумс в тот же день когда Иван Бек подписал контракт произошел вспышка зелёного света, и снова появлился этот зелёный свет который был в конце [Found Footage 2](https://www.youtube.com/watch?v=sA5PxGHqpTo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=15&pp=iAQB0gcJCQYLAYcqIYzv) я думаю что зелённый свет это расширение это похоже на процесс печати но дело в том что это происходило за пределами бэкрумса это случилось с Иваном Бэком, и что же там чёрт побери произошел это загадка ну а мы будем считать что это был момент когда солнечная буря запустил процесс который начался задолго до того как до создания портотипа которую мы видели в предыдущих сериях итак мы возвращем в 1970 значит Иван с тех пор занимался своими эксперементами хорошо значит на этот раз во многих проблемах виновато Солнце возможно именно солнечная вспышка, и солнечные волны, и стали толчком который который, и запустил весь процесс вот почему мы слышим всё это в Found Footage звук треска в красных районах, и всё такое итак мы упомнялуи переполнение Found Footage 2 подвдоные камни, и всё остальное что связанно с красными районами , зелённый свет, изображение Солнце, и [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) теперь я расскажу о том что было концом историю но я думаю что это был не конец истории или лишь часть которая станет концом всец истории я считаю что Солнце ограниченно это огранчиенный источник энергии понимаете но для человеской цивилизации для нас с нашим ничтожным существованием во вселенной нам кажется бесконечным но в конце концов солнце умрёт, и этот источник энергии питает всё закулисье при осмотре плитки в том видео [Backrooms - Lighting and Tile Survey](https://www.youtube.com/watch?v=DSWUEmJDglw&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=20&t=77s&pp=iAQB) становится ясно что все эти лампы их источник света работают бесконечно по крайне мере для нас никто не знаете откуда берется энергия это что-то из области фантастики вы знаете что оно включается даже когда его отключают лампы работают сами по себе здесь всё указывается знает на какой-то необочный источник энергии поэтому я твердо убежден что закулисье питается от Солнца это то что мы видим так оно и продолжает штамповать, копировать, и вставлять но происходит то что назвается эффектом ксеркса что происходит когда вы копируете копию копии, и ещё одну копию копии всё становится ещё более искаженным знаете это в конце концов выглядет ужасным так и происходит здесь кроме того у него проблемы с визуализацией потому что оно берёт данные из временной линии где нет солцне где не этого источника энергии где нет мира а что происходит с Солнцем когда оно умирает оно превращается в красного гиганта и поглощает всё вокруг количество энергии веделяемое Солнцем огромное оно расширяется поглащая всё вокруг количества тепла и свет проосто невероятнно оно будет расширятся и захватит все планеты что-бы мы увидели красное солнце в небе запомните это разу 'Красное Солнце в небе', и освещение та съемка как бы намекает мы не знаем откда берётся это энергия но она походу бесконечна, и будем работать вечно что ещё может быть почти бесконечым источником энергии? Но оно продолжает копироватьи захватывать пространство потому что само пространство бесконечно коруг нет нас другого пространство которое было бы решимо бесконечным как космос Async называет его A-Space это очень точное замечение но они точно знает о космосе, и ещё эта камера которая появляется в найденных плёнках падая с неба это совсем другое оно возвращется в реальность из бэкрумса итак у нас теория о красном Солнце верно мы предпологаем что Солнце в конце концов погаснет а в бэкрумсе нет понятия времени но оно продолжает копировать верно!? Но оно черпает энергию из места где ни данных ни энергии но как тогда оно само себе питает? То есть если оно постоянно пытается вытягивать что-то из разных областей как будто из Швейцарского сыра потому что там много дыра понимаете люди проваливаются в эти дыры, и происходит вся эта хрень то есть это просто не то что мы можем понять, и я не думаю что мы должны это понимать но по сути происходит что-то такое что закулисье продолжает копировать, копировать, и вытягивать энергию из настоящего, и прошлого понимаете из того что было в прошлом когда у него была такая возможность но оно всё равно заглядывает в будущие но потом оно как бы смешивает всё воединно и, не может понять что к чему потому что в одном случае Земли здесь а в другом нет понимаете поэтому, и в итоге появляются такие странные районы с таким красным цветом, и таким вибрирующим звуком Солнечных волн потому что оно так близко к нам знаете как будто в этот момент в этом снимке всё вот-вот исчезнет, теперь когда мы думает о красном Солнце как о части концовки мы видим то что у нас было перед глазами вот тот статичный тупик который в каком-то смысле стал нам ответом на вопрос так вот мы все гадали что же там за дверью перед зелёным светом в [Pitfalls](https://www.youtube.com/watch?v=0XwlWXtpaCM&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=10&pp=iAQB) таким же как в [Found Footage 2](https://www.youtube.com/watch?v=sA5PxGHqpTo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=15&pp=iAQB0gcJCQYLAYcqIYzv), и во всех остальных он повсюду если посмотреть закулисье он будете везде потому что закулисье постоянно что-то печтаете постоянно что-то создает верно? Теперь я всё понял то что было в ловушках действительно связанно с временными рамками в этот момент что-то происходило, и мы это упустили, и к чему это привело? Это то что мы увидели в статическом тупике так что помимо что это связанно с нехваткой времени было совершенно очевидно что зелённый свет загарался когда возникали препятствия! Пернесёмся в сатический тупик мы заходим внутрь камера осматривается и тут что-то бросается в глаза я говорю о том что происходит с обоям чего мы раньше не видели я не видел что-бы обои так себя вели разве что в [Pitfalls](https://www.youtube.com/watch?v=0XwlWXtpaCM&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=10&pp=iAQB) где некоторые стены, и всё остальное как будто растянуто линии идут поперёк потому что изображение неполное незнаю знаком ли вам этот термин но это назвается наложеннием текстуры итак как работает наложение текстуры когда пиксель и цвет отрисовывается доходит до края пикселя, и чего-то подобного, и возможно после это ничего не может быть отрисованно он просто растикается по оставшиеся части области потому что уже просто не на чего наложится вот и всё верно? То есть мы видим что в комнатах как бы говорят ну я незнаю что ещё с этим делать, и просто зажимаю текстуру, и всё готово! Иногда это выглядело очень не однородно знаете как будто в нём проглядывали обои а потом всё остальное пространство было как будто бы с этими прямыми линиями по всему коридору а потом когда вы проходите дальше вы видет этот странный участок вы видите эти углубления по всюду были объекты которые как бы наполовину были прорисованны незнаю может это были упавшие предметы или что-то что бэкрумс пытался прорисовать оно говорило ну мне больше нечего делать так что я просто сделаю это кое как понимаете, и ещё там был такой милый белый стул на холме в самом конце и ещё стол который был наполовину в стене, там даже был мяч который наполовину торчал из стены по сути вся это секция это провал в попытке создать иллюзию реальности это провал в попытке создать иллюзию реальности будто-то игра начинает понимать что у неё нехватает данных, и ей приходится делать то что она может то есть она не понимаете то что происходит ткакая ситуация когда ничего не поделаешь она может делать только так копируя, и вставляя то что у неё есть а знаете оно работает с тем что у неё осталось а что неё осталось? У неё остались искаженные участки тех мест которые оно пытается воспроизвести так что я рассматрваю статичный тупик как доказательство того что бэкрумс несправляется с копированием не может скопировать всё как надо, и это первый признак то чтого что бэкрумс начинаете терять силу в тоё или иной форме потому что копирует слишком далеко вперед понимаете? Знаете если оно черпаете энергию там где нет ни Солнца, ни Земли, или этих конкретных учатков больше несуществует то оно может не справиться с копирование из-за самого принципа путешествия во времени так что это ещё одна возможная причина это не аксиома! Итак мы поговорили о статическом тупике это своего рода неудавшиеся попытка копирование рендринга зелёный свет не сделал того что должен был, и это произошло довольно рано это случилась не в конец [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) это произошло довольно рано зелённый свет появлился довольно ранно даже в [Found Footage 1](https://www.youtube.com/watch?v=H4dGpz6cnHo&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=1&pp=iAQB) так что Кейн начал свою работу довольно ранно итак последний пункт мы поговорили о теории красного Солнце, и о том что это может означать конец Земли, конец вселенной, и конец так сказать его бесконченой силы потому что понимате человечество не прживёт достаточно долго мы не доживём до того момент как Солнце перестанет существовать но Земля останется, и всё что мы построили на ней продолжить стоять когда нас уже давно не будет когда мы перестанем сущестовавать и мы исчезнем наши руины останутся в бэкрумсе а серверный продолжат копировать всё снова, и снова а ещё вот что помните как Кейн говорил нам что мол Async не злодей, и это чистая првда они не похожи на злодеев которые крутят усы настоящие и это чистая правда настоящое зло это время, и сила Солнца вот что по настоящему страшнно время это как бы тот кто наблюдает за всем даже за самим Солнцем но да Иван для меня загадка потому мы знаем что он где-то рядом но что он делает почему он так не уловим для нас всех, и для всех остальных кто учавствует в этой истории? И чем он занимался в 1970? И что с ним случлось ведь это случилось не в бэкрумс а в нашем мире этот контракт был заключён в оффисе который находися за перделами бэкрумс но мы видим что там горит зелённый свет прежде всего даватйе обратимся к последнем 8 трекам третего тома итак мы смотрим последние 8 тректов третего тома я держу его в руках вполне очевидно я думаю что это нам говорит о чём то важном порог мы знаем что такое порог это дверь в бэкрумс который создал Async возможно что это относится, и ко всем областям куда можно попасть без загрузки к чему-то запретному мы часто слышим о море даже о закате над морем о тмо что море поглащает всё знаете тьма которая поглощает всё можно сказать что космос это тоже запретное место это ещё и метафора которая означает что преодолев порог мы прыгнули в бездну а сразу после этого идёт трэк [Rest Forever in This Dead End](https://www.youtube.com/watch?v=1h2fdKzNS1o&list=OLAK5uy_kh-DA5qCCtBrGDbhOMeXmZ2_Kn9DX3F0k&index=8) один из самых любимых в это альбоме там есть такая классная гитарная партия она по сути мы застряли вечно покоится в этом тупике но кто или что будет покоится в нём вечно? Может сам бэкрумс будет вечно покоится в этом тупике потому что оно открыто оно живо оно делает своё дело но оно обреченно, и я незнаю что бы это могло бы разве что только кроме человечества которое покоется в этом тупике в который мы сами себя загнали после того как открыли ящик пандоры после этого у нас будет [Натюрморт](https://www.youtube.com/watch?v=CxDjUTcaCDo&list=OLAK5uy_kh-DA5qCCtBrGDbhOMeXmZ2_Kn9DX3F0k&index=10), и [Натюрморт 2](https://www.youtube.com/watch?v=7qqUHdLAX-8&list=OLAK5uy_kh-DA5qCCtBrGDbhOMeXmZ2_Kn9DX3F0k&index=10) это один из наших любимых треков я знаю что многим из нас это нравится мне тоже это нравится эхто безусловно можно рассматривать как нечто мёртвое ты знаешь существует много произведений исскуства о чём-то умершем но ты понимаешь что касается искусства так что это не обязательно должно быть идеей исскуства просто что-то мёртвое может быть отнесенно к этой категории так что после этих двух композиций есть ещё одна композиция на Китайском языке и когда вы её переводите она переводится как газовая духовка я имею из чего созданно Солнце у тебя есть плазма у тебя есть куча всего ты знаешь всё что электризуется и вызываент много тепла огня и всего остального это похоже о Солнце а потом после этого ты спрашиваешь нравится ли тебе кондиционер когда тебе по настоящему жарко так что знаешь это говорит тебе о том что на Земле скоро станет жарко понимаешь всё вокруг будет нагреваться тебе это нравится потому что тебе это понравится, и последняя строчка из этого списка [Red Sun in the sky](https://www.youtube.com/watch?v=IHeYmFHxSt8&list=OLAK5uy_kh-DA5qCCtBrGDbhOMeXmZ2_Kn9DX3F0k&index=13) когда я прочитал это я подумал срань господня на секунду в небе появилось красное Солнца, и я имею ввиду что мне тебе больше нечего сказать это красное Солнце оно превратилось в красную звёзду оно раскаляется оно расширяется и тут я подхожу к этому понимаете именно здесь мы можем окнчательно утвердится в теории о красном Солнце, время снова и снова показывает что мы можем понять о сюжете если обратим внимание на Солнце но это не главаня цель всей истории Кейна Парсенса, и ещё одно обратите внимание на образ Ивана обратите внимание как он стоит на фоне не только зелёного но, и жёлтого, и оранжевого цвета похоже у него какие-то проблемы что происходит? Понимаете о чём я меня так завораживает этот персонажа и тайна которая его окружает но в любом случае это мои размышления о конце Солнца это может стать концом самого бэкрумса и того как мы наблюдаем конец в реальном времени потому что она не может воспроизвести всё как следует, и скопировать всё что хочет скопировать у неё заканчивается память, заканчивается энергия, но у неё никогда не заканчится место никогда! Оно бесконечно оно будет существовать вечно, и поэтому оно может бесконечно множить свои неудачи но в конце концов оно может начать копировать свои собственные неудачи так что понимает, и тогда, и потом погружаете, и начинаете думать о том что может что-то ускальзнуть или выйти за предел допустимого в [Found Footage 3](https://www.youtube.com/watch?v=acdYs9tPLko&list=PLVAh-MgDVqvDUEq6qDXqORBioE4Yhol_z&index=21&pp=iAQB0gcJCQYLAYcqIYzv) мы ясно видим как что-то выбегает из стены из шкафа, и из окна в подвале где был Рави так что там происходит много всего и всё одновременно но я правда думаю что мы увидели конец и конец этот угасания Солнца наш настоящий враг так время как, и Солнце но опять же время главный фактор в итоге энергия поступающая в бэкрумс изсякнет вот почему мы сталкиваемся с таким проблемами как наложенние текстур на стены это своего рода ремарка. 

## Бэкрумс - это закулисье так что же сцена!?

Если бэкрумс это закулисье, а вселенная это сцена — значит где-то должен существовать зрительный зал, должно быть зрительный зал — это потусторонний мир куда попадают после смерти где существуют боги и высшие силы которые наблюдают за нами, но они не видят то что происходит в закулисье должно быть бэкрумс скрыт от их глаз.
А если развить теорию дальше, то можно подумать, что бэкрумс это скорее оперный театр, чем просто театр, то можно сказать что есть ещё и ложи, бельэтажи, бенуары, галёрки, партеры и чем они являются можно только догадываться.

## Пропавшие без вести

<img width="400" height="400" alt="Сохраненное изображение 2026-5-22_21-42-52 641" src="https://github.com/user-attachments/assets/280ae2a2-f70f-4b2c-b093-e3ac3226724c" />

Мы знаем, что ежегодно пропадает миллионы людей без вести, а самая страшное что многие из них не будут найдены может быть кто-то из них утонул в болоте, а кто-то с инсценировал свою смерть тем не менее многие склоняются к тому люди проваливаются в закулисье, и им остаётся лишь бродить по бесконечному лабиринту в надежде найти выход, которого нигде нет.

## Квантовое туннелированние
Это очень сложное явление в квантовой физике предполагается что у частиц есть некий барьер, который не дает другим частицам пройти через него, то есть если вы будете обладать достаточной энергией, то вы можете преодолеть барьер, и пройти сквозь неё как вы догадались так можно достичь noclip, и раз некоторые люди проваливаются сквозь текстуры нашего мира то это вполне можно объяснить явлением квантового тунеллирования.

## Кем или чем является натюрморт?

Наверняка многие из вас считают что натюрморт это результат мутировавшего человека а что если я вам скажу что натюрморт это не единственный человекоподобнаяы сущность закулисья в изобразительном исскустве натюрморт обозначает жанр в котором обозначает неодушевленный предметы значит исходя из названия можно сразу понять что Натюрморт не явлется живым существом, и никогда им не был во втором эпизоде Found footageи приложенном к нему видео home_27647.mov мы узнали что закулисье полностью копирует людей, и предметы из реального мира только вот во время копирование происходят заметные искажения. 

Напримере натюрморта мы выидим что комплекс может копировать людей, и это значит что натюрмтор является проекцией когда давно пропавшего челвоека в закулисье поэтому вполне возможно что попав в закулисье вы вероятность встретите взрослых, детей, подростков, стариков у которых будут страшные, и непонятные деффекты. 

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

## Бэкрумс это место которое пытается копировать реальный мир

Комплекс попытался скопировать радиостанцию из нашего мира, из-за открытого порога, он вполне мог поймать волну зацикленного фрагмента эфира , при чём исказив его. Для комплекса это как создать кресло: если есть звуки, то будут звуки, но определённого устройства радиовышки не будет. В одном из эпизодов рутины Async, они снимают потолочную лампу рядом с порогом -  у неё вообще нет источника энергии но она работает. То есть комплекс понимает, что это и что оно должно делать, но как это работает он не понимает.

пока порог(ну вход) открыт, комплекс может хоть до бесконечности улучшать архитектуру и сущностей. Для комплекса самой большой нестабильностью является именно порог(его боятся слабо развитые сущности), и он хочет добиться его закрытия: комплекс вполне может создавать ноуклип-зоны в осмысленных местах(в FF3 Рави привлёк некий звук в подвале, это было привлечение внимания), а поведение людей и их, находящихся в нём, он вполне может исследовать для развития натюрморта - он уже имеет очертание человека, способен издавать некоторые человеческие звуки(кашель например). Комплекс может создать "подменыша",  которые вполне может влиться в Async(в комплексе побывало много учёных и рядовых, он мог успеть изучить их цели и поведение), а может даже нескольких таких, для развала Async и последующего запечатывания порога. 

Таким образом - чем больше людей попадают в комплекс, тем более развитыми они становятся для более эффективной утилизации, а чем дольше открыт порог - тем более осмысленными и запутанными становятся локации.

Можно только догадываться о том насколько далеко и «проработанно» закулисье может копировать мир и живое (натюрморт,бактерия и прочих сущности).

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

## Теория об агрессивности закулисья

У меня есть теория: чем сильнее Async изучают и вторгаются в комплекс(ну закулисье), тем агрессивнее он становится. Async буквально мнят себя богами, контролирующими всё, но на самом деле они - вирус, от которого комплекс пытается избавится. Комплекс, насильно затягивая людей в себя, создавая сущностей и запутанные локации, пытается заставить Async закрыть порог и больше в него не соваться. С течением времени, комплекс создаёт всё более трудные условия для выживания человека: FF1 - (возможно) первая попытка создать нечто живое, FF2 - комнаты наполнились странным интерьером, стали разнообразнее, гланую героиню комплекс(скорее всего) использовал для "чертежа" натюрморта, FF3 - новая продвинутая форма жизни - натюрморт (умеет издавать звуки и музыку для привлечения внимания жертвы), коридоры стали совсем запутанными(человеку легче заблудиться и труднее убежать от сущностей). 

## Бэкрумс - это баг который был создан для того чтобы выбраться из бесконечной рекурсии симуляции вселенных.

Согласно этой теории, вселенная это компьютерная симуляция, которая была создана в компьютерной симуляции и так до бесконечности вплоть до самой первой симуляции вселенной, а бэкрумс это дыра проделанная в пространстве под текстурами нашей реальности, бесконечной рекурсии симуляции вселенных баг, который намеренно создало кто-то или что-то для того чтобы выйти за рамки бесконечности рекурсий симуляции вселенных, и попасть в реальную реальность, и чем ближе мы подходим к центру тем глубже мы погружаемся в бэкрумс тем более глючным, и лаганным он становиться… Остается только догадываться что расположено там в настоящей реальной реальности, должно быть это мир хаотичного хаоса – гиперкосмос в котором законы мироустройства настолько бесконечны сложны что бесконечно неописуемые, настолько хаотично хаотичный хаос что вызывает дикий ужас первородного мироздания вселенной перед истинной формой существование всего сущего.

## Бэкрумс – это сущность которая пытается скопировать реальный мир.

Знаешь мне иногда кажется, что где-то там в глубине бесконечности всех этих коридоров, помещений, и уровней обитает некое такое мистическая многомерная сверхъестественная сущность! И вот эта вот сущность для чего-то… Пытается дотянуться до материальности, до физической вселенной, пытается её объять, скопировать наш мир! Но раз за разом у неё ничего не получается, каждая её копия получается битой, и уродливой… Будто-бы она пытается собрать какую-то мозаику… Она проделала бесконечную дыру в пространстве, и времени… Заполнив её бесконечным невпопад случайно неправильно собранной мозаикой уродливых разбитых осколков нашей вселенной... Говорят, что бекрумс это глюк, ошибка в матрице вселенского мироздания… 

А для тех, кто здесь впервые объясняю - бекрумс это глюк реальности, сбой в матрице вселенского мироздания, ошибка! Которой не должно быть… сверхъестественное явление, и от него можно ожидать абсолютно всего чего угодно, так что будьте готовы ко всему законы по которым он существует, и функционирует вообще не поддается какому-либо описанию, объяснению, и логике… Все попытки описать какую-либо логику законов, по которым он существует претерпели крах. Сам факт его существования является невозможным в принципе он противоречит всем законам физики, он противоречит мироустройству всего сущего. Однако он существует каким-то загадочным образом, и это факт. 

## Центр закулисья 

Существует ли центр у закулисья? И что в нём находится?

## P.S.

Теперь это полноценное закулисное пространство! Возможно, кто-то придумает какие-то новые проекты, и проект будет развиваться.
