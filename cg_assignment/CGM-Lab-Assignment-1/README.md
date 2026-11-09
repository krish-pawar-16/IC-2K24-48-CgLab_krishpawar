# Computer Graphics Lab – Assignment 1

## Basic Geometric Shapes Using C++ and SDL2

**Subject:** Computer Graphics  
**Assignment:** 1  
**Topic:** Basic Geometric Shapes  
**Language:** C++  
**Graphics Library:** SDL2

## Objective

To write a C++ program using the SDL2 graphics library to draw four basic geometric shapes in a single graphics window.

## Shapes Implemented

1. **Straight Line – Blue:** Drawn using the SDL2 line drawing function.
2. **Circle – Red:** Drawn using the Midpoint Circle Algorithm.
3. **Rectangle – Green:** Drawn using the SDL2 rectangle drawing function.
4. **Triangle – Purple:** Drawn using three connected lines.

## Technologies Used

- C++
- SDL2 Graphics Library
- GCC / MinGW64 Compiler
- Visual Studio Code

## Project Structure

```text
CGM-Lab-Assignment-1/
│
├── BasicShapes.cpp
├── README.md
│
└── output/
    └── BasicShapes_Output.png
```

## How to Compile

Open the terminal in the assignment folder and execute:

```powershell
& "C:\msys64\mingw64\bin\g++.exe" BasicShapes.cpp -IC:\msys64\mingw64\include\SDL2 -LC:\msys64\mingw64\lib -lmingw32 -lSDL2main -lSDL2 -o BasicShapes.exe
```

## How to Run

```powershell
$env:Path = "C:\msys64\mingw64\bin;" + $env:Path
.\BasicShapes.exe
```

## Output

The program displays all four geometric shapes in a single graphics window with a white background.

The screenshot of the program execution is available in the `output` folder.

## Learning Outcomes

- Understood basic geometric shapes in computer graphics.
- Learned to use SDL2 graphics functions.
- Implemented the Midpoint Circle Algorithm.
- Learned how to draw lines, circles, rectangles and triangles using C++.
- Understood graphical window creation and rendering using SDL2.