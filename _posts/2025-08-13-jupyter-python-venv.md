---
title: Jupyter Problems in Python Environment
author: scott_gromme
date: 2025-08-13 09:10:00 +0000
categories: [Python Environment, VSC]
tags: [ development]
render_with_liquid: false
mermaid: true
---

# Problem

The Jupyter Notebooks freezes when run in Visual Studio Code.  It runs when run from the local Jupyter web page.

System:
1. Ubuntu
2. Python3 venv
3. Visual Studion Code
4. 'jupyter' was install with pip in the Python virtual ( module venv)

# Analysis

Juypter Notebook install seems to need Conda to be installed.  After deleting the environment and reinstall 'ipykernel' the VSC notebook will run.  It still wants 'Conda' but does run.


# Solution

1. Delete the Python environment
2. Install with Pip 'ipykernel' instead of 'juypter'

Juypter Notebooks is still looling for 'Conda' but it at least runs in VSC.

# Apendix

## A


![Desktop View](assets/img/posts/pythonenvironments.png){: width="972" height="589" }
_Message from VSC_



```env
pip install ipykernel 
```

Messages in the Python environment.

```
2025-08-13 12:00:56.612 [info] Telemetry:  {"event":"RefreshPerformance","data":{"refreshPerformance":{"total":2847,"breakdown":{"GlobalVirtualEnvs":3,"Locators":2847,"Path":771,"Workspaces":163},"locators":{"Conda":2846,"Homebrew":0,"LinuxGlobal":19,"PipEnv":0,"Pixi":0,"Poetry":56,"PyEnv":52,"Venv":0,"VirtualEnv":0,"VirtualEnvWrapper":0}}}}

2025-08-13 12:00:56.709 [info] Terminal is activated: /home/sgromme/source/dynamic/.venv/bin/python

2025-08-13 12:00:56.762 [info] Terminal is activated: /home/sgromme/source/dynamic/.venv/bin/python

2025-08-13 12:18:07.279 [error] Error refreshing packages A system error occurred (spawn ENOTDIR)
```

