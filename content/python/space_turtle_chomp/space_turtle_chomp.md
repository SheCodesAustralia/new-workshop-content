---
title: "Space Turtle Chomp"
weight: 2
chapter: false
---

We will start off today creating a simple Python game using Python Turtle Graphics. Turtle Graphics is a prebuilt set of python instructions that allow you to create and move characters around the screen, enabling you to draw pictures, logos and create simple animations or games.

>**Step 1.**  If not already open please open VS Code.

>**Step 2.**  Select File --&gt; New File. You should now see your program window

>**Step 3.**  Since it is a great idea to save your project at the beginning of any new development, select File --&gt; Save and name the file (I called mine kbgame1.py)
> 
> VS Code may ask if you want to install a Python extension, feel free to follow the prompts and do so.

> **Step 4.** We need to make sure that VS Code knows where to find Python. Here's how to do that:
>
> {{< tabs groupid="a">}}
 {{% tab title="_**MacOS**_" %}}

 Press `Cmd+Shift+P` to open the Command Palette, type **Python: Select Interpreter**, and press `Return`.

 A list of available Python installations will appear. Look for one that mentions `uv` in its path (something like `~/.local/share/uv/python/cpython-.../bin/python`). Select it.

 {{% /tab %}}
 {{% tab title="_**Linux**_" %}}

 Sorry, but on Linux things get just a little bit more complicated. Linux doesn't always include the graphics library we need (`tkinter`), so we need to install it manually and set up a virtual environment. Here's how:

 Open the VS Code terminal (`Ctrl+`` ` or **View → Terminal**) and run the following commands one at a time:

 ```sh {title="terminal"}
 sudo apt-get install python3-tk
 ```

 ```sh {title="terminal"}
 uv init --bare
 ```

 ```sh {title="terminal"}
 uv venv --system-site-packages
 ```

 The last command creates a virtual environment that has access to the `tkinter` library you just installed.

 Now tell VS Code to use it: press `Ctrl+Shift+P`, type **Python: Select Interpreter**, and press `Enter`. Choose the option that shows `.venv` in its path.

 {{% /tab %}}
   
 {{% tab title="_**Windows**_" %}}

 Press `Ctrl+Shift+P` to open the Command Palette, type **Python: Select Interpreter**, and press `Enter`.

 A list of available Python installations will appear. Look for one that mentions `uv` in its path (something like `C:\Users\<your_name>\AppData\Roaming\uv\python\cpython-...\python.exe`). Select it.

 {{% /tab %}}
> {{< /tabs >}}

>**Step 5.** When coding one of the first things we should always do as a developer is leave a comment explaining what the program does at the top of the screen. We can make a comment using #

An example of a comment is below, try writing the below on the top line. This code won't run, so feel free to write whatever helpful notes you like here:

```python {title="python"}
# Turtle Graphics Game – Space Turtle Chomp
```

>**Step 6.** Next we need to import the Turtle libraries and set up the screen, we do this by typing:

```python {title="python"}
import turtle

# Set up screen
turtle.setup(650,650)
wn = turtle.Screen()
wn.bgcolor('navy')
```

{{% notice info %}}

`turtle.setup` sets the size of the Turtle game window \(it’s not necessary but helps when using different screen sizes\). 

`wn` is the name we are calling the screen \(as we learnt in the Python introduction all variables need a name\). 

`bgcolor` allows us to set the background colour. 

{{% /notice %}}

There are lots of colours to choose from. 

![colour chart](../images/100_Color_names_python.png)

{{% notice note %}}

**Note:** You have to use the American spelling of **color** in your code, this is something to watch out for when programming.

{{% /notice %}}

{{% notice tip %}}
It is good practice to leave a comment \(\#\) before your code so you can remember what it does. Your future self will thank you!
{{% /notice %}}

>**Step 6.** Next we create our first Turtle character, we do this by typing:

```python {title="python"}
# Create player turtle
player = turtle.Turtle()
player.color('darkorange')
player.shape('turtle')
player.penup()
```

So we create a new turtle variable called player then use the inbuilt turtle attributes to help set it up, `player.color` \(again we can select a different colour from the colour chart). 

`player.shape` selects the shape \(you can also use circle, arrow, square and classic\). 

`penup` means that the turtle shape won’t leave a line when it moves \(think of a pen in your hand, penup\(\) you don’t draw, pendown\(\) you do draw).

>**Step 7.** Now we set the speed we want our turtle to move across the screen at:

```python {title="python"}
# Set speed variable
speed = 1
```

>**Step 8.** Finally we need the turtle to move and the easiest way to do this is by setting a while loop:

```python {title="python"}
while True:
    player.forward(speed)
```

{{% notice note %}}

Note the indent of the line starting with player.forward. This indent needs to be there for the code to work.

{{% /notice %}}

This piece of code is slightly different to the code you have written
before. Instead of telling the computer to perform an instruction *once*, you are telling the computer to **repeatedly** perform that instruction *for as long as some condition is true*. You are doing this using what's called a `while` loop. 

The syntax of a `while` loop is:

```python {title="python"}
while <condition>
   # do stuff here
```

In our example ``<condition>`` is simply the value True, that always evaluates to ``True``. Meaning that our turtle will move forward until the program is closed.

>**Step 9.** Now all we need to do is save our code, we can do this by selecting File --&gt; Save \(Ctrl S on Windows or Cmd S on Mac\). Then run the module by selecting Run --&gt; Run Without Debugging \(or pressing Ctrl F5 on Windows or ^F5 on Mac \).

You should see two windows open up: a Python Shell window that will have “Python 3.12.4 \(v3.12.4:69c0db5, Aug 11 2017, 17:54:52\) \[MSC v.1900 32 bit \(Intel\)\]…” or something similar written on it and your Turtle window with a Navy background and Dark Orange turtle moving across the screen. Close both the shell and turtle window to return to your programming code.

Before moving on to the next section you can have a play with your code by trying different colours, shapes and speeds and for some fun you could change `player.penup()` to `player.pendown()`

Your code should now look like this:

```python {title="python"}
#Turtle Graphics Game
import turtle

#Set up screen
turtle.setup(650,650)
wn = turtle.Screen()
wn.bgcolor("navy")


#Create player turtle
player = turtle.Turtle()
player.color("darkorange")
player.shape("turtle")
player.penup()

#Set speed variable
speed = 1


while True:
   player.forward(speed)
```
{{% notice style="tip" title="Time to celebrate" %}}

**Congratulations Module 1 Completed**

{{% /notice %}}