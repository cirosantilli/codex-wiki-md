<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [closed balls](../../../../../closed-ball.md) with centres belonging to the space being covered. The [covering number](../../../../../metric-covering-number.md) is

$$
\boxed{N(\varepsilon;R,\rho)=\min\left\{|A|:A\subseteq R,\ R\subseteq\bigcup_{a\in A}\overline B_\rho(a,\varepsilon),\ |A|<\infty\right\},}
$$

with value $\infty$ if there is no finite [metric net](../../../../../metric-net.md), and value zero for the empty space.

With this intrinsic-centre convention, **the proposed monotonicity under subsets is false**. Give $R=\{-1,0,1\}$ the usual distance, take $S=\{-1,1\}$, and set $\varepsilon=3/2$. A ball centred at $0$ covers $R$, so $N(3/2;R,\rho)=1$. The two points of $S$ are distance $2$ apart, so a ball centred in $S$ contains only its centre, and $N(3/2;S,\rho)=2$. These values are also valid with [open balls](../../../../../open-ball.md).

The obstruction is that the useful centre $0$ disappears on passing to the subspace. If centres were allowed anywhere in a fixed ambient space, monotonicity would hold. With intrinsic centres, one instead has

$$
\boxed{N(2\varepsilon;S,\rho)\leq N(\varepsilon;R,\rho).}
$$

Indeed, discard covering balls missing $S$ and choose one point of $S$ from each remaining ball. The [triangle inequality](../../../../../triangle-inequality.md) shows that every point of its intersection with $S$ is within $2\varepsilon$ of the chosen point. This proves the replacement bound whenever the right side is finite; otherwise it is automatic.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
