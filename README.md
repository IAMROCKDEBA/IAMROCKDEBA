# Namaste! I'm Deba (IAMROCKDEBA) — Ganapatha 🕉️

Welcome to my Ganapatha — the developer path I walk every day: learning, building, and sharing. This README is a living document that showcases who I am, what I build, and how to connect with me.

---

## About Ganapatha
"Ganapatha" is my personal theme: a blend of growth, gratitude, and the path of continuous creation. Here I document experiments, production projects, and lessons learned. Expect practical code, clean documentation, and a focus on delivering value.

## Quick Bio
- 🔭 I’m currently working on: shipping reliable, well-tested software and exploring full-stack automation.
- 🌱 I’m learning: advanced system design, infra as code, and optimizing developer workflows.
- 👯 I’m open to collaborating on: tooling, open-source infra, and data-driven frontend experiences.
- 💬 Ask me about: Node.js, TypeScript, Python, CI/CD, and developer productivity.
- ⚡ Fun fact: I love turning complex problems into simple, reliable solutions.

---

## GitHub Stats & Activity

- GitHub Readme Cards (auto-updating)

[![IAMROCKDEBA's GitHub stats](https://github-readme-stats.vercel.app/api?username=IAMROCKDEBA&show_icons=true&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=IAMROCKDEBA&layout=compact&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA)

- Contribution Streak

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=IAMROCKDEBA&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA)

Notes:
- These cards are powered by third-party services (github-readme-stats, streak-stats). They update automatically when your public contributions/updateable metrics change.
- If any card fails to render, check the service status or consider self-hosting equivalent endpoints.

---

## Tech & Tools
Here are the technologies I use most often. Replace or reorder to match your current stack.

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

---

## Featured Projects
Click the cards to view repositories. Replace repo names with your actual repos.

[![Pin to repo](https://github-readme-stats.vercel.app/api/pin/?username=IAMROCKDEBA&repo=awesome-repo&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA/awesome-repo)
[![Pin to repo](https://github-readme-stats.vercel.app/api/pin/?username=IAMROCKDEBA&repo=infra-templates&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA/infra-templates)
[![Pin to repo](https://github-readme-stats.vercel.app/api/pin/?username=IAMROCKDEBA&repo=web-app-starter&theme=tokyonight&hide_border=true)](https://github.com/IAMROCKDEBA/web-app-starter)

How to pin your own repos:
1. Go to your profile: Repository settings -> Pin repository
2. Or rename the repo slugs above to the repos you want to highlight.

---

## How I Work
- I prefer small, incremental PRs with clear descriptions and tests.
- I value automated CI, linting, and type checks before review.
- I write docs as code: README.md for usage, docs/ for long-form guides, and examples/ to onboard contributors.

---

## Open Source & Contributions
Interested in contributing? Great!
- Check the repository's CONTRIBUTING.md, run tests locally, and create a small PR.
- Label ideas: good-first-issue, help-wanted.
- I try to review and respond within a week for active PRs.

---

## Articles & Talks
- Blog: https://your-blog.example.com (replace with your blog)
- Talks: add links to slides or recordings here.

---

## Contact & Socials
- Email: your-email@example.com
- LinkedIn: https://www.linkedin.com/in/your-profile
- Twitter/X: https://twitter.com/your-handle
- Mastodon: @yourhandle@instance.social

Replace the placeholders with your real links.

---

## README Automation (optional)
To keep parts of this README fresh (e.g., "Last updated" timestamp or regenerate cards), add this GitHub Actions workflow to your profile repo: create .github/workflows/update-readme.yml

```yaml
name: Refresh README
on:
  schedule:
    - cron: '0 0 * * *' # every day at 00:00 UTC
  workflow_dispatch:

jobs:
  refresh:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - name: Update timestamp in README
        run: |
          NOW=$(date -u +"%Y-%m-%d %H:%M UTC")
          echo "Last updated: $NOW" > last-updated.txt
          # This will update a placeholder line in README.md if present:
          python - <<'PY'
import re,sys
with open("README.md","r",encoding="utf8") as f:
    s=f.read()
ns="Last updated: "
s=re.sub(r"Last updated: .*", ns+open("last-updated.txt").read().strip(), s)
with open("README.md","w",encoding="utf8") as f:
    f.write(s)
PY
      - name: Commit & push
        run: |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add README.md
          git commit -m "chore: refresh README timestamp [skip ci]" || echo "no changes to commit"
          git push
```

Notes:
- This workflow replaces any line in README.md that starts with "Last updated:" with the current UTC timestamp. Add a line "Last updated: ..." somewhere in your README to use it.
- You can extend the workflow to regenerate markdown fragments, fetch blog posts, or rebuild showcases.

---

## Personalize This README
- Replace placeholders (email, social links, repo names).
- Update the theme parameter in the stats cards (e.g., &theme=radical or &theme=gruvbox) to match your style.
- Add or remove badges to reflect the tools you use.
- Pin the repos you want to highlight on your profile page.

---

Last updated: PLACEHOLDER_DATE

If you'd like, I can:
- Replace placeholders with your real links and repos now,
- Generate a custom banner image or emoji set for the Ganapatha theme,
- Provide a ready-to-add Actions file pre-filled with your repo names and preferences.

Just tell me which repos and which socials to include and I’ll update the README for you.
