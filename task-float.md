# Task float

↑ **Parent:** [Critical path method](critical-path-method.md)

[Task float](task-float.md), also called [total float](task-float.md) or [task slack](task-float.md), measures an activity's available start-time delay relative to its earliest start, while allowing a feasible schedule that meets the fixed project finish. For earliest start $E_i$, latest start $L_i$, and fixed duration $\tau_i$, it is

$$
\mathrm{TF}_i=L_i-E_i=(L_i+\tau_i)-(E_i+\tau_i).
$$

In the six-activity [project scheduling](project-scheduling.md) example with start zero and finish 10, B has [task float](task-float.md) 2 and E has [task float](task-float.md) 6. B can move from the interval $[3,5]$ to $[5,7]$, and E from $[0,3]$ to $[6,9]$, without changing D's or F's earliest starts. A, C, D, and F have zero [task float](task-float.md). With the finish fixed to the optimal duration and the basic [critical path method](critical-path-method.md) assumptions, zero [task float](task-float.md) identifies exactly the activities lying on at least one critical [graph path](path-in-a-graph.md). See [Hendrickson, §10.4, Activity Float and Schedules](https://www.cmu.edu/cee/projects/PMbook/10_Fundamental_Scheduling_Procedures.html#10.4).

[Task float](task-float.md) is not generally an independent allowance that can be spent separately on every activity. For a small example, let two duration-1 activities X then Y form one chain, running in parallel with a separate duration-4 activity. The optimal finish is 4. X has earliest/latest starts 0/2 and Y has earliest/latest starts 1/3, so each has [task float](task-float.md) 2. Delaying X to 2 forces Y to start at 3, using Y's allowance too. Choosing X at its latest start 2 and Y at its earliest start 1 violates precedence, although both chosen times lie inside their individual ranges. The [optimization constraints](optimization-constraint.md) still couple the decisions. Here B and E can both use their full [task floats](task-float.md) together because they lie on separate branches; that freedom must be checked from the [Directed acyclic graph](directed-acyclic-graph.md).

// Target: mathematical-optimization.bigb

## ↑ Ancestors (6)

1. [Critical path method](critical-path-method.md)
2. [Project scheduling](project-scheduling.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Critical path method](critical-path-method.md)
- [Task float](task-float.md)
