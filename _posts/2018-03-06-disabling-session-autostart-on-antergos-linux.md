---
layout: post
title: "Disabling autostart session on Antergos Linux"
---

I've looked here at <a href="https://bbs.archlinux.org/viewtopic.php?id=164902" target="_blank">I don't want programs restored after a reboot</a> and over at <a href="https://bbs.archlinux.org/viewtopic.php?id=164354" target="_blank">xfce runs some apps twice at startup</a> for an answer to the question, especially with Antergos, where this behavior has been evident. 

Whether it will be persistent across sessions - no pun intended - it's something that only time will tell. 

Even after reading some pieces of advice from the <a href="https://wiki.archlinux.org/index.php/xfce#Disable_saved_sessions" target="_blank">Disable saved sessions - Arch wiki</a>, only the last `xfconf-query` worked successfully. 

     xfconf-query -c xfce4-session -p /general/SaveOnExit -n -t bool -s false


![](/images/tip-for-xfconfquery.png)


To double check that the settings went to effect, one would have to acess the **xfce4-session.xml** file that should be located at the `.config/xfce4/xfconf/xfce-perchannel-xml/` path. 

One must remember to clear the saved sessions afterwards for the changes to take effect. I don't know if by not doing so, this would have prevented the autostart items from appearing, regardless, and I'm sure one could tweak with the `xfonf-query` further to find out if this is the case. 

![](/images/xfce4-session-preferences-session.png) 

