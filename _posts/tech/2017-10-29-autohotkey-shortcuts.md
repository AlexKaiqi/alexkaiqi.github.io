---
title: AutoHotKey Useful ShortCuts
date: 2017-10-29 08:58:26
tags: autohotkey
---

## Start a program
```script
!q:: run, C:\Users\alexk\Documents\WinApp ShortCut\QQ
return
```

## Search selected text in default browser
```script
; search lighlight text in default browser
^+c:: ; ctrl shift + c
{
 Send, ^c
 Sleep 50
 Run, http://www.google.com/search?q=%clipboard%
 Return
}
```

## Open file with specified program
```script
; Open file with specified program
^j:: ; ctrl + j
Clipboard =
Send ^c
ClipWait ;waits for the clipboard to have content
Run, C:\Users\alexk\AppData\Local\atom\atom.exe %clipboard%
```

## Windows always on top, stroke again to disable
```script
; Windows always on Top
^SPACE:: Winset, Alwaysontop, , A ; ctrl + space
Return
```

## Launch web app
```script
; Launch Chrome app exp. MakeTechEasier, you need set up chrome as default browser first
^+t::Run "www.maketecheasier.com" ; use ctrl+Shift+t
return
```

## Move up a folder in explorer
```script
; Press ~ to move up a folder in Explorer
#IfWinActive, ahk_class CabinetWClass
`::Send !{Up}
#IfWinActive
return
```

## Custom volume buttons
```script
; Custom volume buttons
+NumpadAdd:: Send {Volume_Up} ;shift + numpad plus
+NumpadSub:: Send {Volume_Down} ;shift + numpad minus
break::Send {Volume_Mute} ; Break key mutes
return
```

## Suspend AutoHotKey
```script
; Suspend AutoHotKey
#ScrollLock::Suspend ; Win + scrollLock
return
```

## Insert a text to editor
```script
; Insert jekyll blog front matter to editor
!+f::
; IfWinActive, ahk_group textEditors ; create a group in the auto execute section
FormatTime, time, A_now, yyyy-MM-dd HH:mm:ss ; format current time
SendInput,
(
---
istop: true
title:
date: %time%
background-image: ../style/images/
category:
tags:
---
)
return
```

## Insert current time to editor
```script
; Insert current time to
!+t::
FormatTime, time, A_now, yyyy-MM-dd HH:mm:ss
sendInput %time%
return
```
