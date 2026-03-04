# Pragmatic-CSS
Pragmatic HTML/CSS snippets for grok.com

# Nice ones

<img width="965" height="245" alt="image" src="https://github.com/user-attachments/assets/58613b2d-a293-4e16-900e-d5e2660efd0a" />

```html
<!-- ============== HEADER-NAV ===================== -->
<div style="width: 100%; background: linear-gradient(90deg, #1e293b, #0f172a); border-left: 4px solid #8b5cf6; padding: 14px 18px; border-radius: 6px; margin: 16px 0; box-sizing: border-box; font-family: monospace;">
  <span style="font-size: 19px; font-weight: bold; color: #e0f2fe; letter-spacing: 0.8px; text-shadow: 0 0 6px rgba(139, 92, 246, 0.4);">
    TEST SUITE — ULTIMATE-HTML v1
  </span>
  <div style="margin-top: 8px; font-size: 14px; color: #94a3b8;">
    Four interactive components. Zero JS. Pure CSS + native HTML.
  </div>
</div>
```
---
<img width="624" height="128" alt="image" src="https://github.com/user-attachments/assets/6625c611-5600-48f7-8818-31e65f698ddf" />

```html
<!-- =============== FOOTER NAV ===================== -->
<div style="margin: 32px 0; font-family: system-ui, -apple-system, sans-serif; color: #e5e7eb;">
<div class="card css ui access" style="padding:16px; background:#111827; border:1px solid #374151; border-radius:8px; display:block;">
  <strong>Focusable Custom Checkbox</strong><br>
  CSS + UI + Accessibility
</div>
```
---
<img width="404" height="97" alt="image" src="https://github.com/user-attachments/assets/114ce6c1-f57a-4ff4-a88e-5a37bdb98a2c" />

```html
<!-- =============== BUTTONS ===================== -->
<div style="margin: 32px 0; font-family: system-ui, -apple-system, sans-serif; color: #e5e7eb;">

  <!-- Chipki / filtry – 8 sztuk -->
  <div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 24px; max-width: 100%;">
    <input type="checkbox" id="f-js"     style="display:none;">
    <label for="f-js"     style="cursor:pointer; padding:8px 16px; background:#1e293b; color:#94a3b8; border-radius:999px; font-size:13.5px; border:1px solid #334155; transition:all 0.16s; user-select:none; white-space:nowrap;">JavaScript</label>

    <input type="checkbox" id="f-css"    style="display:none;">
    <label for="f-css"    style="cursor:pointer; padding:8px 16px; background:#1e293b; color:#94a3b8; border-radius:999px; font-size:13.5px; border:1px solid #334155; transition:all 0.16s; user-select:none; white-space:nowrap;">CSS / HTML</label>
```
---
<img width="794" height="559" alt="image" src="https://github.com/user-attachments/assets/c4a3b3c4-1f0d-4549-aea5-6c03b51114b8" />

```html
<!-- =============== DASHBOARD ===================== -->
<div style="width:100%; max-width:600px; margin:40px auto; padding:32px 28px; background:#0f172a; border-radius:12px; border:1px solid #334155; font-family:system-ui, sans-serif; color:#e2e8f0; box-sizing:border-box;">
  <div style="font-size:28px; font-weight:700; color:#cbd5e1; letter-spacing:-0.5px; margin-bottom:16px;">
    Dashboard
  </div>

  <div style="font-size:15px; color:#94a3b8; line-height:1.6; margin-bottom:24px;">
    Status wszystkich systemów: nominalny<br>
    Ostatnia aktualizacja: 04.03.2026 07:37 CET
  </div>

  <div style="display:grid; grid-template-columns:1fr 1fr; gap:16px; margin-bottom:24px;">
    <div style="padding:16px; background:#1e293b; border-radius:8px; border:1px solid #334155;">
      <div style="font-size:14px; color:#94a3b8; margin-bottom:4px;">CPU</div>
      <div style="font-size:20px; font-weight:600; color:#60a5fa;">12%</div>
    </div>
    <div style="padding:16px; background:#1e293b; border-radius:8px; border:1px solid #334155;">
      <div style="font-size:14px; color:#94a3b8; margin-bottom:4px;">Memory</div>
      <div style="font-size:20px; font-weight:600; color:#34d399;">4.2 GB / 32 GB</div>
    </div>
  </div>

  <div style="padding:16px; background:#1e293b; border-radius:8px; border:1px solid #334155;">
    <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Ostatnie logi</div>
    <div style="font-size:13px; font-family:ui-monospace, monospace; color:#cbd5e1; line-height:1.5;">
      [07:37] INFO  Server heartbeat OK<br>
      [07:36] INFO  Cache cleared successfully<br>
      [07:35] DEBUG Query executed in 42ms
    </div>
  </div>
</div>u dla każdego filtra -->
    <style>
      #f-js:checked     + label { background:#f97316 !important; color:#fff !important; border-color:#fb923c !important; box-shadow:0 0 10px rgba(249,115,22,0.35); }
      #f-css:checked    + label { background:#06b6d4 !important; color:#fff !important; border-color:#22d3ee !important; box-shadow:0 0 10px rgba(6,182,212,0.35); }
      #f-react:checked  + label 
      /* Domyślny reset – gdy nic nie zaznaczone → wszystko widać */
      #f-js:not(:checked) ~ #f-css:not(:checked) ~ #f-react:not(:checked) ~ #f-ui:not(:checked) ~
      #f-hack:not(:checked) ~ #f-access:not(:checked) ~ #f-perf:not(:checked) ~ #f-anim:not(:checked) ~ .card {
        display: block !important;
      }
    </style>
  </div>
```

---

**Nowy typ 1 – Compact Metric Cards z subtle progress ring (statyczny SVG)**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">
    Core Metrics
  </div>

  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(180px, 1fr)); gap:20px;">
    <div style="text-align:center; padding:20px; background:#1e293b; border-radius:10px; border:1px solid #334155; position:relative;">
      <svg width="80" height="80" viewBox="0 0 80 80" style="margin-bottom:12px;">
        <circle cx="40" cy="40" r="36" fill="none" stroke="#334155" stroke-width="8"/>
        <circle cx="40" cy="40" r="36" fill="none" stroke="#60a5fa" stroke-width="8" stroke-dasharray="226" stroke-dashoffset="180" transform="rotate(-90 40 40)"/>
      </svg>
      <div style="font-size:28px; font-weight:600; color:#60a5fa;">22%</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">CPU</div>
    </div>

    <div style="text-align:center; padding:20px; background:#1e293b; border-radius:10px; border:1px solid #334155; position:relative;">
      <svg width="80" height="80" viewBox="0 0 80 80" style="margin-bottom:12px;">
        <circle cx="40" cy="40" r="36" fill="none" stroke="#334155" stroke-width="8"/>
        <circle cx="40" cy="40" r="36" fill="none" stroke="#34d399" stroke-width="8" stroke-dasharray="226" stroke-dashoffset="140" transform="rotate(-90 40 40)"/>
      </svg>
      <div style="font-size:28px; font-weight:600; color:#34d399;">38%</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Memory</div>
    </div>

    <div style="text-align:center; padding:20px; background:#1e293b; border-radius:10px; border:1px solid #334155; position:relative;">
      <svg width="80" height="80" viewBox="0 0 80 80" style="margin-bottom:12px;">
        <circle cx="40" cy="40" r="36" fill="none" stroke="#334155" stroke-width="8"/>
        <circle cx="40" cy="40" r="36" fill="none" stroke="#fbbf24" stroke-width="8" stroke-dasharray="226" stroke-dashoffset="90" transform="rotate(-90 40 40)"/>
      </svg>
      <div style="font-size:28px; font-weight:600; color:#fbbf24;">60%</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Disk</div>
    </div>
  </div>
</div>
```

**Nowy typ 2 – Vertical Timeline / Event Stream (z linią łączącą)**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0; position:relative;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">
    Event Timeline
  </div>

  <div style="position:relative; padding-left:32px;">
    <div style="position:absolute; left:12px; top:0; bottom:0; width:2px; background:#334155;"></div>

    <div style="position:relative; margin-bottom:28px;">
      <div style="position:absolute; left:-32px; width:24px; height:24px; background:#0f172a; border:3px solid #60a5fa; border-radius:50%; box-shadow:0 0 12px rgba(96,165,250,0.2);"></div>
      <div style="font-size:15px; font-weight:600; color:#60a5fa;">07:45</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Heartbeat acknowledged – all nodes healthy</div>
    </div>

    <div style="position:relative; margin-bottom:28px;">
      <div style="position:absolute; left:-32px; width:24px; height:24px; background:#0f172a; border:3px solid #34d399; border-radius:50%; box-shadow:0 0 12px rgba(52,211,153,0.2);"></div>
      <div style="font-size:15px; font-weight:600; color:#34d399;">07:42</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Cache rotation completed successfully</div>
    </div>

    <div style="position:relative; margin-bottom:28px;">
      <div style="position:absolute; left:-32px; width:24px; height:24px; background:#0f172a; border:3px solid #fbbf24; border-radius:50%; box-shadow:0 0 12px rgba(251,191,36,0.2);"></div>
      <div style="font-size:15px; font-weight:600; color:#fbbf24;">07:38</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Query optimization applied (–18% response time)</div>
    </div>

    <div style="position:relative;">
      <div style="position:absolute; left:-32px; width:24px; height:24px; background:#0f172a; border:3px solid #a78bfa; border-radius:50%; box-shadow:0 0 12px rgba(167,139,250,0.2);"></div>
      <div style="font-size:15px; font-weight:600; color:#a78bfa;">07:35</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">New session started: @Sernik_Js</div>
    </div>
  </div>
</div>
```

**Nowy typ 3 – Compact Key-Value List (z kopiowalnym stylem)**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:20px;">
    Node Configuration
  </div>

  <div style="display:grid; grid-template-columns:1fr 2fr; gap:12px 20px; font-size:14px;">
    <div style="color:#94a3b8; font-weight:500; text-align:right;">Hostname</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px; font-family:ui-monospace, monospace;">node-hannover-03</div>

    <div style="color:#94a3b8; font-weight:500; text-align:right;">IP</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px; font-family:ui-monospace, monospace;">172.16.42.117</div>

    <div style="color:#94a3b8; font-weight:500; text-align:right;">OS</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px;">Ubuntu 24.04 LTS</div>

    <div style="color:#94a3b8; font-weight:500; text-align:right;">Kernel</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px; font-family:ui-monospace, monospace;">6.8.0-31-generic</div>

    <div style="color:#94a3b8; font-weight:500; text-align:right;">Docker</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px; color:#34d399;">v27.3.1 (running)</div>

    <div style="color:#94a3b8; font-weight:500; text-align:right;">Location</div>
    <div style="background:#1e293b; padding:8px 12px; border-radius:6px;">Hannover, DE</div>
  </div>
</div>
```

**Nowy typ 4 – Status Badge Grid z emoji akcentami**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">
    Service Status
  </div>

  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(160px, 1fr)); gap:16px;">
    <div style="padding:16px; background:#1e293b; border-radius:10px; border:1px solid #334155; text-align:center;">
      <div style="font-size:32px; margin-bottom:8px;">🟢</div>
      <div style="font-size:15px; font-weight:500; color:#34d399;">API Gateway</div>
      <div style="font-size:13px; color:#94a3b8; margin-top:4px;">Healthy</div>
    </div>

    <div style="padding:16px; background:#1e293b; border-radius:10px; border:1px solid #334155; text-align:center;">
      <div style="font-size:32px; margin-bottom:8px;">🟢</div>
      <div style="font-size:15px; font-weight:500; color:#34d399;">Database</div>
      <div style="font-size:13px; color:#94a3b8; margin-top:4px;">Healthy</div>
    </div>

    <div style="padding:16px; background:#1e293b; border-radius:10px; border:1px solid #334155; text-align:center;">
      <div style="font-size:32px; margin-bottom:8px;">🟡</div>
      <div style="font-size:15px; font-weight:500; color:#fbbf24;">Redis Cache</div>
      <div style="font-size:13px; color:#94a3b8; margin-top:4px;">High latency</div>
    </div>

    <div style="padding:16px; background:#1e293b; border-radius:10px; border:1px solid #334155; text-align:center;">
      <div style="font-size:32px; margin-bottom:8px;">🟢</div>
      <div style="font-size:15px; font-weight:500; color:#34d399;">Frontend CDN</div>
      <div style="font-size:13px; color:#94a3b8; margin-top:4px;">Healthy</div>
    </div>

    <div style="padding:16px; background:#1e293b; border-radius:10px; border:1px solid #334155; text-align:center;">
      <div style="font-size:32px; margin-bottom:8px;">🔴</div>
      <div style="font-size:15px; font-weight:500; color:#dc2626;">Backup Queue</div>
      <div style="font-size:13px; color:#94a3b8; margin-top:4px;">Delayed</div>
    </div>
  </div>
</div>
```

**Nowy typ 5 – Simple Horizontal Scrollable Tags / Categories**

html```
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:20px;">
    Active Components
  </div>

  <div style="overflow-x:auto; white-space:nowrap; padding-bottom:8px; scrollbar-width:thin;">
    <div style="display:inline-flex; gap:12px;">
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">Frontend</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">API Layer</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">Database</span>
      <span style="padding:8px 18px; background:#253549; border-radius:999px; font-size:14px; color:#60a5fa; border:1px solid #4b5563; font-weight:500;">Auth Service</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">Queue</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">Monitoring</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">Logging</span>
      <span style="padding:8px 18px; background:#1e293b; border-radius:999px; font-size:14px; color:#94a3b8; border:1px solid #334155;">CI/CD</span>
    </div>
  </div>

  <div style="margin-top:20px; font-size:14px; color:#94a3b8;">
    Scroll horizontally to see more categories
  </div>
</div>
```

**Nowy typ 6 – Compact Two-Column Config / Info Block**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:20px;">
    Node Information
  </div>

  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(280px, 1fr)); gap:24px;">
    <div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px; font-weight:500;">General</div>
      <div style="background:#1e293b; border-radius:8px; padding:16px; border:1px solid #334155;">
        <div style="margin-bottom:12px;"><strong>Hostname:</strong> <span style="font-family:monospace;">node-hannover-03</span></div>
        <div style="margin-bottom:12px;"><strong>Location:</strong> Hannover, DE</div>
        <div><strong>Provider:</strong> Hetzner Cloud</div>
      </div>
    </div>

    <div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px; font-weight:500;">Resources</div>
      <div style="background:#1e293b; border-radius:8px; padding:16px; border:1px solid #334155;">
        <div style="margin-bottom:12px;"><strong>CPU:</strong> AMD EPYC 7763 64-Core</div>
        <div style="margin-bottom:12px;"><strong>RAM:</strong> 128 GB DDR4 ECC</div>
        <div><strong>Storage:</strong> 2× 1.92 TB NVMe SSD</div>
      </div>
    </div>
  </div>
</div>
```

**Nowy typ 7 – Compact Alert Banner z priorytetem**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:24px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="display:flex; align-items:center; gap:16px; flex-wrap:wrap;">
    <div style="padding:12px 20px; background:#dc2626; color:#fee2e2; border-radius:8px; font-size:15px; font-weight:600;">
      Critical
    </div>
    <div style="flex:1; min-width:200px;">
      <div style="font-size:17px; font-weight:600; margin-bottom:4px;">Backup Service Delayed</div>
      <div style="font-size:14px; color:#fca5a5;">
        Last successful backup: 48h ago • Investigating
      </div>
    </div>
    <div style="font-size:13px; color:#fca5a5; opacity:0.9;">
      07:52 CET
    </div>
  </div>
</div>

<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:24px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="display:flex; align-items:center; gap:16px; flex-wrap:wrap;">
    <div style="padding:12px 20px; background:#d97706; color:#fef3c7; border-radius:8px; font-size:15px; font-weight:600;">
      Warning
    </div>
    <div style="flex:1; min-width:200px;">
      <div style="font-size:17px; font-weight:600; margin-bottom:4px;">High Memory Usage on node-04</div>
      <div style="font-size:14px; color:#fde68a;">
        78% – threshold 75% • Monitoring
      </div>
    </div>
    <div style="font-size:13px; color:#fde68a; opacity:0.9;">
      07:48 CET
    </div>
  </div>
</div>
```

**Nowy typ 8 – Minimalistyczny Progress Overview (bardzo płaski, bez SVG)**


```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">
    Daily Progress
  </div>

  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(180px, 1fr)); gap:20px;">
    <div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Requests Handled</div>
      <div style="height:6px; background:#334155; border-radius:3px; overflow:hidden; margin-bottom:6px;">
        <div style="width:92%; height:100%; background:#60a5fa;"></div>
      </div>
      <div style="font-size:18px; font-weight:600; color:#60a5fa;">184k / 200k</div>
    </div>

    <div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Error Rate</div>
      <div style="height:6px; background:#334155; border-radius:3px; overflow:hidden; margin-bottom:6px;">
        <div style="width:0.4%; height:100%; background:#34d399;"></div>
      </div>
      <div style="font-size:18px; font-weight:600; color:#34d399;">0.42%</div>
    </div>

    <div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Cache Hit</div>
      <div style="height:6px; background:#334155; border-radius:3px; overflow:hidden; margin-bottom:6px;">
        <div style="width:97%; height:100%; background:#a78bfa;"></div>
      </div>
      <div style="font-size:18px; font-weight:600; color:#a78bfa;">97.3%</div>
    </div>
  </div>
</div>
```

**Nowy typ 9 – Subtle Card Stack (efekt lekkiego nakładania)**

```html
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:32px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0; position:relative;">
  <div style="position:relative; z-index:3; background:#1e293b; border:1px solid #334155; border-radius:10px; padding:24px; box-shadow:0 10px 30px rgba(0,0,0,0.4);">
    <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:16px;">
      Active Session
    </div>
    <div style="font-size:15px; color:#94a3b8; line-height:1.6;">
      User: <strong style="color:#e2e8f0;">@Sernik_Js</strong><br>
      Location: Hannover, DE<br>
      Device: Desktop • Chrome 134<br>
      Login: 06:12 CET • 1h 43m ago
    </div>
  </div>

  <div style="position:absolute; top:12px; left:12px; right:12px; height:100%; background:#1e293b; border:1px solid #334155; border-radius:10px; opacity:0.6; z-index:2; transform:scale(0.98);"></div>
  <div style="position:absolute; top:24px; left:24px; right:24px; height:100%; background:#1e293b; border:1px solid #334155; border-radius:10px; opacity:0.3; z-index:1; transform:scale(0.96);"></div>
</div>
```

**Nowy typ 10 – Very Flat Footer / Summary Bar**

```html
<div style="width:100%; background:#0f172a; border-top:1px solid #334155; padding:20px 28px; font-family:system-ui,sans-serif; color:#94a3b8; font-size:14px; display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:16px; margin:32px 0;">
  <div>
    © 2026 Sernik Systems • Hannover
  </div>
  <div style="display:flex; gap:24px;">
    <span>Status: <strong style="color:#34d399;">Operational</strong></span>
    <span>Uptime: <strong style="color:#60a5fa;">19d 8h</strong></span>
    <span>Version: <strong>v4.2.1</strong></span>
  </div>
</div>
```

```html
<!-- Typ 11 – Subtle Notification Stack -->
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:20px;">Notifications</div>
  <div style="display:flex; flex-direction:column; gap:12px;">
    <div style="padding:14px 18px; background:#1e293b; border-left:4px solid #34d399; border-radius:6px; display:flex; align-items:center; gap:16px;">
      <div style="font-size:20px;">🟢</div>
      <div>
        <div style="font-size:15px; font-weight:500; color:#34d399;">Cache cleared</div>
        <div style="font-size:13px; color:#94a3b8;">07:58 CET • Manual action</div>
      </div>
    </div>
    <div style="padding:14px 18px; background:#1e293b; border-left:4px solid #60a5fa; border-radius:6px; display:flex; align-items:center; gap:16px;">
      <div style="font-size:20px;">ℹ️</div>
      <div>
        <div style="font-size:15px; font-weight:500; color:#60a5fa;">New version available</div>
        <div style="font-size:13px; color:#94a3b8;">v4.2.2 • Check changelog</div>
      </div>
    </div>
    <div style="padding:14px 18px; background:#1e293b; border-left:4px solid #fbbf24; border-radius:6px; display:flex; align-items:center; gap:16px;">
      <div style="font-size:20px;">⚠️</div>
      <div>
        <div style="font-size:15px; font-weight:500; color:#fbbf24;">Memory approaching limit</div>
        <div style="font-size:13px; color:#94a3b8;">74% • 07:55 CET</div>
      </div>
    </div>
  </div>
</div>
```

```html
<!-- Typ 12 – Two-Tone Summary Cards -->
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">Summary</div>
  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(280px, 1fr)); gap:20px;">
    <div style="padding:24px; background:#1e293b; border-radius:10px; border:1px solid #334155; border-left:6px solid #34d399; position:relative; overflow:hidden;">
      <div style="position:absolute; top:0; right:0; width:120px; height:120px; background:radial-gradient(circle at 100% 0%, rgba(52,211,153,0.12), transparent 70%);"></div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Success Rate</div>
      <div style="font-size:36px; font-weight:700; color:#34d399;">99.7%</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">Last 24h</div>
    </div>
    <div style="padding:24px; background:#1e293b; border-radius:10px; border:1px solid #334155; border-left:6px solid #60a5fa; position:relative; overflow:hidden;">
      <div style="position:absolute; top:0; right:0; width:120px; height:120px; background:radial-gradient(circle at 100% 0%, rgba(96,165,250,0.12), transparent 70%);"></div>
      <div style="font-size:14px; color:#94a3b8; margin-bottom:8px;">Avg Response</div>
      <div style="font-size:36px; font-weight:700; color:#60a5fa;">41 ms</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">p95: 58 ms</div>
    </div>
  </div>
</div>
```

```html
<!-- Typ 13 – Simple Footer Info Bar -->
<div style="width:100%; background:#0f172a; border-top:1px solid #334155; padding:20px 28px; font-family:system-ui,sans-serif; color:#94a3b8; font-size:14px; display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; gap:20px; margin:40px 0;">
  <div style="display:flex; flex-direction:column; gap:4px;">
    <div><strong style="color:#cbd5e1;">Node:</strong> node-hannover-03</div>
    <div><strong style="color:#cbd5e1;">Location:</strong> Hannover, DE</div>
  </div>
  <div style="display:flex; flex-direction:column; gap:4px; text-align:right;">
    <div><strong style="color:#cbd5e1;">Uptime:</strong> 19d 9h 12m</div>
    <div><strong style="color:#cbd5e1;">Last reboot:</strong> Feb 13, 2026</div>
  </div>
  <div style="width:100%; text-align:center; margin-top:12px; font-size:13px; color:#64748b;">
    © 2026 Sernik Systems • @Sernik_Js • SuperGrok
  </div>
</div>
```

```html
<!-- Typ 7 (bonus) – Compact Metric Cards z progress ring -->
<div style="width:100%; background:#0f172a; border-radius:12px; border:1px solid #334155; padding:28px; font-family:system-ui,sans-serif; color:#e2e8f0; box-sizing:border-box; margin:32px 0;">
  <div style="font-size:24px; font-weight:700; color:#cbd5e1; margin-bottom:24px;">Core Metrics</div>
  <div style="display:grid; grid-template-columns:repeat(auto-fit, minmax(180px, 1fr)); gap:20px;">
    <div style="text-align:center; padding:20px; background:#1e293b; border-radius:10px; border:1px solid #334155; position:relative;">
      <svg width="80" height="80" viewBox="0 0 80 80" style="margin-bottom:12px;">
        <circle cx="40" cy="40" r="36" fill="none" stroke="#334155" stroke-width="8"/>
        <circle cx="40" cy="40" r="36" fill="none" stroke="#60a5fa" stroke-width="8" stroke-dasharray="226" stroke-dashoffset="180" transform="rotate(-90 40 40)"/>
      </svg>
      <div style="font-size:28px; font-weight:600; color:#60a5fa;">22%</div>
      <div style="font-size:14px; color:#94a3b8; margin-top:4px;">CPU</div>
    </div>
    <!-- kolejne koła analogicznie... -->
  </div>
</div>
```
