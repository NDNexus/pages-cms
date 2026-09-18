# Pages CMS Sandbox

A small experimental repository for learning and evaluating [Pages CMS](https://pagescms.org/) as a Git-based content management system.

This repository is intentionally separate from any production project. The goal is to understand Pages CMS properly before deciding where and how it could be useful in real projects.

---

## Why This Exists

I regularly work with Markdown-based content, Git repositories, and static-site build pipelines.

While Git is an excellent source of truth for content, editing Markdown directly in a repository is not always the best experience—especially when content contains structured frontmatter, images, and other metadata.

Pages CMS provides a visual editing interface on top of Git-based content.

This sandbox is an attempt to understand that workflow from both sides:

- As a **content editor**
- As a **developer**

The core question is:

> **Can Pages CMS provide a pleasant editing experience while keeping Markdown files and Git as the source of truth?**

---

## Initial Architecture

The initial experiment is deliberately simple:

```text
                  Pages CMS
                      │
                      ▼
                GitHub Repository
                      │
              ┌───────┴────────┐
              ▼                ▼
          Frontmatter       Markdown
              │                │
              └───────┬────────┘
                      ▼
                Content Files