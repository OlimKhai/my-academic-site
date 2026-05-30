---
title: "Automating My Website with GitHub Actions"
date: 2024-05-27
summary: "How I set up CI/CD pipelines to automatically deploy my academic site."
tags:
  - CI/CD
  - GitHub Actions
  - DevOps
categories:
  - Technology
authors:
  - me
---

One of the most valuable skills I learned this week was **Continuous Integration and Continuous Deployment (CI/CD)**. Instead of manually uploading files to a server, I configured GitHub Actions to build and deploy my site automatically.

## Ì¥Ñ How It Works
1. I write content locally using Markdown.
2. I push changes to GitHub with `git push`.
3. GitHub Actions triggers a workflow that:
   - Installs Hugo
   - Builds the static site
   - Deploys it to GitHub Pages
4. Within minutes, the changes are live!

## Ìª†Ô∏è Challenges & Solutions
- **Node Options Error**: Fixed by removing conflicting environment variables in the workflow.
- **Hugo Version Mismatch**: Updated `HUGO_VERSION` to `0.161.0` to match the HugoBlox theme requirements.
- **Workflow Conflicts**: Removed duplicate workflow files to prevent race conditions.

## ‚úÖ Result
Now I can focus on **writing content** instead of managing deployments. This is a core DevOps principle: automate the boring stuff!

Next, I'll explore adding more advanced features like custom domains and SEO optimization.
