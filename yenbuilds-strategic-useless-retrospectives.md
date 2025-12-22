# Structural Retrospectives

Retrospectives are **worse than useless** if they focus on one-off mistakes, edge cases, or narrative explanations.  
They create the *illusion* of learning while guaranteeing recurrence.

This operating system rejects retrospectives unless they operate **at the level of structure**.

---

## The Core Principle

> **Outcomes are not caused by individuals.  
They are caused by systems.**

If an outcome can reoccur with a different competent person in the same environment, it is **structural**.  
If it cannot, it is **noise**.

Only structural forces are worth analyzing.

---

## Why Traditional Retrospectives Fail

Most retrospectives:
- Catalog **symptoms**, not causes
- Focus on **events**, not incentives
- Optimize for **closure**, not causality
- Produce “action items” that don’t change the system

They ask:
> *“What went wrong?”*

When the only meaningful question is:
> **“What made this outcome the default?”**

If the system remains unchanged, the retro achieved nothing.

---

## The Structural Retrospective Test

Before discussing *any* issue, apply this filter:

> **If this situation replayed with a different competent person, would it still happen?**

- **Yes** → Structural → Worth analyzing  
- **No** → Edge case → Ignore it

This single question eliminates most retro noise.

---

## The Only Forces That Actually Cause Recurring Failure

Nearly all repeat failures reduce to one or more of the following:

### 1. Incentive Misalignment
People did what the system rewarded.

Examples:
- Speed rewarded over stability
- Visibility rewarded over correctness
- New features rewarded, deletions ignored

If incentives don’t change, behavior won’t change.

---

### 2. Energy Gradient Mismatch

The “correct” action requires more effort than the incorrect one.

Examples:
- The safe path is slower than the risky path
- The documented path is harder than tribal knowledge
- Fixing technical debt carries political or emotional cost

Humans follow the **path of least resistance**, not ideals.

**Concrete Example: Bureaucratic Change Control**

A formal change control process is introduced to “prevent errors.”

In practice:
- Submitting a change requires multiple forms, meetings, and approvals
- The process is slow, emotionally draining, and reputation-risking
- Reviews focus on compliance (boxes checked, approvals present), not substance
- Real failure modes are rarely surfaced or meaningfully challenged

As a result:
- Engineers batch changes to avoid repeated overhead
- Small fixes are delayed or bundled into larger changes
- Changes are described strategically to avoid scrutiny
- Workarounds become normalised

The system unintentionally rewards:
- Fewer but larger changes
- Reduced transparency
- Risk concentration
- Ritual compliance over correctness

The “correct” behaviour (small, frequent, well-scoped changes) is made expensive.  
The “incorrect” behaviour (bundling, hiding, rushing) is made efficient.

People do not bypass change control because they are careless.  
They bypass it because the energy gradient is misaligned.

This is not a failure of discipline.  
It is a failure of design.

---

### 3. Feedback Delay or Absence
Consequences arrived too late to influence behavior.

Examples:
- Bugs surfaced weeks later
- Operational pain felt by a different team
- Long-term costs invisible at decision time

Delayed feedback prevents learning.

---

### 4. Local Optimization vs System Health

Subcomponents optimize themselves at the expense of the whole.

Examples:
- Throughput is maximized while stability degrades
- KPIs conflict across team or system boundaries
- Ownership stops at interfaces rather than outcomes

Systems get the behavior they reward.

**Role of Tight (and Broken) Feedback Loops**

Local optimization thrives when feedback is:
- Immediate at the local level
- Delayed, diffused, or invisible at the system level

In these conditions:
- Teams receive fast reinforcement for local wins
- System-wide costs surface too late to influence behavior
- Pain is experienced by downstream teams, not the optimizers

As a result:
- Metrics improve while the system worsens
- Success is measured where feedback is tight, not where impact is real
- Local efficiency masks global fragility

Healthy systems align feedback loops such that:
- The cost of local optimization is felt locally
- System-level failures propagate quickly and visibly
- Incentives reflect end-to-end outcomes, not partial wins

When feedback is misaligned, rational actors will optimize locally.  
This is not selfishness — it is predictable behavior.

The failure is not in execution.  
It is in feedback and incentive design.

---

### 5. Cognitive Load Overload

Correct operation requires sustained vigilance or individual heroics.

Examples:
- Too many rules to remember and apply correctly
- Critical knowledge remains implicit or tribal
- Success depends on individuals “being careful” or “remembering next time”

**Any system that relies on attention instead of constraints is already broken.**

**Concrete Failure Modes**

In cognitively overloaded systems:
- Operators must mentally simulate the system to avoid failure
- Correct sequencing exists only in people’s heads
- Safety depends on experience, not structure
- Mistakes are framed as carelessness rather than predictability

**Common Organisational Examples**

- Deployment processes that require remembering undocumented steps  
- Safety procedures that live in slide decks, not in tooling  
- Manual environment switches with no guardrails  
- Configuration flags that can be toggled into invalid states  
- Systems where “senior people” are required to supervise routine work  

**Second-Order Effects**

These systems:
- Punish newcomers disproportionately
- Create knowledge bottlenecks around a few individuals
- Encourage fear-driven conservatism or over-checking
- Fail catastrophically under stress, fatigue, or interruption

**Structural Correction**

Robust systems:
- Encode correctness into defaults
- Make invalid states unrepresentable
- Fail fast and visibly
- Reduce the need for memory, vigilance, or heroics

If success requires constant attention, failure is only a mental lapse away.

This is not a training problem. It is an architecture problem.

---

## The Only Acceptable Closing Question

> **How do we make the correct behavior the path of least resistance?**

If this cannot be answered concretely, the retrospective should end immediately.

---

## Operating System Rule

> **Do not spend time explaining failures.  
Spend time making them structurally impossible.**

All other retrospectives are theater.
