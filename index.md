---
layout: default
title: Welcome
---

<!-- Hero Section -->
<div style="text-align:center; padding:40px 10px;">
    <img src="/assets/images/ban.png" alt="Welcome" style="width:65%; max-width:850px; border-radius:12px; margin-bottom:25px;">
    <h1 style="margin-bottom:10px;">Cloud & Network Engineering Blog</h1>
    <p style="font-size:18px; opacity:0.8;">
        Routing • Cloud • Linux • IoT • Security • eBPF
    </p>

    <!-- Tags -->
    <div style="margin-top:15px;">
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">BGP</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">OSPF</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">AWS</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">Linux</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">IoT</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">Suricata</span>
        <span style="background:#6c63ff; color:white; padding:6px 12px; border-radius:16px; margin:3px; font-size:12px;">eBPF/XDP</span>
    </div>
</div>


<!-- Intro Text -->
<div style="max-width:750px; margin:0 auto; font-size:17px; line-height:1.65;">
    <p>
        This website is both my <strong>technical blog</strong> and my <strong>engineering portfolio</strong>.
        Here I document network architectures, cloud labs, SOC pipelines, IoT systems, and Linux kernel networking.
    </p>

    <p>
        I write about:
    </p>
    <ul>
        <li>ISP & routing architectures</li>
        <li>Cloud networking (AWS, hybrid interconnects)</li>
        <li>IoT & IPv6 networks</li>
        <li>Security engineering (IDS, SIEM, MITRE ATT&CK)</li>
        <li>Linux kernel networking (eBPF/XDP)</li>
    </ul>
</div>


<!-- Latest Articles -->
<div style="max-width:750px; margin:60px auto;">
    <h2>🔥 Latest Articles</h2>
    <ul>
      {% for post in site.posts limit:5 %}
        <li style="margin-bottom:10px;">
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span style="opacity:0.6;">— {{ post.date | date: "%B %d, %Y" }}</span>
        </li>
      {% endfor %}
    </ul>
    <a href="/articles/" style="display:inline-block; margin-top:10px; background:#6c63ff; color:white; padding:8px 14px; border-radius:6px; text-decoration:none; font-size:14px;">
        View All Articles →
    </a>
</div>


<!-- Featured Projects -->
<div style="max-width:750px; margin:60px auto;">
    <h2>🚀 Featured Projects</h2>

    <ul style="list-style:none; padding-left:0;">

        <li style="margin-bottom:20px;">
            <strong><a href="/projects/isp-network-lab/">ISP / Enterprise / Cloud Multi-AS Architecture</a></strong><br>
            <span style="opacity:0.7;">OSPF • BGP • HSRP • VLANs • Tunnels • HA routing</span>
        </li>

        <li style="margin-bottom:20px;">
            <strong><a href="/projects/iotbox/">IoTBox – Virtual IoT Edge Gateway</a></strong><br>
            <span style="opacity:0.7;">FRR • nftables • DHCPv6 • Suricata • Flask API</span>
        </li>

        <li style="margin-bottom:20px;">
            <strong><a href="/projects/soc-wazuh-suricata/">SOC Detection Lab (Wazuh + Suricata + APT-28)</a></strong><br>
            <span style="opacity:0.7;">MITRE ATT&CK • CVE exploitation • CALDERA</span>
        </li>

    </ul>

    <a href="/projects/" style="display:inline-block; margin-top:10px; background:#6c63ff; color:white; padding:8px 14px; border-radius:6px; text-decoration:none; font-size:14px;">
        View All Projects →
    </a>
</div>
