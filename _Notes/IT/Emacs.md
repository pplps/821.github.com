---
layout: indexed
title: Emacs 折騰錄
---
本人折騰過若干次 Emacs ，都沒有成功。雖然沒成功實現需要的樣子，不過總是一次比一次好的。由於記憶不佳，所以決定以後記錄一下每次折騰時的心得。  

##2014.10
環境： Windows 7 64 bit, G1620+B75H+8GB  
用 Emacs還是需要比較高的配置的，至少四年前的低配筆記本有點帶不動。  
配置的註釋用 ; 來寫。  
快捷鍵用形如 (global-set-key (kbd "C-x") 'kill-region) 的模式比較好， ErgoEmacs 和 ErgoEmacs Mode 都會嚴重拖慢啓動速度。 ErgoEmacs 配了個簡陋的右鍵菜單。  
Tabbar 是個好插件，可以讓 Emacs 看起來更像一個 Windows 用的軟件。  
可以針對不同字符集設置不同字體。  
顯示行號需要 linum 。  
顏色主題比較煩人，但是網上很多現成貨。  
安裝插件的好方法，相當於 Plugin Manager: M+x list-packages 。
便攜化很簡單，寫個 bat 就行：  
    {% highlight bat %}
    @echo off
    set HOME=%CD%\config
    cd bin
    runemacs
    {% endhighlight %}