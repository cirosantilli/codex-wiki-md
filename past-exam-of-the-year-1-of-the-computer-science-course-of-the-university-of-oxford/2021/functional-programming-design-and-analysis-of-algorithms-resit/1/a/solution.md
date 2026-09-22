<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The empty-[list](../../../../../list-abstract-data-type.md) case uses $f(a)=b$. At a cons, assuming the equality for the tail, the calculation is

$$
f(\operatorname{foldr}\ g\ a\ (x:xs))=f(g\ x\ (\operatorname{foldr}\ g\ a\ xs))=h\ x\ (f(\operatorname{foldr}\ g\ a\ xs))=h\ x\ (\operatorname{foldr}\ h\ b\ xs).
$$

The middle equality is the supplied compatibility condition, instantiated with the folded tail; the last expression is the [right fold](../../../../../list-fold.md) on the whole [list](../../../../../list-abstract-data-type.md). [Structural induction](../../../../../structural-induction.md) therefore proves fusion for finite total spines.

The strictness condition accounts for a bottom-valued input spine: the inner [list fold](../../../../../list-fold.md) returns bottom, and $f(\bot)=\bot$ makes the two sides agree. The same [induction](../../../../../mathematical-induction.md) covers finite [partial lists](../../../../../partial-list.md). For pure definable continuous [functions](../../../../../function-split.md), an infinite [list](../../../../../list-abstract-data-type.md) is the limit of its finite partial approximations, so equality extends to it. These are the three distinct obligations in the [right-fold fusion law](../../../../../right-fold-fusion-law.md); strictness is not needed if the domain is restricted to finite terminating spines.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
