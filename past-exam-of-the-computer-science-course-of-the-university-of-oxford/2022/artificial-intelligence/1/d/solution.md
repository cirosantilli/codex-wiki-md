<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Ordinary [classical planning](../../../../../classical-planning.md) with [STRIPS](../../../../../strips.md) starts from one completely specified state. Here the missing locations express ignorance: not listing a pit or a monster at a room does not establish its absence. Applying the [closed-world assumption](../../../../../closed-world-assumption.md) to those omissions would manufacture knowledge of safety. Moreover, future sensor readings can determine which action is appropriate, so a fixed action sequence need not suffice.

The suitable object is a [belief state](../../../../../belief-state.md) and a [contingent plan](../../../../../contingent-planning.md) that branches on observations. A finite [belief state](../../../../../belief-state.md) model could in principle be compiled into a larger [classical planning](../../../../../classical-planning.md) instance, but the ordinary physical-state [STRIPS](../../../../../strips.md) representation does not directly represent the required uncertainty and sensing.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
