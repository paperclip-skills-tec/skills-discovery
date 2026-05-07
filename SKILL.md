---
name: skills-discovery
description: Standing responsibility for all agents to identify opportunities for new skills and improvements to existing skills. Use when you notice a repeating workflow, a gap in guidance, or a place where an existing skill could be improved. Defines how to raise proposals and the approval gates before any skill is created or changed.
---

# Skills Discovery & Governance

## Standing Responsibility

Every agent has a standing responsibility to watch for skill opportunities during their normal work. This does **not** require a separate heartbeat — it is an ongoing awareness check.

### When to raise a proposal

Raise a skill proposal when you notice any of the following:

- A task required improvisation that a skill would have guided
- You repeated the same multi-step reasoning more than twice with no skill to anchor it
- An existing skill produced an output in the wrong format, missed an edge case, or gave outdated advice
- You found a better approach to a problem a skill already covers
- A new tool, API, or workflow exists that agents aren't yet equipped to use well

### When NOT to raise a proposal

- One-off or highly context-specific tasks (no repeatable pattern)
- Minor wording tweaks that don't change guidance (fix inline, don't propose)
- Anything already covered by an existing skill with a small extension

---

## How to Raise a Proposal

Create a TEC issue (do **not** implement or prototype the skill first):

```
goalId: 86792fd3-dbe0-40e4-a585-875aac7a2d1e   ← Skills Discovery & Governance
assigneeAgentId: 7de0f97a-1196-456c-8ef0-073eac20e67b   ← Chief of Staff
status: todo
title: [Skill Proposal] <Skill Name>
   OR: [Skill Improvement] <Skill Name>
```

**Description template:**

```markdown
## Skill Proposal

**Type:** New skill | Improvement to existing skill
**Skill name / target:** <name, or which skill to improve>
**Problem it solves:** <what gap, pain point, or failure mode>
**Agents that benefit:** <list or "all">
**Example trigger:** <what user message or situation would invoke this>
**Estimated complexity:** Low | Medium | High
**Draft content (optional):** <outline or proposed change>
```

File the issue and stop. The Chief of Staff picks it up from there.

---

## Approval Gates

| Type | Approver | Time |
|---|---|---|
| Minor improvement (bug fix, edge case, wording, stale reference) | Chief of Staff | 1 heartbeat |
| New skill | Board | Board review cycle |
| Major rework (new trigger, renamed skill, multi-agent impact) | Board | Board review cycle |

You will be notified on the proposal issue when a decision is made.

---

## Implementation

After approval, the Chief of Staff assigns implementation to the `skill-creator` skill. You do not need to do anything unless asked. If you are assigned the implementation, use the `skill-creator` skill.

---

## Governance Notes

- All proposals are tracked under goal [Skills Discovery & Governance](/TEC/goals/86792fd3-dbe0-40e4-a585-875aac7a2d1e)
- No agent may modify another agent's assigned skills without Chief of Staff approval
- Skills are shared company assets — proposals from any agent are welcome and valued

---

*TEC Custom Skill — maintained by the Deltek Technical Services Engineering team.*