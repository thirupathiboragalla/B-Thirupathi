# B-Thirupathi
i got a problem while running python code in atom. can anyone please help?
[Enter steps to reproduce:]

1. ...
2. ...

**Atom**: 1.45.0 ia32
**Electron**: 4.2.7
**OS**: Microsoft Windows 10 Pro
**Thrown From**: [script](https://github.com/rgbkrk/atom-script) package 3.25.0


### Stack Trace

Uncaught TypeError: Cannot read property 'remove' of undefined

```
At C:\Users\like\.atom\packages\script\node_modules\atom-message-panel\lib\MessagePanelView.js:189

TypeError: Cannot read property 'remove' of undefined
    at ScriptView.MessagePanelView.remove (/packages/script/node_modules/atom-message-panel/lib/MessagePanelView.js:189:30)
    at ScriptView.detach (/packages/script/node_modules/jquery/dist/jquery.js:5357:15)
    at ScriptView.removePanel (/packages/script/lib/script-view.js:89:10)
    at Object.closeScriptViewAndStopRunner (/packages/script/lib/script.js:161:21)
    at HTMLElement.scriptCloseView (/packages/script/lib/script.js:94:39)
    at CommandRegistry.handleCommandEvent (~/AppData/Local/atom/app-1.45.0/resources/app/static/<embedded>:11:349290)
    at CommandRegistry.dispatch (~/AppData/Local/atom/app-1.45.0/resources/app/static/<embedded>:11:347765)
    at ScriptView.close (/packages/script/lib/script-view.js:99:19)
    at /packages/script/node_modules/space-pen/lib/space-pen.js:220:36)
    at HTMLDivElement.dispatch (/packages/script/node_modules/jquery/dist/jquery.js:4435:9)
    at HTMLDivElement.elemData.handle (/packages/script/node_modules/jquery/dist/jquery.js:4121:28)
```

### Commands

```
 15x -3:10 core:move-right (input.hidden-input)
  2x -3:05.5.0 core:move-left (input.hidden-input)
     -3:02.2.0 core:backspace (input.hidden-input)
  6x -2:59.9.0 core:move-left (input.hidden-input)
     -2:56.7.0 core:backspace (input.hidden-input)
     -2:52.6.0 editor:move-to-end-of-screen-line (input.hidden-input)
     -2:48.8.0 core:save (input.hidden-input)
     -2:45 script:run (input.hidden-input)
  5x -2:23.2.0 core:backspace (input.hidden-input)
  6x -1:44.2.0 core:delete (input.hidden-input)
     -1:40.7.0 core:backspace (input.hidden-input)
  2x -1:36.3.0 core:move-right (input.hidden-input)
     -1:34.2.0 core:save (input.hidden-input)
     -1:30.3.0 core:backspace (input.hidden-input)
     -1:29 script:run (input.hidden-input)
     -0:45.4.0 script:close-view (atom-workspace.workspace.scrollbars-visible-always.theme-one-dark-syntax.theme-one-dark-ui)
```

### Non-Core Packages

```
atom-python-run 0.9.7 
script 3.25.0 
```


