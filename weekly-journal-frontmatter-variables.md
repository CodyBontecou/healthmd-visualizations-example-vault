---
journal-start: 2026-04-13
journal-end: 2026-04-19
tags:
  - healthmd/example
---

# Weekly Journal — Frontmatter Date Variables

This note demonstrates the reusable weekly-journal pattern for Health.md date variables.

The `health-viz` blocks below always use the same variable names:

```yaml
from: {journal-start}
to: {journal-end}
```

Each weekly note can reuse the same blocks, while the results change based on that note's Properties/frontmatter:

```yaml
journal-start: 2026-04-13
journal-end: 2026-04-19
```

To make another weekly note, duplicate this note or use it as a template, then change only the `journal-start` and `journal-end` property values.

---

## Weekly Steps

A fixed week of steps, pinned to this note's `journal-start` → `journal-end` properties.

```health-viz
type: step-spiral
from: {journal-start}
to: {journal-end}
height: 420
```

---

## Weekly Activity Bars

```health-viz
type: bar-chart
metric: steps
from: {journal-start}
to: {journal-end}
height: 220
goal: 10000
```

---

## Heart Range This Week

```health-viz
type: heart-range
from: {journal-start}
to: {journal-end}
height: 220
```

---

## Sleep Schedule This Week

```health-viz
type: sleep-schedule
from: {journal-start}
to: {journal-end}
height: 260
sleepGoal: 8
```

---

## Workouts This Week

```health-viz
type: workout-log
from: {journal-start}
to: {journal-end}
height: 160
```
