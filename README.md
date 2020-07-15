# CPPND: Capstone Snake Game Example

This is a starter repo for the Capstone project in the [Udacity C++ Nanodegree Program](https://www.udacity.com/course/c-plus-plus-nanodegree--nd213). The code for this repo was inspired by [this](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) excellent StackOverflow post and set of responses.

<img src="snake_game.gif"/>



At the begin the game asking the user to enter values for:
- The prefered starting speed from 1 to 100 
- The prefered increasing rate from 1 to 100

<img src="User_Input.png"/>


* The score increasing each time depending of the current speed and the selected by the user increasing rate. 
* So here is a challenge: How to achieve the best score? (making different combinations of starting speed and increasing rate)


The Capstone Project gives you a chance to integrate what you've learned throughout this program. This project will become an important part of your portfolio to share with current and future colleagues and employers.

In this project, you can build your own C++ application or extend this Snake game, following the principles you have learned throughout this Nanodegree Program. This project will demonstrate that you can independently create applications using a wide range of C++ features.

## Dependencies for Running Locally
* cmake >= 3.7
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* SDL2 >= 2.0
  * All installation instructions can be found [here](https://wiki.libsdl.org/Installation)
  * Note that for Linux, an `apt` or `apt-get` installation is preferred to building from source.
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory in the top level directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./SnakeGame`.


## Matched Rubrics 
1. Object Oriented Programming - The project uses Object Oriented Programming techniques.
The project code is organized into classes with class attributes to hold the data, and class methods to perform tasks.
Each class is seperated in to definition and in to declaration files which includes the corresponding implementation of the functions respectively.

2. Loops, Functions, I/O - The project accepts user input and processes the input.
The project accepts input from a user as part of the necessary operation of the program.

In file game.cpp from line 21 to 25 the system ask the user to enter the prefered starting speed. 
Within these lines the system detects if the number the user entered are higher than the accepted.

In file game.cpp from line 28 to 32 the system ask the user to enter the prefered speed increasing rate after each food the snake eats. 
Within these lines the system detects if the number the user entered are higher than the accepted.

In file game.cpp line 97 created a new scoring mechanism to make the game more challenging. New scoring mechanism assigns score depended on users selected speed, increasing spead Rate and how many food the snake eaten. The biger the selected speed and higher the increasing ration, means that the user takes bigger score for each food the snake eat.
 
3. Object Oriented Programming - Classes abstract implementation details from their interfaces.
All class member functions document their effects, either through function names, comments, or formal documentation. Member functions do not change program state in undocumented ways.

The C++ Guide by Google was used to for any needed documentation. An example can be found within the file game.cpp lines 95-98 were described the new scoring mechanism.

4. Object Oriented Programming - Class constructors utilize member initialization lists.
All class members that are set to argument values are initialized through member initialization lists.

In file game.cpp in line 8 the variable tempSpeed initialized with value {0.1} as default value within the constructors initialization list.

5. Object Oriented Programming - Classes use appropriate access specifiers for class members.
All class data members are explicitly specified as public, protected, or private.

Within game.h the new variables incr and tempSpeed are private members in lines 33-34 and are used to store user's preferences about the speed and increrasing speed rate.

 
 
 
 
