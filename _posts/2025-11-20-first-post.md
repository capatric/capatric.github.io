---
layout: post
title: "Reliability work starts with fewer hidden states"
date: 2025-11-20
description: Why simplifying operational state is one of the fastest ways to make systems easier to trust.
excerpt: "The fastest reliability gains often come from removing ambiguity, not adding more dashboards."
---

When a system feels unreliable, the first instinct is often to add more visibility: more alerts, more dashboards, more checks. That helps, but only up to a point.

The faster improvement usually comes from reducing the number of hidden states the system can enter.

## Hidden state is expensive

Operational work gets harder when the real system state is spread across too many places:

- manual steps that live in someone’s memory
- service dependencies that are not modeled clearly
- recovery paths that depend on timing or order
- tooling that succeeds silently even when part of the job failed

Each of those conditions forces engineers to guess. Reliability drops because the team is operating on incomplete information.

## What to simplify first

I usually start with three questions:

1. Can the system describe its own current state clearly?
2. Can an operator tell what failed without reading source code or tribal knowledge?
3. Can the recovery path be repeated the same way every time?

If the answer is no, the problem is not only observability. It is design.

## Good operational design looks boring

The best systems are rarely dramatic. They expose clear status, fail in obvious ways, and recover through a narrow set of well-tested actions.

That kind of boring behavior is valuable. It reduces time spent interpreting the platform and increases time spent actually fixing problems.

## Closing thought

Reliability work is often framed as resilience under failure. In practice, a large part of it is simpler: remove ambiguity until the system becomes easier to reason about.
