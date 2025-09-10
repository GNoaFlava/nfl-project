# 🏈 NFL Project Sync Bot

![Sync Workflow](https://github.com/your-org-or-username/your-repo/actions/workflows/project-sync.yml/badge.svg)

This repo syncs **GitHub Issues ↔ GitHub Projects (v2)** automatically:

- **Issues → Project**
  - Adds issues to project
  - Ensures milestones exist + assigns
  - Applies milestone-based labels

- **Project → Issues**
  - Syncs Priority → labels
  - Syncs Target Date → due date
  - Closes issues when moved to **Done**

## 🚀 Setup

1. Create a **GitHub Project (v2)** inside your org or user.
2. Replace these in `.github/workflows/project-sync.yml`:
   - `ORG: "your-org-or-username"`
   - `PROJECT_NUMBER: 1`
3. Push changes — on the first run, it will generate `.github/config/project_config.json`.
4. Config auto-commits itself. IDs are masked in logs for safety.

## 🔄 Usage

- Add/edit issues → they appear in the Project with proper labels + milestones.
- Update Project fields → they sync back into Issues.
- Move Issue to **Done** in Project → GitHub Issue closes.

Enjoy the automation 🎉

