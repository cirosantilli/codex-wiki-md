<h1 id="16f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Knaster-Tarski theorem](../../../../../../knaster-tarski-theorem.md) says that the fixed points of a monotone self-map of a complete lattice form a complete lattice. In particular,

$$
\operatorname{lfp}(f)=\bigwedge\{x:f(x)\leq x\},
\qquad
\operatorname{gfp}(f)=\bigvee\{x:x\leq f(x)\}.
$$

For the first formula, let $a$ be the displayed meet. Monotonicity gives $f(a)\leq f(x)\leq x$ for every prefixed point $x$, hence $f(a)\leq a$. Then $f(f(a))\leq f(a)$, so $f(a)$ is itself prefixed; minimality of $a$ gives $a\leq f(a)$. Thus $f(a)=a$. The dual argument gives the greatest fixed point. Applying the same construction above the join of any family of fixed points, and dually below its meet, supplies joins and meets within the fixed-point set.

A down-set contains every element below any of its members. Arbitrary unions and intersections of down-sets are down-sets. Thus the down-sets of $X$, ordered by inclusion, have joins given by unions and meets by intersections, so they form a complete lattice.

For the requested counterexample, take

$$
X=[0,1),\qquad Y=[0,1]
$$

with their usual orders. The set $X$ is a down-set in $Y$, while $Y$ is order-isomorphic to the down-set $[0,1/2]$ of $X$. They are not isomorphic because $Y$ has a greatest element and $X$ does not.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [16F](../../16f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
