<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $I_i=[s_i,t_i]$ be an interval whose earliest end triggers greedy meeting $i$. After that meeting, every remaining interval starts strictly after $t_i$: its end is at least $t_i$, and otherwise it would contain $t_i$ and be removed. Hence

$$
s_{i+1}>t_i,\qquad t_1<t_2<\cdots<t_k.
$$

The witness intervals $I_1,\ldots,I_k$ are therefore pairwise disjoint. Every feasible schedule needs a distinct meeting in each one, yielding a lower bound of $k$. The greedy schedule uses exactly $k$ meetings and covers everyone, so **it is optimal**. This is an optimality certificate for the [interval stabbing problem](../../../../../interval-stabbing-problem.md).

To follow the source's suggested contradiction explicitly, suppose a schedule $u_1<\cdots<u_j$ with $j<k$ covered everyone. Since $I_1$ ends at $t_1$, some $u_\ell\leq t_1$, so $u_1\leq t_1$. If $u_i\leq t_i$ and $i<j$, then none of the first $i$ alternative meetings can hit $I_{i+1}$, which starts after $t_i$. A later meeting must hit it by its end $t_{i+1}$, implying $u_{i+1}\leq t_{i+1}$. [Mathematical induction](../../../../../mathematical-induction.md) gives $u_i\leq t_i$ for $1\leq i\leq j$. But $I_{j+1}$ starts after $t_j\geq u_j$, later than every alternative meeting. It is uncovered, a contradiction. For $j=0$ a nonempty family is immediately uncovered. The source's hint starts at index zero without defining $u_0,t_0$; the proof above starts at the actual first meetings instead.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
