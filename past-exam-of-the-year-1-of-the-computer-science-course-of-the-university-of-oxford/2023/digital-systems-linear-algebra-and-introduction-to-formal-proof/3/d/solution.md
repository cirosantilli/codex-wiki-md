<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Four state [bits](../../../../../bit.md) are necessary and sufficient.** For each output value, distinguish three armed situations, remembering a trailing high run of length $0,1,2$, and three disarmed situations, remembering a trailing low run of length $0,1,2$. Thus a direct minimal behavioural description has

$$
2(3+3)=12\text{ states},\qquad\lceil\log_2 12\rceil=4\text{ bits}.
$$

All twelve situations are reachable. Different output values are immediately distinguishable. Within an armed group, a suitable number of high samples distinguishes the three run lengths by when the next toggle occurs. Within a disarmed group, a suitable number of low samples followed by three highs distinguishes the three rearming distances. An armed situation and a disarmed situation of the same output value are distinguished by an all-high continuation: the armed one eventually toggles and the disarmed one does not. Hence these twelve situations cannot be merged in a [finite-state machine](../../../../../finite-state-machine.md) implementing the specification.

The shared-history design in (c) uses four [bits](../../../../../bit.md), meeting this lower bound. Its sixteen encoded states have some behaviourally equivalent histories, so its encoding need not use only twelve combinations. Building two separate copies of (a) plus the two-[bit](../../../../../bit.md) module (b) would use six state-bearing elements; sharing the input history saves two.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
