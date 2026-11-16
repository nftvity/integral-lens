# Integral Action Planning — From Map to Tasks

The map is only worth something if it changes what people do. This is the method for
turning an AQAL analysis into an **Integral Action Plan**: a balanced, prioritized,
level-appropriate list of tasks.

## Contents
1. Why single-quadrant plans fail
2. The seven steps
3. The tetra-intervention matrix
4. Calibrating tasks to levels, lines, states and types
5. Prioritizing
6. Metrics per quadrant
7. Task schema and export formats
8. Review rhythm

---

## 1. Why single-quadrant plans fail

| Plan only in… | Typical form | Why it fails |
|---|---|---|
| **UL** | "Change your mindset." Motivation talks, affirmations. | Insight without new behavior, support or structure fades in weeks. |
| **UR** | "Just do the habit." Checklists, training, tools. | Behavior without meaning, culture or system support is resisted or abandoned. |
| **LL** | "Let's build a better culture." Values workshops. | Shared values without structures and incentives become posters on walls. |
| **LR** | "Restructure / new process / new software." | New systems run by people with old mindsets and old culture reproduce old results. |

An Integral Action Plan addresses all four, in a sequence that fits the situation.

## 2. The seven steps

1. **State the outcome** in one sentence.
2. **Define "done" in every quadrant.**
   - I: what will people experience, believe, intend?
   - It: what will people do, observably?
   - We: what will be shared — norms, stories, trust?
   - Its: what structures, systems and resources will exist?
3. **Identify the gaps** between now and done, per quadrant (from the analysis).
4. **Design tetra-interventions** — one or more tasks per quadrant per objective (§3).
5. **Calibrate** each task (§4).
6. **Prioritize and sequence** (§5), mark dependencies, choose the first three actions
   for the next 48 hours.
7. **Attach metrics** in every quadrant (§6) and a review date.

## 3. The tetra-intervention matrix

For each objective, fill this grid. Each cell is a task or small set of tasks.

| | Interior | Exterior |
|---|---|---|
| **Individual** | **I-task** — shift awareness, intention, emotional relationship. *Examples:* reflection, coaching, values clarification, shadow work, personal commitment. | **It-task** — change behavior and capacity. *Examples:* habit, skill training, practice routine, health action, the concrete deliverable. |
| **Collective** | **We-task** — shift shared meaning and relationships. *Examples:* a conversation, ritual, shared story, agreement, feedback culture, trust-building. | **Its-task** — change the system. *Examples:* process, incentives, roles, tools, budget, policy, environment design, infrastructure. |

### The Four Ups (tag each task)

- **Wake Up** — work with states: presence, attention, rest, meditation, flow.
- **Grow Up** — support stage development: new perspectives, mentoring, challenge plus
  support, "stretch" assignments.
- **Clean Up** — work with shadow: conflicts, projections, unprocessed emotions,
  repair conversations.
- **Show Up** — embody it in action, relationships, work and the world.

A plan with only "Show Up" tasks is busy; a plan with only "Wake Up" tasks is
pleasant and changes nothing outside.

## 4. Calibrating tasks

Before finalizing any task, check:

- **Level fit.** Will the person doing it find it meaningful from their center of
  gravity? (An Amber team needs clear roles and procedures; an Orange team needs goals
  and autonomy; a Green team needs participation; a Teal team needs purpose and
  freedom.)
- **Translation vs. transformation.** Is this asking people to do their current level
  better (most tasks should) or to grow into a new one (few, well-supported tasks)?
- **Lines.** Does the task depend on a line that is weak? If so, add support or pair
  people.
- **States.** Is this realistic for people in their current state? Burned-out people
  need fewer, smaller tasks — and rest is a task.
- **Types.** Does the plan offer something for different types (reflective and active,
  agency-oriented and communion-oriented)?

## 5. Prioritizing

Score each task:

- **Impact** — High / Medium / Low. Extra weight if it moves several quadrants at once.
- **Effort** — S (≤ 1 day), M (≤ 1 week), L (> 1 week).
- **Leverage** — does it unlock other tasks?
- **Dependencies** — what must happen first?

Sequencing heuristics:

1. **Stabilize states first** when people are in crisis or burnout.
2. **Begin with a We-conversation** when trust is low; structural changes imposed on a
   low-trust culture are read as threats.
3. **Pair every Its-change with a We-change** (explain, co-design, ritualize it).
4. **Make the first It-actions small and visible** to create momentum.
5. **Schedule a Clean Up task** when the same conflict keeps returning.

Always end with **"Start in the next 48 hours"**: three concrete, small, unambiguous
actions with a named owner.

## 6. Metrics per quadrant

Measure in all four quadrants. Not everything that counts can be counted, but most
things can be noticed.

| Quadrant | What to measure | How |
|---|---|---|
| **I** | Motivation, clarity, stress, meaning, confidence | Self-rating 1–10, journal entries, check-in questions |
| **It** | Behaviors, skills, health, output | Habit tracker, observable outputs, biometrics, performance data |
| **We** | Trust, alignment, belonging, psychological safety | Pulse surveys, quality of conversations, retention, stories people tell |
| **Its** | Systems working, KPIs, resources, process speed | Dashboards, cycle time, cost, revenue, error rates |

## 7. Task schema and export formats

### Markdown table (default)

```markdown
| # | Task | Quadrant | Up | Owner | Effort | Impact | Depends on | Due | Done when |
|---|------|----------|----|-------|--------|--------|------------|-----|-----------|
| 1 | Hold a 60-min team retrospective on the last launch | LL | Clean Up | Lead | S | High | — | Fri | Three agreed changes recorded |
```

### Checklist (personal plans)

```markdown
- [ ] (UL · Wake Up) 10 minutes of morning journaling — Mon–Fri
- [ ] (UR · Show Up) Walk 7,000 steps a day
- [ ] (LL · Clean Up) Have the postponed conversation with my partner by Sunday
- [ ] (LR · Show Up) Move the gym bag to the front door
```

### CSV (spreadsheets, Notion, Linear, Jira, Todoist imports)

```csv
id,title,description,quadrant,up,owner,effort,impact,depends_on,due,done_when,metric
1,"Team retrospective","60-min blameless retro on the last launch",LL,Clean Up,Lead,S,High,,2026-11-21,"Three agreed changes recorded","Trust pulse +1"
```

### JSON (automation, GitHub issues, APIs)

```json
{
  "outcome": "Ship v2 without burning out the team",
  "tasks": [
    {
      "id": 1,
      "title": "Team retrospective",
      "description": "60-min blameless retro on the last launch",
      "quadrant": "LL",
      "up": "Clean Up",
      "owner": "Lead",
      "effort": "S",
      "impact": "High",
      "depends_on": [],
      "due": "2026-11-21",
      "done_when": "Three agreed changes recorded",
      "metric": "Trust pulse +1"
    }
  ]
}
```

Use labels such as `quadrant:UL`, `up:clean-up` when creating issues in tools that
support labels.

## 8. Review rhythm

- **Weekly (15 min):** What moved in each quadrant? Which quadrant is lagging?
- **Monthly:** Update the map. Has the center of gravity, state or culture shifted?
- **Per milestone:** Rerun the Integral Lens Protocol on the new situation.

The plan is a living map. When one quadrant stalls, the fix is almost always in a
different quadrant.
