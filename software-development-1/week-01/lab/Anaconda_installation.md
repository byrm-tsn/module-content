# Anaconda installation

These instructions are adapted from the main Anaconda Installation instructions available here: [Installation — Anaconda documentation (continuum.io)](https://docs.continuum.io/anaconda/install/).

### Windows

1. Download the 64-bit Graphical Installer for Anaconda from <https://www.anaconda.com/download/#windows>.

![image-20210402200458023](image-20210402200458023.png)

2. Double-click the installer to launch.

3. Click Next.

4. Click "I Agree".

5. Select an install for "Just Me".

6. Select a destination folder to install Anaconda (the default is normally fine) and click the Next button.

7. Click Install.

8. Click Next.

9. Click Next.

10. You will now see the "Thanks for installing Anaconda" dialog box. Click the Finish button.

### MacOS

1. Download the 64-bit Graphical Installer for Anaconda from <https://www.anaconda.com/downloads#macos>.

   ![image-20210402200458023](image-20210402200458023.png)

2. Double-click the downloaded file and click continue to start installation.

3. Answer the prompts on the Introduction, Read Me, and License screens.

4. On the Destination Select screen, select Install for Me Only then click Continue.

5. Click the Install button.

6. Grant any permissions that the installer asks for.

7. Click Continue.

8. Click Close.

9. Click Move to Bin.

## Advice before Starting

The **computer is stupid**. It needs to know exactly what you mean when you give it instructions. It has no ability to guess. To become a programmer, you have to work on three skills as a beginner:

- **Precision** -- you need to **type instructions exactly as given**. The computer is case sensitive, it will treat uppercase and lowercase letters differently. The computer cannot guess your spelling mistakes. You need to be precise when entering instructions.
- **Patience** -- you need to be patient when learning to program. You will make mistakes, and the computer will shout at you. Your job is to recognise your errors and start building your programming capability.
- **Practice** -- you have to **constantly practice**. You cannot write a few lines of code and think you are a programmer. You have to build up a certain type of problem solving skill to talk to the computer and write high-quality software.

## Setting Up Python

1. Open **Anaconda Navigator** from your Start Menu (Windows), Launchpad (MacOS), or equivalent on Linux.

2. Once started, you will be presented with the following window.

   ![image-20210402214430745](image-20210402214430745.png)

3. Click Launch under Qt Console.

4. This will open a **Command Line Interface** window similar to the following:

   ![image-20210402214603068](image-20210402214603068.png)

We must install an additional package to work with graphics in Python.

- **Enter the following *precisely* into the command line interface.**

```shell
pip install graphics.py
```

- **Next we have to do is ask Python to import our graphics library.**

```python
from graphics import *
```

## Creating a Graphics Window in Python

We are going to draw graphics to a window. Let us perform the following steps:

1. Open a graphics window.
2. Set its background to white.
3. Close the graphics window.

- **This is accomplished with the following lines of code. Enter them *precisely* into Python.**

```python
win = GraphWin()
win.setBackground('white')
win.close()
```

## Graphics Coordinate Systems

Windows have coordinates. `(0, 0)` is the top-left corner. `(w, h)` is the bottom-right corner -- where `w` is the window width and `h` the height.

![](screen.png)

## Drawing Circles

Circles have a centre (in coordinates) and a radius. We can also set the colour of our circle. Let us do the following:

1. Create a graphics window. Let's call the window `Flag` and set the size to 600 by 400.
2. Create a circle with centre at (100, 100) and radius 50.
3. Set the fill colour of the circle to red.
4. Draw the circle to the window.

- **Try the following code in Python.**

```python
win = GraphWin("Flag", 600, 400)
circle = Circle(Point(300, 200), 100)
circle.setFill('red')
circle.draw(win)
```

Congratulations. You have just drawn the Japanese flag.

![image-20201109145817238](image-20201109145817238.png)

- **Close the window using the following.**

```python
win.close()
```

## Drawing Rectangles

A rectangle has a start point and an end point. We can also set its colour. Let us do the following:

1. Create a graphics window called `name` with a size of 600 by 400.
2. Create a rectangle from point (0, 0) to point (100, 200).
3. Set the rectangle colour to blue.
4. Draw the rectangle.

- **Try drawing the rectangle now using the following code in Python.**

```python
france = GraphWin("France", 600, 400)
rect = Rectangle(Point(0, 0), Point(200, 400))
rect.setFill("blue")
rect.draw(france)
```

### Now You Try -- Completing the French Flag

You have now started drawing the French flag. You can complete the flag by drawing two more rectangles. For reference, here is a visual aid.

![](French.png)

- **If you cannot complete this, the following code will complete the flag.**

```python
rect = Rectangle(Point(200, 0), Point(400, 400))
rect.setFill('white')
rect.draw(france)
rect = Rectangle(Point(400, 0), Point(600, 400))
rect.setFill('red')
rect.draw(france)
```

- **Remember to close the window when you are finished.**

```python
france.close()
```

### Now You Try -- More Flags

Write code to draw the following flags.

- **Indonesia**

![image-20210331200627218](image-20210331200627218.png)

- **Poland**

![image-20210331200636972](image-20210331200636972.png)

- **Austria**

![image-20210331200649941](image-20210331200649941.png)

- **Gabon**

![image-20210331200704928](image-20210331200704928.png)

- **Yemen**

![image-20210331200713546](image-20210331200713546.png)

- **Mauritius**

![image-20210331200722066](image-20210331200722066.png)

- **Italy**

![image-20210331200734172](image-20210331200734172.png)

- **Mali**

![image-20210331200744304](image-20210331200744304.png)

- **UAE**

![image-20210331200754487](image-20210331200754487.png)

- **Gambia**

![image-20210331200802531](image-20210331200802531.png)

- **Thailand**

![image-20210331200810728](image-20210331200810728.png)

- **Laos**

![image-20210331201016569](image-20210331201016569.png)

- **Maldives**

![image-20210331201122316](image-20210331201122316.png)
