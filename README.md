<div align="center">
  <a href="https://leantime.io">
    <img src="https://leantime.io/wp-content/uploads/2023/03/leantime_logo.png" alt="Leantime Logo" width="280"/>
  </a>

  # Leantime®

  ⭐ **If you find Leantime useful, please star us on GitHub!** ⭐

  **Leantime** is an open-source project management system built for non-project managers.<br>
  We combine strategy, planning, and execution while making it easy for everyone on the team to use.<br>
  Built with **ADHD, dyslexia, and autism in mind.** 🧠

  💪 As simple as Trello but as feature-rich as Jira &nbsp;|&nbsp; 🔄 A perfect alternative to ClickUp, Monday, or Asana

  [Website](https://leantime.io) • [Documentation](https://docs.leantime.io) • [Community Discord](https://discord.gg/4zMzJtAq9z)

  <br>

  <a href="https://trendshift.io/repositories/2264" target="_blank">
    <img src="https://trendshift.io/api/badge/repositories/2264" alt="Trendshift Badge" width="250" height="55"/>
  </a>

  <br><br>

  [![License Badge](https://img.shields.io/github/license/leantime/leantime?style=flat-square)](https://www.gnu.org/licenses/agpl-3.0.en.html)
  [![Docker Hub Badge](https://img.shields.io/docker/pulls/leantime/leantime?style=flat-square)](https://hub.docker.com/r/leantime/leantime)
  ![Github Downloads](https://img.shields.io/github/downloads/leantime/leantime/total?style=flat-square)
  [![Discord Badge](https://img.shields.io/discord/990001288026677318?label=Discord&style=flat-square)](https://discord.gg/4zMzJtAq9z)
  [![Crowdin](https://badges.crowdin.net/leantime/localized.svg?style=flat-square)](https://crowdin.com/project/leantime)
  ![GitHub Sponsors](https://img.shields.io/github/sponsors/leantime?style=flat-square)

  <br>

  <img src="public/assets/images/Screenshots/mywork-v3.5.png" alt="Leantime Dashboard" width="100%" style="border-radius: 8px; border: 1px solid #333;" />
</div>

---

## 🚀 Features

*Yes, all of these features are included in the open-source (OSS) version!*

| Task Management | Project Planning | Information & Knowledge | Administration |
| :--- | :--- | :--- | :--- |
| • Kanban boards, Gantt, table, list & calendar views<br>• Unlimited subtasks & dependencies<br>• Milestone management<br>• Sprint management<br>• Time tracking & timesheets | • Project dashboards & status reports<br>• Goal & metrics tracking<br>• Lean & Business Model Canvas<br>• SWOT analysis canvas<br>• Risk analysis | • Wikis / Documentation<br>• Idea boards<br>• Retrospectives<br>• S3 or local file storage<br>• Comments & discussions on everything | • Easy installation<br>• Multi-role & project permissions<br>• 2FA, LDAP, & OIDC integration<br>• REST & JSON-RPC API & plugins<br>• Slack, Mattermost, & Discord sync<br>• Available in 20+ languages |

---

## 📸 Screenshots

<table width="100%">
    <tr>
        <td width="33%"><img src="public/assets/images/Screenshots/dark.png" alt="Dark Mode" width="100%"/><br><em>Dark Mode</em></td>
        <td width="33%"><img src="public/assets/images/Screenshots/projectDashboard.png" alt="Project Dashboard" width="100%"/><br><em>Project Dashboard</em></td>
        <td width="33%"><img src="public/assets/images/Screenshots/table.png" alt="Table View" width="100%"/><br><em>Grouped To-Dos</em></td>
    </tr>
    <tr>
        <td><img src="public/assets/images/Screenshots/kanban.png" alt="Kanban" width="100%"/><br><em>Kanban Board</em></td>
        <td><img src="public/assets/images/Screenshots/timeline.png" alt="Timeline" width="100%"/><br><em>Gantt Timeline</em></td>
        <td><img src="public/assets/images/Screenshots/calendar.png" alt="Calendar" width="100%"/><br><em>Project Calendar</em></td>
    </tr>
    <tr>
        <td><img src="public/assets/images/Screenshots/goals.png" alt="Goals" width="100%"/><br><em>Goals</em></td>
        <td><img src="public/assets/images/Screenshots/docs.png" alt="Docs" width="100%"/><br><em>Wikis & Documents</em></td>
        <td><img src="public/assets/images/Screenshots/timesheet.png" alt="Timesheets" width="100%"/><br><em>Timesheets</em></td>
    </tr>
</table>

---

## ❗ System Requirements

* **PHP:** 8.2+
* **Database:** MySQL 8.0+ or MariaDB 10.6+
* **Web Server:** Apache or Nginx (IIS is supported with minor adjustments)
* **Required PHP Extensions:** 
  `bcmath`, `ctype`, `curl`, `dom`, `exif`, `fileinfo`, `filter`, `gd`, `hash`, `ldap`, `mbstring`, `mysql`, `opcache`, `openssl`, `pcntl`, `pcre`, `pdo`, `phar`, `session`, `tokenizer`, `zip`, `simplexml`

---

## ⚡ Installation & Deployment

### 🐳 Production via Docker (Recommended)
We maintain an official [Docker image on DockerHub](https://hub.docker.com/r/leantime/leantime). 

```bash
docker run -d --restart unless-stopped -p 8080:8080 --network leantime-net \
-e LEAN_DB_HOST=mysql_leantime \
-e LEAN_DB_USER=admin \
-e LEAN_DB_PASSWORD=321.qwerty \
-e LEAN_DB_DATABASE=leantime \
-e LEAN_EMAIL_RETURN=changeme@local.local \
--name leantime leantime/leantime:latest
