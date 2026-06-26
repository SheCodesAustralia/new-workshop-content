---
title: "Getting started"
weight: 1
chapter: false
pre: "💻🐍 "
---

### Let’s start with Python

We're finally here!

We need Python before we can start. To handle that we will use a tool called `UV`. [Check out the documentation here if you are curious.](https://docs.astral.sh/uv/)

`UV` simplifies the process of installing and running Python, and can help us organise our various Python projects too.

{{< tabs groupid="a">}}
{{% tab title="_**MacOS**_" %}}

Open the Mac Terminal by:
1. Pressing `Command` (⌘) + `Spacebar` to open Spotlight Search
2. Typing "Terminal" in the search field
3. Pressing `Return` (Enter) to launch the Terminal

Next, copy-paste the following command into your terminal window, and then hit `Return`:

<!-- {% filename %}command-line{% endfilename %} -->
```sh
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Congrats, you now have `UV` installed.

{{% /tab %}}
{{% tab title="_**Linux**_" %}}
Open the bash terminal, and run the following command:

<!-- {% filename %}command-line{% endfilename %} -->
```sh
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Congrats, you now have `UV` installed.

{{% /tab %}}
  
{{% tab title="_**Windows**_" %}}

Open PowerShell by:
1. Pressing the Windows key
2. Typing "powershell"
3. Clicking `Windows PowerShell`

Next, copy-paste the following command into your PowerShell window, and then hit `Return`:

<!-- {% filename %}command-line{% endfilename %} -->
```sh
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

Congrats, you now have `UV` installed.

{{% /tab %}}
{{< /tabs >}}

----

If you have any doubts, or if something went wrong and you have no idea what to do next, please ask a mentor!
