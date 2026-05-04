# GitHub Feature Prioritization: MoSCoW Matrix

## Overview

This document presents the full MoSCoW prioritization of eight GitHub features based on customer feedback themes. Each feature is categorized using the test question MoSCoW poses: "What happens if this is not delivered?" Features that would cause the platform to fail without them land in Must-Have. Features the product can survive without sit in Should-Have, Could-Have, or Won't-Have based on their impact and timing.

For the underlying feedback responses, see [`customer-feedback.md`](customer-feedback.md).

---

## Must-Have: Non-negotiable features
*Without these, GitHub fails its purpose.*

### 1. Version Control with Git Repositories

**Justification:** Core to GitHub's identity and the foundation of the entire platform. Repositories are how source code lives on the system, and branching, merging, and history tracking are the daily mechanics every other feature builds on.

**Feedback connection:** Users consistently cite version control as the most valuable feature on the platform and as the reason they chose GitHub in the first place.

**MoSCoW test:** If repositories were not delivered, GitHub would not exist as a product. Clear Must-Have.

### 2. Pull Requests & Code Review

**Justification:** The backbone of team collaboration on the platform. Inline comments, approval workflows, and change tracking turn pull requests into the place where most actual collaborative decisions happen.

**Feedback connection:** Pull requests and code review come up first in feedback about most-valuable features. Teams describe the workflow as the difference between solo development and effective team development.

**MoSCoW test:** Without pull requests, the platform reverts to a Git host without collaboration tooling. Many enterprise customers would leave.

### 3. Issue Tracking & Bug Reporting

**Justification:** Provides centralized visibility into bugs, tasks, and enhancements tied directly to the codebase. Linking issues to pull requests improves transparency and accountability across teams.

**Feedback connection:** Issue tracking is consistently in the top three most-valued features. Teams describe the codebase-adjacent tracking as the reason they do not need a separate bug database.

**MoSCoW test:** Without issue tracking, teams would adopt external tools like Jira and reduce their dependence on GitHub. Significant strategic loss.

---

## Should-Have: Important but not vital
*The platform still functions without these in the short term.*

### 4. GitHub Actions (CI/CD)

**Justification:** A strong productivity boost that automates testing and deployment, but the platform still functions for users who use external CI tools or skip automation entirely. Solo developers and small projects can ship without it.

**Feedback connection:** Power users describe Actions as transformative for their workflows. Newer users describe initial setup as confusing, which keeps it out of Must-Have for now.

**MoSCoW test:** If Actions were not delivered, users would adopt Jenkins, CircleCI, or similar tools. Productivity loss but no platform failure.

### 5. Project Boards

**Justification:** Useful for planning and visualizing work at scale, but optional for smaller teams and solo developers who manage tasks through issues alone.

**Feedback connection:** Larger organizations and open-source projects describe Project Boards as helpful for coordinating contributors. Smaller teams often skip the feature entirely.

**MoSCoW test:** Without Project Boards, teams would use Trello, Linear, or external project management tools. Friction but not failure.

---

## Could-Have: Quality-of-life improvements
*Nice-to-have features that improve user experience.*

### 6. Advanced Search & Filtering

**Justification:** Improves discoverability across repos and issues, especially for large organizations and open-source maintainers managing many repositories at once. Reduces time spent hunting for old pull requests, code snippets, or related issues.

**Feedback connection:** Cross-repository search is one of the most-cited improvement areas in feedback. Users describe the current search as functional but limited at scale.

**MoSCoW test:** Without improved search, users keep using the existing search and external tools. Productivity friction but no functional gap.

### 7. Enhanced Onboarding & Tutorials

**Justification:** Lowers the learning curve for new users by walking them through common workflows like opening a pull request, configuring branch protection, or setting up Actions.

**Feedback connection:** Onboarding is consistently flagged as a weakness for new users, and interactive tutorials are one of the most-requested new features. Power users do not need this, which keeps it out of Must-Have.

**MoSCoW test:** Without enhanced onboarding, new users continue to learn from external tutorials and trial and error. Slower adoption but no functional gap.

---

## Won't-Have: Out of scope for this release
*Intentionally deferred or excluded.*

### 8. Built-in Real-Time Code Editor (Full IDE)

**Justification:** Out of scope for this release because most developers already rely on external IDEs like VS Code, IntelliJ, or Vim. Building a full IDE inside GitHub would require significant engineering investment with limited additional value, and it conflicts with GitHub's strategic position as a collaboration platform rather than a development environment.

**Feedback connection:** Users do not request a full IDE inside GitHub. Existing lightweight editors and Codespaces already cover the in-browser editing use cases users actually have.

**MoSCoW test:** Building a full IDE has high cost and low marginal value. Naming this in the Won't-Have category prevents the same feature request from coming up in every planning cycle.

---

## Summary Table

| # | Feature | Category | Core Reason |
|---|---|---|---|
| 1 | Version Control with Git Repositories | Must-Have | Foundation of the platform |
| 2 | Pull Requests & Code Review | Must-Have | Core collaboration workflow |
| 3 | Issue Tracking & Bug Reporting | Must-Have | Codebase-adjacent task tracking |
| 4 | GitHub Actions (CI/CD) | Should-Have | Productivity boost, not required |
| 5 | Project Boards | Should-Have | Planning at scale, optional |
| 6 | Advanced Search & Filtering | Could-Have | Discoverability improvement |
| 7 | Enhanced Onboarding & Tutorials | Could-Have | Lower learning curve |
| 8 | Built-in Real-Time Code Editor | Won't-Have | Out of scope, IDEs cover this |

---

## Notes on Application

The eight features above were selected to balance core functionality, workflow improvements, and intentional exclusions. The matrix is a starting point rather than a final answer. Feature categories drift over time as user expectations shift, and features in one category today may move into another after a few release cycles. Re-running the matrix quarterly keeps it current and catches shifts before they become roadmap problems.
