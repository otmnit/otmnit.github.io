---
layout: default
title: Welcome
---

![Alt text](welcome.png)

This website is both my **technical blog** and my **portfolio**.

I write about:
- ISP & routing architectures  
- Cloud networking (AWS, hybrid interconnects)  
- IoT & IPv6  
- Security engineering (IDS, SIEM, MITRE ATT&CK)  
- Linux kernel networking (eBPF/XDP)  

---

## 🔥 Latest Articles
<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>

