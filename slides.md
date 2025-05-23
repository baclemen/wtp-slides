---
# try also 'default' to start simple
theme: dracula
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
wakeLock: "build"
# aspect ratio for the slides
aspectRatio: 16/9
css: unocss
---

# WebTigerPython

## Unleashing Python's Full Potential in the Browser

Clemens Bachmann

---
layout: two-cols-header
---

# Who am I

::left::
- Name: Clemens Bachmann
- Occupation: Software Developer / Educator
  - Algorithms and **didactics** group at ETH
- clemens.bachmann@inf.ethz.ch

::right::
<div>
  <img src="./images/clemi.jpeg" width=150 class="absolute right-50px top-90px"/>
</div>

---
layout: two-cols-header
---

# TigerJython 2012- (A bit of History)

::left::
<v-clicks>

- Many educational libraries for Java
- Jython
- Graphics Libraries
  - Turtle, Games
- Robotics
  - micro:bit, Mindstorms EV3
- Works on any Plattform (Windows, Mac, Linux)
- Easy installation
- Interactive Debugger

</v-clicks>

::right::
<img src="./images/jython.png" alt="drawing" width="100"/>
<br>
<img src="./images/tigerjython.png" alt="drawing" width="350"/>

---
layout: two-cols-header
---

# TigerJython now

::left::
<v-clicks>

- Jython is still at Python 2.7
- Does not work on all Platforms (iPad / Android)
- No support for popular Python libraries written in C (numpy, scipy, matplotlib, pandas)
- Swing UI looks a bit dated

</v-clicks>

::right::
<img src="./images/jython.png" alt="drawing" width="100"/>
<br>
<img src="./images/tigerjython.png" alt="drawing" width="350"/>

---

# Bring TigerJython to the Web

<v-clicks>

- WebAssembly makes it possible to run python in the Browser (Pyodide)
- Web apps really on all plattforms (Windows, Mac, Linux, Android, iPad)
- No installation required
- WebAPIs pathe the way for Robotics in the Web
  - WebBluetooth (2017)
  - WebUSB (2021)
- Critical Requirements
  - Robotics
  - Graphics Libraries
  - Debugger

</v-clicks>

<v-click>

> 🛠️ Features marked with this icon are not deployed yet

</v-click>

---
layout: two-cols-header
---

# Robotics

::left::

<v-clicks>

- WebUSB (micro:bit, calliope_mini)
- Simulation 🛠️
- IoT (oxocard) 🛠️

</v-clicks>

::right::
<img src="./images/maqueen.webp" alt="drawing" width="200"/>

[https://www.mouser.at/new/dfrobot/dfrobot-micro-maqueen-robot/](https://www.mouser.at/new/dfrobot/dfrobot-micro-maqueen-robot/)

<img src="./images/ledring.jpg" alt="drawing" width="200"/>

[https://whadda.com/product/rgb-led-ring-shield-for-microbit-wpse475/](https://whadda.com/product/rgb-led-ring-shield-for-microbit-wpse475/)

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/microbit?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAhjQGMGAjNMptGbPVq8AVEwA6EOoxacANnGJ8BQ0ZMm042OOUSSmBptSF8-EJrSgQA5nAAUAJgAsASj3nDn6mjly7ABgJA_xd9T0MAZzgyAH0FYjs0AiZAlOSARn8QsPCmCIUtOwBWLNCPXJzwsABfAF0gA&device=micro%3Abit&breakpoints=1
---

# Robotics - WebUSB

<v-clicks>

- Single Devices have to be added for WebUSB
  - Auto-connect on plug if registered
- Only in Chrome
- Safari / Firefox declined to implement the feature
  - Many schools work with iPads
  - No real chrome on iPads

</v-clicks>

---
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAhjQGMGAjNMptGbPVq8AVEwA6EOoxacu9Xv0HCmIyZIDOcMgGVscOMQAUARgAMZgJSTacfeUSSmzpgDcASkwC8fWu7QA5gAWZJi2UMQA-sSBPFAANkbWEC5uADLevmlw1KHhUTEBcYmWLk4uaNTp3j5mTFAQxG6eXrWOKaku1EIA7lC0xqUSHc5w8ZXVrUwm9Y3NNUxm7Z0utIEhSSvlo-NVrhlTdQ1NHgsmyytM8Tlkm8OpxGNQuKYWlmAAvgC6QA&device=micro%3Abit
---

# Robotics - Simulation 🛠️

<v-clicks>

- Works on any device
- No robot needed

</v-clicks>

---
layout: iframe-2-cols
url: https://test.webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAnoA96BjKW4ptGbPVpkmAKiYAdCP0HCmqMtgA29MkrQAjHLmWqmUAM5NlZKVIBuUJQFc4RgLxNgAXSkQmjgIwAGb2YjUQnx87rRQEADmcAAUEACUiFJMyUyWSh5MUWQAsmgcDNgAFvQQcAAicByacErRcUkpabYGmFDY2HAQxNFp9e4pZPxwAPqCGGQOTOoGZNFhkTFoANSecX0pxkpkmNRoEda0MbsRBmgAXnD20T4ETACsaw3JJjgqs08bTIPwo_TjBrcPhsmnZAf1PvJuABrOC0ewAcno8LBEOS6lKM1wSku8IAtMjJODPhx6Co4fCNPD1ikXoM1DF4WVyFAqR8XqwlFANDVovDsnBDAc4PAIBNWUSXliuTz4QA1UnWeBMaLEDRxcUbF4RWhoboAFVotmpzy2mAMxQA7nUpGAAL7OIA&device=Oxocard
---

# Robotics - IoT 🛠️

<v-clicks>

- Connection over IoT
- Works on iPad
- Messages are exchanged
  - Does not work without WebTigerPython
  - Not real robotics
  - Oxocard has no wheels

</v-clicks>

---

# Robotics Summary

<v-clicks>

- WebUSB (Chrome only)
- WebBluetooth (Chrome only)
  - We don't support this right now
- No real Chrome on iPads 
  - Chrome on iPad is WebKit (Safari Engine) based
- IoT 🛠️
  - Code runs in Browser
- Simulation works on anything 🛠️

</v-clicks>

---

# Graphics Libraries

<v-clicks>

- Turtle
  - The opposite of a blackbox
  - Intuitive commands (forward, left etc.)
- Pygame
  - Advanced
  - Popular

</v-clicks>

---
layout: two-cols-header
---

# WebTigerPython Architecture

::left::

<v-clicks>

- Python (Pyodide) runs in a Webworker
  - UI does not freeze (single threaded)
- Graphic rendering is done with callbacks
- Pausing execution is done with a SharedArrayBuffer

</v-clicks>

::right::

```mermaid
graph TD
    A[Main Thread] <-->|Interacts with| B[DOM]
    A <-->|postMessage API| C[Web Worker]
    A -->|Accesses| D[SharedArrayBuffer]
    C -->|Accesses| D
style A fill:#ffcc00, color:#000000
style C fill:#ffcc00, color:#000000
```

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAjIFdayAbOJtGbehyYAqADoRxAY3qdBAClFgARp1ZxFASnHiITALy8I2VmQCSEMgrABlNMTgBnRJu0QAxEwBy9Mk1pwoTiYABVwyAAt6CQh_bADfCEQmcSZUpmpBAHcoWmI5AFYABkKmAHomCC1dNNo0AHNwywBmADYS8sqwAF8AXSA
---

# Turtle / Input Function

<v-clicks>

- Webworker is Paused
- SharedBufferArray
- Whole thread is halted
- Callback functions, cannot access DOM

</v-clicks>

---
layout: two-cols-header
---

# WebTigerPython Architecture 2

::left::

<v-clicks>

- pygame-ce was ported to Pyodide with a canvas backend
- Render Graphics off screen in Web Worker
  - offscreenCanvas
  - Introduced for better interactivity

</v-clicks>

::right::

```mermaid
graph TD
    A[Main Thread] <-->|Interacts with| B[DOM]
    A <-->|postMessage API| C[Web Worker]
    A -->|Accesses| D[SharedArrayBuffer]
    C -->|Accesses| D
    B -->|Contains| E[OffscreenCanvas]
    C -->|Accesses| E
style A fill:#ffcc00, color:#000000
style C fill:#ffcc00, color:#000000
```

---
layout: two-cols-header
---

# Asynchronity Problem

::left::

<v-clicks>

- async functions (render updates) are done in the webloop
- It is not possible to synchronously give control to webloop
- asyncio.sleep
  - only in asynchronous contexts
  - async rogramming is not easy

</v-clicks>

::right::

### Synchronous Execution

```mermaid
flowchart LR
    A[Python Execution Pt. 1 & 2] --> C[Render 1]
    C --> D[Render 2]

    style A fill:#ffcc00, color:#000000
    style C fill:#66ccff, color:#000000
    style D fill:#66ccff, color:#000000
```

### Desired Execution Flow

```mermaid
flowchart LR
    A[Python Execution Pt. 1] --> B[Render 1]
    B --> C[Python Execution Pt. 2]
    C --> D[Render 2]

    style A fill:#ffcc00, color:#000000
    style B fill:#66ccff, color:#000000
    style C fill:#ffcc00, color:#000000
    style D fill:#66ccff, color:#000000
```

---

# Asynchronity Example

````md magic-move
```py
from pygame import *

def render():
     #...
    display.flip()
def updateActors():
    #...
    render()
def main():
    while True:
        #...
        updateActors()
main()
```
```py
from pygame import *
import asyncio

async def render():
     #...
    display.flip()
    asyncio.sleep(0)
def updateActors():
    #...
    render()
def main():
    while True:
        #...
        updateActors()
main()
```
```py
from pygame import *
import asyncio

async def render():
     #...
    display.flip()
    asyncio.sleep(0)
async def updateActors():
    #...
    await render()
def main():
    while True:
        #...
        updateActors()
main()
```
```py
from pygame import *
import asyncio

async def render():
     #...
    display.flip()
    asyncio.sleep(0)
async def updateActors():
    #...
    await render()
async def main():
    while True:
        #...
        await updateActors()
await main()
```
````

--> Even harder with class methods

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMNGbAewCcyACPAc1jgB0IeBiZgEkIaMmigAbNAC84zAAq4O8Hu06YMogBQBKHv2YBlOCwCu2ZmQAWc4mgDO2CVFw97AYwZw4EZgF5WJXU7R2dcTHsTAH0YOmI4LR5mZOYtAGYABgyCZkyMvQgCgXkwuAZWBjpsMrE4ex4vdxYAtXhMACU4Jq1s5l6AVgH8_QgBAFl0Xwk6Kp4Adys0CTkAFQZTOEQklPG6ADc5Jxcy7eSAazhce39A5ThMC_C2aOwve0jiXVPmNAAzZke9mArXuAGkogAZACiADEVgBdRDMb4pZiNMiYAAezAAtAF-t8_gDLkCQZhwe1BABxAASCKRKJS6KxzAA1PjCf9AcCgm1wQBVeSI5G-VFMrqYXC4jmi5JE7lk8EAEQA8gB1ABywsZyWZUvZzAJsuYAiVDCgc2YcAODFw1gwbG-Hi8PkwvyWEi0PRyvXyBVRZOI5rmmHRiWNqOd3ggOS0ACZ-v0fT6dDl0f6UoGHEdwr8pNgvsayWI2gBhabuM66TBiStaABs-TAAF94UA
---

# Asyncify Problem Solution

<v-clicks>

- We asyncify code for students
- Fix line numbers in errors
- JavaScript Promise Integrations (JSPI) 
- Experimental Chrome only feature

</v-clicks>

<v-click>

```py
import async
from pyodide.ffi import run_sync

def sync_update(url):
  resp = run_sync(asyncio.sleep(0))
```

</v-click>

---
layout: iframe-2-cols
leftWidth: 25%
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMNGbAewCcyACPAc1jgB0If3PMcAB6xsAGzgBnTFDFo4EaagwAKAJRgAvgF0gA
---

# Pygame Aliens

---
layout: two-cols-header
---

# Debugger

::left::

<v-clicks>

- Pause the execution
- Step by step / breakpoints
- Memory state sent and visualized by the JS frontend
- Inspired by TigerJython debugger / pythontutor.ch

</v-clicks>

::right::

<img src="./images/tigerjythondebugger.jpeg" alt="drawing" width="250"/>

TigerJython Debugger

<img src="./images/pythontutor.png" alt="drawing" width="250"/>

[https://pythontutor.com/](https://pythontutor.com/)


---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAMwCcB7GAAjIFdayAbOJtGbehyYAqADoRx1NJ04Bjep0EAKUSigBzOBAqqAlOOxb5i2irWbtUPeIBGcdRgD6UmUv0RacQ-SYBWROJMQUzUxEoAjABsAAzuwUwcEQAsSe5axM7SnG5gAL4AukA
---

# Debugger Turtle

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAHQmLgDMACBtAIwAoIBKRWpgUzTMITADwBeJgAY-owQoBOcMgFdFo6U36C4AG2FNREqQEY5CpSvWjT2-QP0BnOBcsDlajS3ZcmAWiZTbiYAah9OUUCAJhDaWmMmABZaZSdVPTImKVZI7lpsRQwyDjSMsm4wAF8AXS
---

# Debugger Recursion

- Every scope is displayed

---
layout: iframe-2-cols
url: https://webtigerpython.ethz.ch/?code=NobwRAdghgtgpmAXGGUCWEB0AHAnmAGjABMoAXKJMAYwBsoBnBgAgAU4AnBgewkQB0IzZsTgAzZgH1JGNGWkAKBnFpiCzaPHVQA5nACUAocObLVmTXGYBeDbDiCTplWMy6rt94MHYAjDbZOHggFfjAAKW4ACwgw9QBmADZ9bwhsDgwyBT8LexS0jIgsnPd9ZjAAXwBdIA
---

# Debugger Classes

---
layout: two-cols-header
---

# Debugger Overview

::left::
Dictionaries
<img src="./images/debugger_dict.png" alt="drawing" width="350"/>
Self Referencing Lists
<img src="./images/debugger_self_ref.png" alt="drawing" width="350"/>

::right::
Nested Lists
<img src="./images/debugger_nested_lists.png" alt="drawing" width="350"/>

---

# Conclusion

- Most things do work in the browser
- Except for iPads, all Features to Work on any device
  - Not on any browser (Firefox/Safari)
- Try it out at [wtp.ethz.ch](https://webtigerpython.ethz.ch)
- Coding exercises [python-online.ch](https://python-online.ch)

# Outlook

- Bluetooth Robotics
- Multifile
- Open Source