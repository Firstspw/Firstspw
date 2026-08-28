<svg fill="none" width="100%" max-width="600" height="380" viewBox="0 0 600 380" xmlns="http://www.w3.org/2000/svg">
  <foreignObject width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <style>
        .holo-card {
          width: 550px;
          margin: 10px auto;
          padding: 24px;
          background: rgba(3, 15, 30, 0.85);
          border: 1px solid #00f3ff;
          border-radius: 10px;
          box-shadow: 0 0 15px rgba(0, 243, 255, 0.3), inset 0 0 15px rgba(0, 243, 255, 0.15);
          font-family: 'Segoe UI', Monospace, monospace;
          color: #fff;
          position: relative;
          overflow: hidden;
        }

        .holo-card::before {
          content: '';
          position: absolute;
          top: 0; left: 0; right: 0; bottom: 0;
          background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 243, 255, 0.1) 50%);
          background-size: 100% 4px;
          pointer-events: none;
        }

        .holo-card::after {
          content: '';
          position: absolute;
          top: -100%; left: 0; width: 100%; height: 100%;
          background: linear-gradient(to bottom, transparent, rgba(0, 243, 255, 0.25), transparent);
          animation: scan 4s linear infinite;
          pointer-events: none;
        }

        .header {
          display: flex;
          justify-content: space-between;
          align-items: center;
          border-bottom: 2px dashed #00f3ff;
          padding-bottom: 8px;
          margin-bottom: 16px;
        }

        .title {
          color: #00f3ff;
          font-size: 16px;
          font-weight: bold;
          letter-spacing: 2px;
          text-shadow: 0 0 8px #00f3ff;
        }

        .grid {
          display: grid;
          grid-template-columns: 1fr 1fr;
          gap: 12px;
        }

        .item {
          background: rgba(0, 243, 255, 0.05);
          border-left: 3px solid #00f3ff;
          padding: 8px 12px;
          opacity: 0;
          transform: translateY(10px);
          animation: fadeIn 0.5s forwards ease-out;
        }

        .item:nth-child(1) { animation-delay: 0.2s; }
        .item:nth-child(2) { animation-delay: 0.5s; }
        .item:nth-child(3) { animation-delay: 0.8s; }
        .item:nth-child(4) { animation-delay: 1.1s; }
        .item:nth-child(5) { animation-delay: 1.4s; }
        .item:nth-child(6) { animation-delay: 1.7s; }

        .label {
          font-size: 10px;
          color: #8ab4f8;
          text-transform: uppercase;
          letter-spacing: 1px;
        }

        .val {
          font-size: 13px;
          color: #e0f7fa;
          font-weight: bold;
          text-shadow: 0 0 5px #00f3ff;
          margin-top: 2px;
        }

        .skills {
          margin-top: 14px;
          border-top: 1px solid rgba(0,243,255,0.2);
          padding-top: 10px;
          opacity: 0;
          animation: fadeIn 0.5s forwards ease-out 2.0s;
        }

        .badge {
          display: inline-block;
          background: rgba(0, 243, 255, 0.15);
          color: #00f3ff;
          border: 1px solid #00f3ff;
          font-size: 10px;
          padding: 2px 8px;
          margin: 2px;
          border-radius: 3px;
          box-shadow: 0 0 5px rgba(0,243,255,0.3);
        }

        @keyframes scan {
          0% { top: -100%; }
          100% { top: 200%; }
        }

        @keyframes fadeIn {
          to { opacity: 1; transform: translateY(0); }
        }
      </style>

      <div class="holo-card">
        <div class="header">
          <span class="title">⚡ HOLOGRAM USER PROFILE</span>
          <span style="color: #00f3ff; font-size: 11px;">[ ONLINE ]</span>
        </div>

        <div class="grid">
          <div class="item">
            <div class="label">IDENTITY / NAME</div>
            <div class="val">Firstspw</div>
          </div>
          <div class="item">
            <div class="label">PRIMARY ROLE</div>
            <div class="val">Developer &amp; UI/UX Creator</div>
          </div>
          <div class="item">
            <div class="label">TECH STACK</div>
            <div class="val">Web, IoT &amp; Microservices</div>
          </div>
          <div class="item">
            <div class="label">STATUS</div>
            <div class="val">Building Cyber-Interfaces</div>
          </div>
          <div class="item">
            <div class="label">SYSTEM SECURITY</div>
            <div class="val">ENCRYPTED // ACTIVE</div>
          </div>
          <div class="item">
            <div class="label">LOCATION</div>
            <div class="val">Thailand 🇹🇭</div>
          </div>
        </div>

        <div class="skills">
          <div class="label" style="margin-bottom: 6px;">TECH MODULES DETECTED:</div>
          <span class="badge">HTML5/CSS3</span>
          <span class="badge">JavaScript</span>
          <span class="badge">Angular</span>
          <span class="badge">NestJS</span>
          <span class="badge">Socket.IO</span>
          <span class="badge">ESP32 / IoT</span>
        </div>
      </div>
    </div>
  </foreignObject>
</svg>

---

## 🛸 CYBERNETIC STATS OVERVIEW

<div align="center">

![Firstspw's GitHub stats](https://github-readme-stats.vercel.app/api?username=Firstspw&show_icons=true&theme=cyan&bg_color=030f1e&title_color=00f3ff&text_color=8ab4f8&icon_color=00f3ff&border_color=00f3ff&hide_border=false&count_private=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Firstspw&layout=compact&theme=cyan&bg_color=030f1e&title_color=00f3ff&text_color=8ab4f8&border_color=00f3ff&hide_border=false)

</div>

---

## ⚙️ TECH ARSENAL

<div align="center">

**FRONTEND** | **BACKEND** | **IoT & EMBEDDED** | **TOOLS**
---|---|---|---
🎨 HTML5/CSS3 | 🔧 NestJS | 🤖 ESP32 | 🐙 Git
⚛️ JavaScript | 🔌 Node.js | 📡 Socket.IO | 💻 VS Code
🅰️ Angular | 💾 MongoDB | 🔋 Microservices | 📦 Docker

</div>

---

## 🚀 FEATURED PROJECTS

<table>
  <tr>
    <td width="50%">
      <h3>🎯 Project Alpha</h3>
      <p>อลังการ Web Application ที่ใช้ Angular + NestJS</p>
      <a href="#">View Repository →</a>
    </td>
    <td width="50%">
      <h3>📡 IoT Dashboard</h3>
      <p>Real-time monitoring system สำหรับ ESP32 devices</p>
      <a href="#">View Repository →</a>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>💻 UI Components</h3>
      <p>Beautiful reusable component library</p>
      <a href="#">View Repository →</a>
    </td>
    <td width="50%">
      <h3>🔐 Cyber Security Tools</h3>
      <p>Advanced security solutions & encryption</p>
      <a href="#">View Repository →</a>
    </td>
  </tr>
</table>

---

## 📊 ACTIVITY STREAK

<div align="center">

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=Firstspw&theme=dark&background=030f1e&stroke=00f3ff&ring=00f3ff&fire=00f3ff&currStreakNum=8ab4f8&sideNums=8ab4f8&currStreakLabel=00f3ff&sideLabelsColor=00f3ff&dates=8ab4f8&hide_border=true)](https://git.io/streak-stats)

</div>

---

## 💼 EXPERIENCE HIGHLIGHTS

- 🎯 **Full-Stack Development** - Web & IoT Integration
- 🔧 **Microservices Architecture** - Scalable Backend Systems
- 🤖 **IoT Solutions** - ESP32 & Embedded Systems
- 🎨 **UI/UX Design** - Modern & Responsive Interfaces
- 💡 **Innovation Driven** - Always exploring new technologies

---

## 🌐 CONNECT WITH ME

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Firstspw)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your@email.com)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com)

</div>

---

<div align="center">

### ⭐ If you find my projects helpful, please give them a star! ⭐

![Profile Views](https://komarev.com/ghpvc/?username=Firstspw&color=00f3ff&style=flat-square)

</div>

---

<div align="center">
  
**Made with 💙 by Firstspw | Building the Future, One Line at a Time**

</div>
