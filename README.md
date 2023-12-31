# UE_Ball – Первое тестовое задание
На стажировку в 42dev studio. 

![bgfg](https://github.com/KachesovVadim/UE_Ball/assets/142095950/cbd65b92-c77d-484f-83aa-bb10052b50ea)

Геймплейный ролик - https://youtu.be/8aSiHEYz9OE?si=GViK071dAaMX2u2H

Билд игры - https://drive.google.com/file/d/1iSfzFSQ70l5wC9UuJYzeq3YAuqvF2Z3w/view?usp=sharing

<details><summary>Техническое задание (нажми)</summary>
<p>
  
(Я добавил пояснения к некоторым пунктам)
  
Реализовать сцену, содержащую в себе:
1.	Ландшафт
-	Реализовано на 1 уровне
2.	Растительность (для слабых компов можно немного)
- На 3 уроне
3.	Наложить текстуры (как можно ровнее, без швов)
4.	Перевести всю созданную геометрию в Static Mesh, добавить коллизии
5.	Сделать зеркало
- Зеркальная комната на 3 уровне
6.	Расставить на уровне освещение
7.	Сделать сборку освещения (для слабых компов - Preview, для компов посильнее можно выбрать более красивые настройки освещения)
8.	В случае, если static mesh после сборки освещения стали абсолютно черными, в свойствах каждого static mesh найти и указать значения для Light Map Resolution - 64, для Light Map Coordinate Index - 1
9.	Добавить постобработку (post-process) изображения на свой вкус.
-	Реализовано в камере персонажа


Техническая часть:
1.	Создать персонажа (можно импортировать из стартовых паков или создать без скелета (пустого)), который может передвигаться, управлять камерой.
2.	Добавить дверь в виде БП (попробовать избежать Collision Box)
3.	Создать функционал различного взаимодействия с объектами, объекты могут быть разных классов (поведение объекта должно быть разным при взаимодействии с ним, допустим двери в разные комнаты открываются по-разному)
- В конце 3 уровня есть 4 фигуры которые через диспатчеры синхронно уничтожаются при взаимодействии хотя бы с одной
4.	Добавить вывод виджетов на экран, содержащие разную информацию, ОБЯЗАТЕЛЬНО - ваша ФИО и ник, остальное ваш вкус
- Виджет после прохождения игры.
5.	Создать БП, логика которого основана на Event tick, с применением delta секунд (крутящаяся лампочка крутится с одинаковой скоростью, независимо от FPS на ПК)
- Вентилятор на 3 уровне сделан с применением delta секунд
  
Так же, нужно было создать актора, который использует BPI (спавн врагов), gameinstance, реализовать в компонентах основную логику персонажа.
</p>
</details>

## Об игре

В моем случае тема проекта была свободная. Срок 5 дней. Суть этого тестового задания была в том, что нужно доказать свои базовые навыки владения блюпринтами и движком для прохождения стажировки. 

Суть игры – выжить. Необходимо продержаться минуту на первых двух уровнях чтобы перейти на последний. После прохождения 1 уровня даются 2 пистолета, которыми нужно поочередно стрелять на ПКМ и ЛКМ. С каждым выстрелом коэффициент урона увеличивается. Этим пистолетом можно отстреливаться от контейнеров на 2 уровне. Чтобы пройти 3 уровень, нужно взаимодействовать с 1 из фигур.

На тот момент я уже во всю работал над основным проектом «Superindustry», процесс создания которого я публикую в девлогах - https://habr.com/ru/users/OMEGA-quality/publications/articles/ В нем были реализованы реально сложные механики, которыми можно гордиться. Этот проект так же есть и на моем github.

## Управление
ПКМ, ЛКМ – стрельба

Е - взаимодействие

## Фотогалерея
![Снимок экрана (176)](https://github.com/KachesovVadim/UE_Ball/assets/142095950/1a382f24-32e0-48f2-972a-38dec84ec3cd)
![Снимок экрана 2023-09-15 165437](https://github.com/KachesovVadim/UE_Ball/assets/142095950/6870bf84-bed1-48bf-9412-1068aaff8537)
**Уровень 1**

![Снимок экрана (192)](https://github.com/KachesovVadim/UE_Ball/assets/142095950/7d6e9417-2552-46dc-be09-37d74165cdd5)
![Снимок экрана 2023-09-15 165531](https://github.com/KachesovVadim/UE_Ball/assets/142095950/630974ab-26f8-400f-88d2-9073f113abc9)
**Уровень 2**

![Снимок экрана (197)](https://github.com/KachesovVadim/UE_Ball/assets/142095950/35e6d864-99fc-410e-a0a0-7838f693d0d2)
![Снимок экрана (208)](https://github.com/KachesovVadim/UE_Ball/assets/142095950/c3df9c82-0e9e-4d4b-b01a-20611895e44f)
**Уровень 3**

![Снимок экрана (210)](https://github.com/KachesovVadim/UE_Ball/assets/142095950/9d643e44-af2a-4bf6-a6bf-05c45a6e9c3e)


