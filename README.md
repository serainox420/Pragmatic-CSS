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
