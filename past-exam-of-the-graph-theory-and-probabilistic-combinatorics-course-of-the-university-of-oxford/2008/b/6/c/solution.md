<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z_r$ be the size of generation $r$, with $Z_0=1$. Its offspring mean is $2p$, so conditioning on the previous generation gives $\mathbb EZ_r=(2p)^r$. At $p=1/2$,

$$
\boxed{\mathbb EZ_r=1\text{ for every }r,\qquad\mathbb EK=\sum_{r\ge0}\mathbb EZ_r=\infty}.
$$

The interchange uses [Tonelli's theorem](../../../../../tonelli-theorem.md) for nonnegative variables. Critical extinction is nevertheless almost sure: its probability is the smallest root in $[0,1]$ of $s=(1+s^2)/2$, whose only root is one. Hence $K$ is finite almost surely. If all its finite atoms had the exponential bound, then $\mathbb EK\le\sum_{k\ge1}ke^{-ck}<\infty$, a contradiction.

For $p>1/2$ the extinction probability is $(1-p)/p<1$. There is positive mass at $K=\infty$, so the mean is infinite even if every finite atom decays exponentially. This is precisely why the critical contradiction does not extend to the supercritical case.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
