---
title: The Person Who Knows Is a Bottleneck
layout: post
subtitle: Valuable Knowledge
tags:
  - AI
  - coding
---
This may show up everywhere, but as a software engineer it's where I see it most often: two developers on the same team, using the same tool, working in the same codebase, can produce wildly different results. Not because the model is inconsistent. Because their prompts are.

The senior engineer asks for a new service and naturally specifies the architecture pattern, the error-handling approach, the logging conventions. The junior just asks the AI to "create a notification service". Same tool, but completely different output.

This isn't a *skills* problem. It's a *systems* problem, and we keep solving it the wrong way.

We keep trying to fix it the old way: more docs, more pairing, more "knowledge sharing sessions". It helps a little, but it's slow as hell and doesn't scale. The real knowledge already exists on the team, it just lives in a few people's heads and transfers slowly through mentorship and code review. I've run enough code reviews to know how much unspoken knowledge just... never survives that transfer. The industry is changing so fast but we're still building teams around the one person who knows (or thinks they know).

What actually works is treating the prompts like infrastructure.

When your team's standards are encoded into shared, versioned instruction sets (living in the repository, updated through pull requests) they stop being unwritten rules and start behaving like linting rules or CI pipelines. The junior developer doesn't need to know what the senior would ask for. They just invoke the instruction. The team's actual judgment runs on autopilot.

And yeah, it compounds. Every gap the instructions miss becomes a PR. Every production incident becomes another rule. The standards **actually** get better over time instead of living in one person's head.

We've been treating expert judgment like something you absorb over time. It can just be a file in the codebase.
