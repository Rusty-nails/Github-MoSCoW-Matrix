# GitHub Customer Feedback Analysis

## Overview

This document presents the detailed customer feedback responses used to inform the MoSCoW prioritization for GitHub. The five questions come from Module 6's virtual lab activity. Responses reflect realistic feedback themes commonly seen in developer surveys, GitHub community discussions, product reviews, and support channels.

---

## Q1: What features do users find most valuable?

Pull requests and the surrounding code review tools come up first in nearly every developer survey of GitHub users. Teams describe the inline comment threads, approval gates, and review request flows as the workflow that makes collaborative development possible at scale.

Version control through Git repositories is the second most-cited feature. Users frame this as the foundation everything else builds on, with branching and merging called out as daily essentials.

Issue tracking rounds out the top three. Developers value the ability to log bugs and feature requests directly alongside the code they relate to, and linking between issues and pull requests improves accountability.

**Common feedback themes:**
- "Pull requests are how our team actually communicates about code"
- "We could not run our development workflow without branches and merges"
- "Linking issues to pull requests keeps everyone on the same page"

---

## Q2: What features are missing or could be improved?

Cross-repository search comes up repeatedly as a pain point, especially for users in large organizations and open-source maintainers managing dozens of repos. Users describe spending too much time hunting for relevant code, issues, or pull requests across their work.

Onboarding for new users is the second major gap. Power users love the depth of the platform, but newcomers describe the learning curve as steep, with terminology and workflow conventions assumed rather than explained.

The setup experience for GitHub Actions is the third common improvement request. Users describe initial configuration as confusing, with YAML errors and unclear documentation cited as common blockers.

**Common feedback themes:**
- "Searching across repos is harder than it should be"
- "GitHub is powerful but the onboarding could be more beginner-friendly"
- "Actions setup gets complicated quickly for first-time users"

---

## Q3: How do users feel about the user interface and user experience?

Reactions are mixed and tend to split along experience lines. Users who have spent significant time on the platform describe the UI as clean, functional, and information-dense in a productive way. Newer users more often describe it as overwhelming, with cluttered navigation and too many options surfaced at once.

Notification settings draw consistent complaints across both groups. Users report that even with custom notification rules, the volume of emails and in-app alerts can become unmanageable on active repositories.

Recent navigation redesigns have been divisive in community discussions, with some users appreciating the cleaner layout and others reporting that familiar tools became harder to find.

**Common feedback themes:**
- "The interface is solid once you know your way around"
- "Notification settings feel like they were designed for a different era"
- "The new navigation took some getting used to"

---

## Q4: Are there any recurring issues or bugs reported by users?

Performance on large pull requests is the most-cited recurring issue. Users working on major refactors or bulk changes report slow loading times for diffs over a few thousand lines, and the inline comment system can lag during heavy review activity.

GitHub Actions runner queue delays during peak hours are the second common complaint. Teams report builds sitting in queue for noticeable stretches when overall platform load is high, which slows feedback cycles for tight iteration loops.

Notification reliability rounds out the top three. Users describe occasional missed alerts for review requests and mentions, which can result in pull requests sitting longer than expected before getting reviewed.

**Common feedback themes:**
- "Large diffs take forever to load and review"
- "Actions queues can stall when traffic is heavy"
- "I have missed review requests because notifications did not fire"

---

## Q5: What suggestions do users have for new features or improvements?

Interactive onboarding tutorials top the suggestion list. Users want guided walkthroughs of common workflows like opening a pull request, configuring branch protection, or setting up Actions, ideally embedded directly in the platform.

Simplified Actions setup is the second most-common request. Users suggest pre-built templates for common stacks, smarter error messages, and a visual workflow editor as ways to lower the configuration barrier.

Better cross-repository search filters are the third recurring suggestion. Users want the ability to narrow searches by date range, author, status, and other metadata more easily than the current filter syntax allows.

Improved project board templates round out the top suggestions. Users describe the existing templates as basic and request more options for engineering, design, and product workflows.

**Common feedback themes:**
- "Interactive tutorials would help new developers get productive faster"
- "Pre-built Actions templates for common stacks would save hours"
- "Better search filters would help me find old pull requests faster"

---

## Themes That Emerged Across the Feedback

Three patterns showed up across multiple questions:

- **Power and learning curve are connected.** The same depth that makes GitHub valuable to experienced users creates friction for new ones. Several Could-Have features address this gap directly.
- **Performance issues affect trust.** Users tolerate occasional slowness, but recurring performance problems on core workflows like large diff review reduce confidence in the platform overall.
- **Tooling depth is uneven.** Search, notifications, and project planning lag behind the maturity of the version control and code review experience, which is where most improvement requests cluster.

These patterns shaped which features earned Must-Have versus Should-Have versus Could-Have categorization in the MoSCoW matrix. See [`moscow-matrix.md`](moscow-matrix.md) for the full categorization.
