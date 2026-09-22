<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [query certificate](../../../../../../query-certificate.md) for input $x$ is a subset $S$ of coordinates such that every $y$ agreeing with $x$ on $S$ has the same value of $f$. Define [certificate complexity of a Boolean function](../../../../../../certificate-complexity-of-a-boolean-function.md) by

$$
C(f,x)=\min\{|S|:S\text{ certifies }f(x)\},\quad C_b(f)=\max_{f(x)=b}C(f,x),\quad C(f)=\max(C_0,C_1).
$$

If no input has output $b$, take $C_b(f)=0$. Unlike a [decision tree](../../../../../../decision-tree.md), a [query certificate](../../../../../../query-certificate.md) may be selected with full knowledge of the input.

Take a full [star graph](../../../../../../star-graph-theory.md) centered at $v$, containing all $n-1$ incident edges and no others. For any edge $e$ not incident to $v$, changing only its bit from zero to one destroys the [common-center graph property](../../../../../../common-center-graph-property.md): two spokes already force $v$ as the only possible common endpoint. Therefore every positive [query certificate](../../../../../../query-certificate.md) for this input must include every nonincident edge bit, otherwise this one-bit change would preserve its answers but change the output. There are $\binom{n-1}{2}$ such bits. Conversely, fixing all those bits to zero suffices for a [query certificate](../../../../../../query-certificate.md), because all remaining edges are incident to $v$. Hence

$$
\boxed{C_1(\mathrm{STAR}_n)=\binom{n-1}{2},\qquad C(\mathrm{STAR}_n)=\Omega(n^2)}.
$$

The upper bound for $C_1$ holds for any accepted [graph](../../../../../../graph-split.md) by choosing any valid center and certifying its nonincident edges absent.

For completeness, the negative side is much smaller. Given a [graph](../../../../../../graph-split.md) with no common center, choose a present edge $\{a,b\}$, an edge not containing $a$, and an edge not containing $b$. These at most three present edges have empty common intersection and certify rejection. A triangle with isolated additional vertices needs all three of its present edges: with at most two queries, set every unqueried edge absent and the remaining present edges share a vertex. Thus the [certificates for the common-center graph property](../../../../../../certificates-for-the-common-center-graph-property.md) satisfy

$$
\boxed{C_0(\mathrm{STAR}_n)=3,\qquad C(\mathrm{STAR}_n)=\max\left\{3,\binom{n-1}{2}\right\}\quad(n\geq3)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
