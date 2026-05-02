# GitHub Profile README — Full Visual Overhaul

**Date:** 2026-05-02
**Target file:** `README.md` (apple037 GitHub profile repo)
**Style:** Developer-styled — badges, shields, stat cards, animated header
**Language:** English only

---

## Goal

Replace the current sparse GitHub profile README with a polished, visually rich developer portfolio page. Content is sourced from `Wen-Li_Fan_Resume_Taiwan.docx`.

---

## Sections

### 1. Header
- Centered `<h1>` with name: "Hi, I'm Jasper 👋"
- Animated typing SVG via `readme-typing-svg.demolab.com` cycling through: `Backend Engineer`, `AI Engineer`, `Blockchain Developer`
- Visitor counter badge via `komarev.com/ghpvc/?username=apple037` centered below the title

### 2. About Me
Short paragraph from the resume's Professional Summary:
> "Backend and AI engineer with ~5 years of experience delivering backend systems, AI integration, and blockchain-related services. Strong hands-on execution in production environments with a practical, team-oriented approach."

### 3. GitHub Stats Row
Three cards in a centered HTML `<table>` with no borders:
- **GitHub Stats card** — `github-readme-stats.vercel.app/api?username=apple037` (show stars, commits, PRs, issues; theme: `tokyonight`)
- **GitHub Streak card** — `streak-stats.demolab.com?user=apple037` (theme: `tokyonight`)
- **Top Languages card** — `github-readme-stats.vercel.app/api/top-langs/?username=apple037&layout=compact` (theme: `tokyonight`)

### 4. Tech Stack
Shields.io badges (`style=for-the-badge`) grouped into labeled rows:

| Group | Badges |
|---|---|
| Languages | Java, Python, Node.js |
| Backend | Spring Boot, RESTful API, Microservices |
| DB / Cache / Messaging | PostgreSQL, MongoDB, Redis, Kafka, RabbitMQ, Firebase |
| AI/ML | PyTorch, Diffusion Models, GANs |
| Blockchain | Solidity, Hardhat, Web3j |
| DevOps & Tools | Docker, GCP, Git, Linux, Jenkins |

### 5. Work Experience
Compact list format: `**Role** @ Company (dates)` followed by 2–3 bullet highlights per role, sourced directly from resume.

1. **Backend & AI Engineer** @ Mygram AI Technology Co., Ltd. (Jul 2024 – Present)
2. **Senior Software & Blockchain Engineer** @ GASH POINT Co., Ltd. (Oct 2023 – Jun 2024)
3. **Java Backend & Blockchain Engineer** @ Wandatech Co., Ltd. (Jul 2021 – Oct 2023)
4. **MIS Engineer** @ Vanguard International Semiconductor Corp. (Oct 2019 – Apr 2021)

### 6. Projects
Three GitHub repo cards using `github-readme-stats` repo-card widget:
- `apple037/chatter-app` — Blockchain chatroom
- `apple037/notify-schedule` — Price notify bot
- `apple037/stanley` — Discord chatbot app

### 7. WakaTime Metrics
Keep existing `<!--START_SECTION:waka-->` / `<!--END_SECTION:waka-->` block unchanged. This section is auto-updated by the waka-readme GitHub Action.

### 8. Connect
Two shields.io link badges:
- Email: `apple037037@gmail.com`
- GitHub: `github.com/apple037`

---

## Implementation Notes

- All stat cards use `theme=tokyonight` for visual consistency
- Cards in the stats row are wrapped in `<td>` tags with `align="center"` for proper centering in GitHub Markdown
- Shields.io badge colors: use `logo=` parameters with official brand colors where available
- Remove the existing `[![Jasper's GitHub stats]...]` badge and replace with the new stats row
- Remove the existing contact table and replace with the new Connect section
- The `<!--START_SECTION:waka-->` markers must be preserved exactly for the GitHub Action to continue working

---

## Success Criteria

- README renders correctly on github.com/apple037 (no broken images)
- All 8 sections present and populated with real resume data
- WakaTime section still auto-updates after the change
- Stat cards, streak, and top-languages cards all load
- Tech badges display with correct logos and colors
