---
Layout: post
Title: "libzita-resampler.so.1 exists in filesystem"
Date: 2018-02-22 
---

On the most recent upgrade for Arch, some file conflicts prevented the upgrades from going through. 

The message was:

     zita-resampler: libzita-resampler.so.1 already exits in filesystem

Which by looking at the directory `/usr/lib` which contained it, it was a safe assumption that by removing it manually would not cause any harm to the system. 

![](/images/libzita-resampler.png)

But I wanted to make sure nonetheless, and by following good practice I queried a search, which returned that it was not a bug, and that it could be removed from the `/usr/lib`, to let the updates continue. 

For further reading see:

<a href="https://bugs.archlinux.org/task/57602" target="_blank">FS#57602 - [zita-resampler] Conflicting file in upgrade to 1.6.0-2</a>

<a href="https://www.archlinux.org/news/zita-resampler-160-1-2-update-requires-manual-intervention/" target="_blank">zita-resampler 1.6.0-1 -> 2 update requires manual intervention</a>







