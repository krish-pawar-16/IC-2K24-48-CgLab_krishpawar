# Computer Graphics Lab – Assignment 2

## DDA Line Drawing Algorithm

**Subject:** Computer Graphics  
**Assignment:** 2  
**Topic:** Digital Differential Analyzer (DDA) Algorithm  
**Language:** C++  
**Graphics Library:** SDL2

## Objective

To implement the Digital Differential Analyzer (DDA) line drawing algorithm using C++ and SDL2 to draw a straight line between two user-defined points.

## Introduction

The Digital Differential Analyzer (DDA) is a line drawing algorithm used in computer graphics to generate a straight line between two given points.

It calculates intermediate pixel positions using incremental values of X and Y coordinates.

## Algorithm

1. Accept the starting coordinates (x1, y1).
2. Accept the ending coordinates (x2, y2).
3. Calculate dx = x2 - x1.
4. Calculate dy = y2 - y1.
5. Calculate the number of steps using the maximum absolute value of dx and dy.
6. Calculate X increment and Y increment.
7. Start from the initial coordinates.
8. Plot each pixel using the calculated increments.
9. Repeat until all steps are completed.

## Technologies Used

- C++
- SDL2 Graphics Library
- GCC / MinGW64 Compiler
- Visual Studio Code

## Project Structure

```text
CGM-Lab-Assignment-2/
│
├── DDA.cpp
├── README.md
│
└── output/
    └── DDA_Output.png
```

## How to Compile

Open the terminal in the assignment folder and execute:

```powershell
& "C:\msys64\mingw64\bin\g++.exe" DDA.cpp -IC:\msys64\mingw64\include\SDL2 -LC:\msys64\mingw64\lib -lmingw32 -lSDL2main -lSDL2 -o DDA.exe
```

## How to Run

```powershell
$env:Path = "C:\msys64\mingw64\bin;" + $env:Path
.\DDA.exe
```

## Sample Input

```text
Enter starting point (x1 y1): -200 -100
Enter ending point (x2 y2): 200 100
```

## Calculations

For the above input:

- dx = 400
- dy = 200
- Steps = 400
- X Increment = 1.0
- Y Increment = 0.5

## Output

The program displays coordinate axes and a blue line connecting the user-defined starting and ending points.

The screenshot of the program execution is available in the `output` folder.

## Learning Outcomes

- Understood the working of the DDA line drawing algorithm.
- Learned how to calculate dx, dy and the number of steps.
- Implemented incremental pixel plotting.
- Understood the conversion of mathematical coordinates into screen coordinates.
- Learned to display graphical output using SDL2.