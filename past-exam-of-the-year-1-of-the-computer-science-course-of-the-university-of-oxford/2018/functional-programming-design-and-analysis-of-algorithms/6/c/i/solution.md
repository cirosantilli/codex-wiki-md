<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a Boolean [dynamic programming state](../../../../../../dynamic-programming-state.md) $R(a)$ for whether amount $a$ can be made exactly. Initialize $R(0)=\mathrm{True}$ and, for $a=1,\ldots,v$, compute

$$
R(a)=\bigvee_{i:v_i\leq a} R(a-v_i).
$$

An empty disjunction is false. Any nonempty representation ends in some coin; removing it gives one of the displayed predecessor states, and adding it back proves the converse. **Return $R(v)$**. This takes $O(nv)$ time and $O(v)$ space for positive integer denominations and nonnegative integer target $v$, with unlimited coins of each type.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
