# CV Data Conventions

This folder is intended to act as a **source-of-truth content repository** for CV generation and profile reuse.

It is not the CV-generation application itself.

## Goals

- Keep reusable career facts in small, maintainable files.
- Separate **public source content** from **private personal details**.
- Make it easy for a downstream app or LLM workflow to:
  - read relevant experience and skills
  - inject private variables locally
  - produce role-specific CVs, cover letters, or profile summaries

## Placeholder Rules

Use placeholders for personal details that should not be hardcoded into reusable public content.

Examples:

- `{{FULL_NAME}}`
- `{{PHONE}}`
- `{{EMAIL}}`
- `{{LOCATION}}`
- `{{LINKEDIN_URL}}`
- `{{GITHUB_URL}}`

These should be merged by a separate local process or application.

## Content Rules

Each file should bias toward **facts, evidence, and outcomes**.

Good content types:

- scope of role
- team size or leadership scope
- systems owned
- technologies used
- measurable outcomes
- regulatory or domain context
- business impact
- examples of architecture, delivery, or recovery work

Avoid mixing in too much polished prose when the same file is meant to support multiple outputs.

## Recommended Tagging Approach

As this evolves, consider tagging experience and skill items with metadata such as:

- `leadership`
- `hands-on`
- `architecture`
- `platform`
- `delivery`
- `cloud`
- `api`
- `security`
- `regulated`
- `ai`
- `llm`
- `fintech`
- `healthcare`

That can be done later as front matter, JSON sidecar files, or a separate index.

## Suggested Future Enhancements

A separate CV-generation app could eventually:

- parse these files into structured models
- rank relevant experience against a job spec
- merge local private variables at runtime
- generate CV variants by target role
- generate a cover letter from the same source pack
- preserve evidence bullets separately from polished narrative bullets

## Practical Advice

For future automation, the most useful pattern is:

1. keep this repo human-readable
2. keep placeholders for anything private
3. store role facts and outcomes in small files
4. let the generator app handle scoring, selection, merging, and formatting
