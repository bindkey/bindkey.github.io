---
layout : post
title : "Manjaro Xfce Bluetooth Problem"
date : "2017-09-29T13:32:01-05:00"
---
 <p>Bluetooth recognition - at least on Manjaro Xfce - has been erratic and inconsistent.</p>

<p>For no clear reason the LTS kernel and even a newer kernel have identified the hardware, while it has failed to do so in a great many occasions.</p>

<p>Many of the tweaks included reinstalling <code>bluez</code>, <code>bluez-firmware</code>, <code>bluez-libs</code>, <code>bluez-tools</code>, and <code>bluez-utils</code>.</p>

<p>Back to the drawing room and back again.</p>

<p>The bluetooth adapters were not being recognized however. And after logging out and back into the session, and even after <code>sudo /sbin/shutdown -r now</code>, nothing seemed to work.</p>

<p>The following day - to my surprise - I booted the system and it picked the bluetooth adapters without a problem.</p>

<p>It reminded me of a comment on the manjaro forum thread entitled <a href="https://forum.manjaro.org/t/bluetooth-adapters-app-not-opening-bluetooth-manager-bluez-failed/4367/19" target="_blank">Bluetooth adapters app not opening Bluetooth Manager</a> in which one of the participants said:</p>

<blockquote>
<p>Bluetooth support in Linux is always troublesome, even in Windows, smartphone, etc. So yeah, I think staying away from bluetooth related hardwares if you want a trouble free experience. Wireless hardwares nowadays are going towards a dedicated receiver way to handle wireless connection and that’s a better approach. Just my two cents <a href="#blueref"><sup id="bluerefsup">1</sup></a></p>
</blockquote>

<p>I have to agree with him on that regard.</p>

<p>On the other hand, the desktop environment <strong>KDE</strong> hasn’t - I ran it for a short while and perhaps my feedback is worthless of consideration on that regard - given me the same problems than the current configuration under <strong>xfce</strong>.</p>

<p>But I never thought that the problems would persist even after the installation of a newer kernel. That is perhaps the main reason which has been drifting me away from <strong>xfce</strong> until further notice.</p>

<p>And while <strong>KDE</strong>-fanboys have come up with the slogan that <em>it grows on you</em>, <strong>xfce</strong> is perhaps a more GNU/Linux-centric configurable environment than the former. I still enjoy tweaking with its features even though its less polished than Plasma <strong>KDE</strong>. There is no question about this. <strong>KDE</strong> aims at the latest hardware, while <strong>xfce</strong> focuses on the rest. I’ve never tried to benchmark its memory and CPU consumption, but I’m almost certain it fairs much better than <strong>KDE</strong>.</p>

<p>Whether <strong>xfce</strong> will be a daily desktop environment driver running the main programs on which my workflow depends upon, it’s a question of time and how well it will handle them without a major setback.</p>

<p><strong>References</strong></p>

<p><a name="blueref"></a><a href="https://forum.manjaro.org/t/bluetooth-adapters-app-not-opening-bluetooth-manager-bluez-failed/4367/19" target="_blank">bluetooth adapters not opening bluetooth-manager-bluez-failed</a><a href="#bluerefsup">_↩︎</a></p>
