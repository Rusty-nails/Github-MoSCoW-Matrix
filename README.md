# GitHub Feature Prioritization Using the MoSCoW Framework

**Author:** CSP Student M252
**CST 640: Platform and Product Development — Week 7 Assignment**
**Date:** 5/3/2026

## Project Overview

This project analyzes customer feedback for GitHub and applies the MoSCoW prioritization framework to categorize key features for a future release cycle. Acting as a product manager at CodeCrafters Inc., the goal is to show how realistic user feedback can be turned into a clear, defensible product roadmap. The five feedback questions used here come from the virtual lab activity in Module 6, applied to GitHub as the chosen developer tool.

## Selected Tool: GitHub

GitHub is a Git-based code hosting and collaboration platform used by developers and teams to manage source code, review changes, and ship software. Its feature set covers the full development lifecycle, including repositories, pull requests, automated builds, issue tracking, and project management. With millions of daily users and a wide feature surface, GitHub generates the kind of continuous feedback stream that prioritization frameworks are built to handle.

## Prioritization Framework: MoSCoW

The MoSCoW framework was developed by Dai Clegg at Oracle to help teams prioritize during time-boxed releases. It groups features into four categories:

- **Must-Have**: Non-negotiable features the product cannot ship without
- **Should-Have**: Important features that add real value but can wait if needed
- **Could-Have**: Nice-to-have improvements with smaller impact if left out
- **Won't-Have**: Features intentionally excluded from this release cycle

MoSCoW was chosen over alternatives like KANO because it pairs well with feedback-driven prioritization and gives a clear visual story for stakeholder communication.

## Customer Feedback Summary

Five feedback questions from Module 6's virtual lab activity were applied to GitHub. Realistic responses were drawn from common community themes:

1. **Most valuable features**: Pull requests, code review, version control, and issue tracking
2. **Missing or improvable**: Cross-repo search, beginner onboarding, and the Actions setup experience
3. **UI/UX feedback**: Generally clean for experienced users but dense for newcomers, with notification settings drawing frequent complaints
4. **Recurring issues**: Slow loading on large diffs, Actions runner queue delays during peak hours, and notification reliability issues
5. **New feature suggestions**: Interactive tutorials, simplified Actions setup, better search filters, and improved project board templates

Full feedback responses are available in [`customer-feedback.md`](customer-feedback.md).

## MoSCoW Matrix

Eight GitHub features were categorized based on the feedback patterns above. Summary view:

| Priority | Feature | Justification |
|---|---|---|
| **Must-Have** | Version Control with Git Repositories | Core to GitHub's identity and the foundation of the entire platform |
| **Must-Have** | Pull Requests & Code Review | Backbone of team collaboration and code quality |
| **Must-Have** | Issue Tracking & Bug Reporting | Centralized visibility into bugs, tasks, and enhancements |
| **Should-Have** | GitHub Actions (CI/CD) | Strong productivity boost, but the product still functions without it |
| **Should-Have** | Project Boards | Useful for planning at scale and optional for smaller teams |
| **Could-Have** | Advanced Search & Filtering | Improves discoverability across repos and issues |
| **Could-Have** | Enhanced Onboarding & Tutorials | Lowers the learning curve for new users |
| **Won't-Have** | Built-in Real-Time Code Editor (Full IDE) | Out of scope, since external IDEs already serve this need |

The full matrix with extended reasoning is available in [`moscow-matrix.md`](moscow-matrix.md).

## Repository Contents

- `README.md` — This file
- `CST-640-Week7.pptx` — Presentation deck with detailed speaker notes
- `moscow-matrix.md` — Full MoSCoW matrix in markdown format
- `customer-feedback.md` — Detailed feedback responses for each of the five question

## Key Insights

- Customer feedback turns feature prioritization from guesswork into evidence-based decisions
- The Won't-Have category is one of MoSCoW's strongest tools for managing scope creep and stakeholder expectations
- The framework is fast to apply but lacks an objective scoring method, so pairing it with weighted scoring or KANO can give a fuller picture
- Feature categories drift over time as user expectations shift, which is why quarterly re-runs help keep the matrix current
- The matrix doubles as a communication artifact, useful for explaining roadmap decisions to engineering, design, and leadership

## References

DigitalOcean. (2023). How to prioritize your product roadmap. https://www.digitalocean.com/resources/articles/product-roadmap-prioritization

Dziuba, L. (2025). 9 prioritization frameworks & which to use in 2025. Product School. https://productschool.com/blog/product-fundamentals/ultimate-guide-product-prioritization

Lucas_DevSamurai. (2023). Understanding the MoSCoW prioritization: How to implement it into your project. Atlassian Community. https://community.atlassian.com/forums/App-Central-articles/Understanding-the-MoSCoW-prioritization-How-to-implement-it-into/ba-p/2463999

Productboard. (n.d.). Product prioritization frameworks: What is prioritization in product management? https://www.productboard.com/glossary/product-prioritization-frameworks/

ProductPlan. (n.d.). MoSCoW prioritization. https://www.productplan.com/glossary/moscow-prioritization

WiMi Teamwork. (2026). MoSCoW method: Simple prioritization matrix for project tasks. https://www.wimi-teamwork.com/en/blog/project-management/moscow-method

