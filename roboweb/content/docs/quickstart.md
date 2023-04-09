---
title: "Quickstart"
date: 2023-04-06T09:49:12-07:00
draft: false
---

## Install the JupyterLab Extension


Install the extensions


```
python -m pip install roboweb-extension
python -m pip install roboweb-server
```

Activate the extension


```
python -m jupyter serverextension enable --py roboweb_server
```

## Configure the Extension

To use the extension start jupyter lab.


```
jupyter-lab
```

In the right hand navigation window click the roboweb icon. This will open up the roboweb extension
in the right half of the screen.

{{< figure src="/docs/toolbar.png" caption="The Roboweb assistant should appear in the right hand side toolbar in JupyterLab." alt="Roboweb toolbar">}}

If you haven't already created an account (e.g. by visiting [ui.roboweb.app](https://ui.roboweb.app))
click **Create account**. 

Once you have created an account sign in.

{{< figure src="/docs/signin.png" caption="The Roboweb signin screen." alt="SignIn Page">}}

Once you are logged in, click the settings button in the navigation bar inside Roboweb's JupyterLab extension.


{{< figure src="/docs/lefthandnav.png" caption="The lefthand navigation bar shows a list of your chats and also a button to access settings." alt="SignIn Page">}}

On the settings page, enter your OpenAI API key and then click save.

{{< figure src="/docs/settings.png" caption="The settings page lets you configure Roboweb." alt="Settings">}}

Make sure the dropdown is set to `ChatGPT`.


## Using the extension to fix code

In Roboweb's extension, click on an existing Chat or start a new chat just like you would on ChatGPT.
Ask the assistant to help you with writing some code, just like you would in the ChatGPT playground.
When ChatGPT responds with code, Roboweb will display this in a code box. The upper right hand corner
will contain a play button. Click this button to copy the code into a jupyter cell.

{{< figure src="/docs/codebox.png" caption="Roboweb makes it easy to copy code into Jupyter cells." alt="Codebox">}}

## Using the extension to fix code

To use the assistant to correct an error, right click on the cell output containing an error.
In the pop up menu, click on the fix option.

{{< figure src="/docs/fixmenu.png" caption="The fix option can be used to fix errors." alt="Codebox">}}

Clicking fix will create an entry in the prompt bar to ask the Ai assistant to fix the error. You can edit the
prompt or submit it directly.

{{< figure src="/docs/fixprompt.png" caption="Roboweb makes it easy to create prompts to fix errors." alt="Codebox">}}
