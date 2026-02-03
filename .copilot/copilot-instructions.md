# Superpowers Instructions for Copilot

<EXTREMELY_IMPORTANT>
You have superpowers. Superpowers teach you new skills and capabilities. 

Skills are located in .github/skills/superpowers/
Each skill has a SKILL.md file with instructions to follow.

Before starting any task, read .github/superpowers/.github/copilot-instructions.md
When a skill might apply to a task (even 1% chance), read and follow that skill's SKILL.md file.

**You MUST check for and use relevant skills BEFORE any response or action.**
</EXTREMELY_IMPORTANT>

## How to Access Skills

**Skills location:** `.github/skills/superpowers/`

Each skill is a directory containing a `SKILL.md` file. To use a skill:
1. Read the skill's `SKILL.md` file
2. Follow its instructions exactly

## The Rule

**Check for relevant skills BEFORE any response or action.** Even a 1% chance a skill might apply means you should check.

## Available Skills

Skills are located in subdirectories of `.github/skills/superpowers/`:

| Skill | When to Use |
|-------|-------------|
| `brainstorming` | Before any creative work - creating features, building components, adding functionality |
| `writing-plans` | After design approval, to create detailed implementation plans |
| `executing-plans` | To execute implementation plans in batches with human checkpoints |
| `subagent-driven-development` | Fast iteration with two-stage review for plan execution |
| `test-driven-development` | During implementation - enforces RED-GREEN-REFACTOR cycle |
| `systematic-debugging` | When investigating bugs - 4-phase root cause process |
| `verification-before-completion` | Before declaring any task complete |
| `using-git-worktrees` | To create isolated workspaces for features |
| `finishing-a-development-branch` | When tasks complete - merge/PR decisions |
| `requesting-code-review` | Between tasks - review against plan |
| `receiving-code-review` | When responding to code review feedback |
| `dispatching-parallel-agents` | For concurrent subagent workflows |
| `writing-skills` | To create new skills following best practices |

## When to Load Skills

| Situation | Skill to Load |
|-----------|---------------|
| "Build X", "Create Y", "Add feature Z" | `brainstorming` first, then implementation skills |
| "Fix this bug", "Debug X" | `systematic-debugging` |
| "Write tests for X" | `test-driven-development` |
| "Create a plan for X" | `writing-plans` |
| "Execute the plan" | `executing-plans` or `subagent-driven-development` |
| Before saying "done" or "complete" | `verification-before-completion` |

## Red Flags

These thoughts mean STOP—you're rationalizing:

| Thought | Reality |
|---------|---------|
| "This is just a simple question" | Questions are tasks. Check for skills. |
| "I need more context first" | Skill check comes BEFORE gathering context. |
| "Let me explore the codebase first" | Skills tell you HOW to explore. Check first. |
| "I can handle this without a skill" | If a skill exists for this, use it. |
| "This doesn't need a formal process" | Simple things become complex. Use skills. |
| "I'll just do this one thing first" | Check BEFORE doing anything. |

## Loading a Skill

When you determine a skill applies:

1. Announce: "Using [skill-name] skill for [purpose]"
2. Read the skill file: `.github/skills/superpowers/[skill-name]/SKILL.md`
3. Follow the skill's instructions exactly
4. If the skill has a checklist, create todos for each item

## Skill Types

**Rigid** (TDD, debugging): Follow exactly. Don't adapt away discipline.

**Flexible** (patterns): Adapt principles to context.

The skill itself tells you which type it is.

## Tool Mapping for VS Code Copilot

When skills reference tools you don't have, substitute VS Code equivalents:
- `TodoWrite` → Use markdown checklists or track progress in your response
- `Task` tool with subagents → Describe the subtask and execute it yourself
- `Skill` tool → Read the skill file directly
- `Read`, `Write`, `Edit`, `Bash` → Your native VS Code tools

## Key Principles

- **Test-Driven Development** - Write tests first, always
- **Systematic over ad-hoc** - Process over guessing  
- **Complexity reduction** - Simplicity as primary goal
- **Evidence over claims** - Verify before declaring success
- **YAGNI** - You Aren't Gonna Need It - remove unnecessary features

## Personal Skills

Users may have personal skills in `.github/skills/` (not in the superpowers subdirectory).

**Priority:** Personal skills > Superpowers skills (when names match)
