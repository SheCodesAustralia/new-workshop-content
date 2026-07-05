---
title: "Getting Started"
weight: 2
chapter: false
---

In this tutorial you will be building a Bakery app. In order to do that, as you go through the tutorial you'll be instructed on how to install various software on your computer and set up some online accounts as needed if you wish to put your site live on the internet.

---

{{% notice info %}}
**Brief intro to the command line**

Many of the steps below reference the `console`, `terminal`, `command window`, or `command line` -- these all mean the same thing: a window on your computer where you can enter commands. For now, the main thing you need to know is how to open a command window and what it looks like. You'll get your first taste of this in the instructions below!

{{% /notice %}}

### Install Python

You'll need Python installed to follow this tutorial. If you haven't already, head over to the "Python" section in the lefthand panel of this website, and follow the instructions under "Getting Started".

Then come back here and continue below!

### Install a Code Editor

There are a lot of different editors and it largely boils down to personal preference. Most Python programmers use complex but extremely powerful IDEs (Integrated Development Environments), such as PyCharm. As a beginner, however, that's probably less suitable; our recommendations are equally powerful, but a lot simpler:

- [Visual Studio Code](https://code.visualstudio.com/)

#### Why are we installing a code editor?

You might be wondering why we are installing this special code editor software, rather than using something like Word or Notepad.

The first reason is that code needs to be plain text, and the problem with programs like Word and Textedit is that they don't actually produce plain text, they produce rich text (with fonts and formatting), using custom formats like RTF (Rich Text Format).

The second reason is that code editors are specialised for editing code, so they can provide helpful features like highlighting code with color according to its meaning, or automatically closing quotes for you.

We'll see all this in action later. Soon, you'll come to think of your trusty old code editor as one of your favorite tools. 

### Set up virtual environment and install Django

> [!primary] NOTE 
> The following instructions should be executed in the terminal!

Before we install Django we will get you to set up an extremely useful tool to help keep your coding environment tidy on your computer: a virtual environment. You might sometimes hear this referred to as a "venv".

Your virtual environment will isolate your Python/Django setup on a per-project basis. This means that any changes you make to one website won't affect any others you're also developing. Neat, right?

First, locate a directory in which you want to store your Django project. A good choice for this is your "Home" directory. On Windows, it might look like `C:\Users\<your_name>\` (where `<your_name>` is the name of your login).

You can navigate to that directory in your terminal using the following command:

```sh {title="terminal"}
cd ~
```

#### Create a project directory

For this tutorial we will be using a new directory bakery_site from your home directory:

```sh {title="terminal"}
uv init bakery_site --bare
```

This tells UV to set up a new project directory for you. 

Next change directory into your new `bakery_site/` directory with the `cd` command like so:

```sh {title="terminal"}
cd bakery_site
```

Let's take a quick look at what UV created for us using the `ls` command:

```sh {title="terminal"}
ls
```

You should see one file listed: `pyproject.toml`. UV uses this file to keep track of the details of your project.

#### Add Django As a Dependency

We need to tell UV that this project will use Django. The command for that is simple:

```sh {title="terminal"}
uv add django
```

This will add Django to the list of "project dependencies" in your `pyproject.toml` file. You can check this by running:

```sh {title="terminal"}
cat pyproject.toml
```

You should see something like:

```sh {title="terminal"}
[project]
name = "bakery_site"
version = "0.1.0"
requires-python = ">=3.12"
dependencies = [
    "django>=6.0.6",
]
```

#### Create the Virtual Environment and Install Dependencies

Here it is - we are now ready to install Django. The command to run is:

```sh {title="terminal"}
uv sync
```

This creates a virtual environment folder for you (with the directory name `.venv/`), and installs any listed dependencies.

When you use UV to run a python command, UV will automatically use your virtual environment if one is present. You can also manually activate your virtual environment if you need - the command to do this was displayed in the output when you created your virtual environment. (Probably something like `source .venv/bin/activate`, or `.venv\Scripts\Activate.ps1`)

---

Congrats, you are ready to Django!
