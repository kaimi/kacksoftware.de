---
layout: post
title: "Linux Kernel 3.8"
date: 2013-04-28 13:02
comments: true
categories: [Linux, Kernel]
---

Nach dem Update auf Kernel 3.8 kommt meine Intel E1000 NIC nicht wieder korrekt aus dem Standby und man muss folgendes als root ausführen damit es wieder geht

{% codeblock %}
echo "on" > /sys/class/net/eth0/device/power/control
{% endcodeblock %}

Das Problem ist wohl gefixt, man muss jetzt auf 3.9 warten oder auf backport hoffen.

Voll gut, nicht! m)
