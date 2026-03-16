# Use Markdown Architectural Decision Records (MADRs) for documenting decisions.

## Context and Problem Statement

I want to document all the decisions I make while developing nagi.

## Considered Options

* Use one of the templates in https://github.com/joelparkerhenderson/architecture-decision-record
* Use one of the templates in https://adr.github.io/adr-templates/

## Decision Outcome

Chosen option: https://github.com/adr/madr because the template it used looked familiar enough to me, I was aiming for some Markdown-based template, and anyone of them seemed to work for me so I just chose one.

The template lives in [../adr-template.md](../adr-template.md) currently, I did some adjustments to make it simpler:
- No status field since there is no one to approve (personal project)
- No date field, I made it mandatory to name the files with the date (so humans and AI agents can know which file is new by the filename).
- No decision-makers, for the same reason (I am always the decision-maker)
