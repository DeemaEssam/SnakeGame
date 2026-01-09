# SnakeGame
*****************************************************************************************

| Endlish | عربي  |
| -- | -- |
|
**SnakeGame** is a JavaFX application that implements the classic **Snake** game.
The player controls a snake that moves around the game board and eats food that appears at random locations.
The game ends when the snake collides with the wall or with its own body.

---

## 🎮 Game Mechanics

* The snake moves continuously in the current direction.
* When the snake eats food:

  * The snake grows in length.
  * The player’s score increases.
  * The snake’s speed may increase based on the score.
* The game ends when:

  * The snake hits the wall.
  * The snake collides with itself.

---

## ⚙️ Game Configuration

The **SnakeGame** class contains a set of constants and variables that define the game’s behavior and state, including:

* Snake movement speed.
* Game board size.
* Snake position and direction.
* Food position and color.
* Game state (running or game over).

---

## 🧱 Classes Description

### 1️⃣ SnakeGame Class

The main class of the application.

#### Key Methods:

* **start()**
  Creates the game start screen.
* **startGame()**
  Starts the actual game by:

  * Creating the game board.
  * Updating the snake’s movement.
  * Rendering frames.
  * Detecting collisions.

---

### 2️⃣ Corner Class

A nested class that represents a single cell on the game board.

#### Attributes:

* `int x` – horizontal position.
* `int y` – vertical position.

#### Constructor:

* Initializes the cell’s position using the provided `x` and `y` values.

---

### 3️⃣ Speedup Class

A class responsible for increasing the snake’s speed as the player’s score increases.

#### Attributes:

* `int scoreThreshold`
  Represents the score at which the speed increase is triggered.

#### Constructor:

* Assigns the score threshold value.

#### Method:

* **increaseSpeed(int score)**
  Adjusts the snake’s speed based on the score:

  * Score = 3 → speed is set to **7**
  * Score = 6 → speed is set to **10**
  * Score = 8 → speed is set to **14**
  * Otherwise → no change is applied

> This class is used in `SnakeGame` with a `scoreThreshold` value of **3**.
---

## 🚀 Technologies Used

* Java
* JavaFX
)  | (
**SnakeGame** هو تطبيق مكتوب باستخدام **JavaFX** يُحاكي لعبة **Snake** الكلاسيكية.
تتحكم في ثعبان يتحرك داخل لوحة اللعب، ويقوم بأكل الطعام الذي يظهر بشكل عشوائي.
تنتهي اللعبة في حال اصطدام الثعبان بجدار اللعبة أو بجسمه.

---

## 🎮 Game Mechanics

* يتحرك الثعبان بشكل مستمر حسب الاتجاه الحالي.
* عند أكل الطعام:

  * يزداد طول الثعبان.
  * تزداد النقاط (Score).
  * قد تزداد سرعة الثعبان حسب النقاط.
* تنتهي اللعبة عند:

  * الاصطدام بالجدار.
  * الاصطدام بجسم الثعبان نفسه.

---

## ⚙️ Game Configuration

تحتوي فئة **SnakeGame** على مجموعة من الثوابت والمتغيرات التي تتحكم في:

* سرعة الثعبان.
* حجم لوحة اللعب.
* اتجاه وحركة الثعبان.
* موقع الطعام ولونه.
* حالة اللعبة (تشغيل / انتهاء).

---

## 🧱 Classes Description

### 1️⃣ SnakeGame Class

الفئة الرئيسية للتطبيق، وتشمل:

* **start()**
  تقوم بإنشاء شاشة البداية للعبة.
* **startGame()**
  تبدأ اللعبة فعليًا من خلال:

  * إنشاء لوحة اللعب.
  * تحريك الثعبان.
  * تحديث الإطارات (Frames).
  * التحقق من التصادمات.

---

### 2️⃣ Corner Class

فئة داخلية (Nested Class) تمثل خلية واحدة في لوحة اللعب.

#### Attributes:

* `int x` : الموقع الأفقي.
* `int y` : الموقع العمودي.

#### Constructor:

* يستقبل قيم `x` و `y` ويقوم بتهيئة الخلية.

---

### 3️⃣ Speedup Class

فئة مسؤولة عن **زيادة سرعة الثعبان** مع تقدم اللاعب في النقاط.

#### Attributes:

* `int scoreThreshold`
  تمثل النقاط التي عندها تبدأ زيادة السرعة.

#### Constructor:

* يستقبل قيمة النقاط المطلوبة لزيادة السرعة.

#### Method:

* **increaseSpeed(int score)**
  تزيد سرعة الثعبان حسب النقاط:

  * عند Score = 3 → السرعة تصبح **7**
  * عند Score = 6 → السرعة تصبح **10**
  * عند Score = 8 → السرعة تصبح **14**
  * غير ذلك → لا يتم تغيير السرعة

> يتم استخدام هذه الفئة داخل `SnakeGame` مع قيمة `scoreThreshold = 3`.

---

## 🖼️ Screenshots

### ❌ Game Over

![lose](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/ed634157-c19d-47e4-b59d-d1d4e3b5b286)

### 🏆 Winning State

![win](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/de65181e-3908-4948-a9d6-84fc2b2c3437)

---

## 🚀 Technologies Used

* Java
* JavaFX
✨
) |








The SnakeGame class is a JavaFX application

that implements the classic Snake game. The game consists of a snake that moves around the game board
and eats food that appears randomly on the board. The game ends when the snake collides with the wall or
with its own body. The class has a set of constants and variables that define the game’s behavior and state,
including the speed of the snake, the size of the game board, the snake’s position and direction, and the
location and color of the food. The class also has a nested Corner class that represents a single cell of the
game board, and a nested Speedup class that can be used to increase the speed of the snake as the player’s
score increases. The class has two methods: start, which creates the game’s start screen, and startGame,
which starts the game by creating the game board and updating the frames of the snake’s movement on the
screen.

The Corner class is a simple class that represents a single cell of the game board. It has two integer
instance variables, x, and y, that represent the cell’s position on the board. The class has a constructor that
takes two integer parameters and initializes the instance variables.

The Speedup class is a class that can be used to increase the speed of the snake as the player’s score
increases. 

The class has an integer instance variable scoreThreshold that stores the score at which the speed
will be increased. The class has a constructor that takes an integer parameter and assigns it to the instance
variable. The class also has a method increaseSpeed that takes an integer parameter score and increases the
speed of the snake based on the score. 

If the score is equal to 3, the speed is set to 7. If the score is equal
to 6, the speed is set to 10. If the score is equal to 8, the speed is set to 14. If the score does not match any
of these values, the method does nothing. The class is used in the SnakeGame class to create an instance of
the class with a score threshold of 3.

# execution
![lose](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/ed634157-c19d-47e4-b59d-d1d4e3b5b286)
![win](https://github.com/DeemaEssam/BabyNamesRanking/assets/106381596/de65181e-3908-4948-a9d6-84fc2b2c3437)

