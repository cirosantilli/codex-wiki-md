<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here is an explicit [Braess paradox](../../../../../../braess-s-paradox.md). Use four vertices $s,a,b,t$ and unit demand from $s$ to $t$. The delay on $s\to a$ equals its own link flow, as does the delay on $b\to t$; the delays on $a\to t$ and $s\to b$ are constantly one. Initially the two routes are $s\to a\to t$ and $s\to b\to t$. If the first carries $u$ and the second $1-u$, their delays are $1+u$ and $2-u$. The [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) has $u=1/2$, so **every traveler takes time $3/2$**.

Add a directed link $a\to b$ with zero delay. Let the old upper and lower routes carry $a_0,b_0$, and let the new route $s\to a\to b\to t$ carry $z$, with $a_0+b_0+z=1$. Their delays become

$$
L_{\rm upper}=1+a_0+z,\qquad L_{\rm lower}=1+b_0+z,\qquad L_{\rm middle}=a_0+b_0+2z=1+z.
$$

If $a_0>0$, the upper route is strictly slower than the middle route, contradicting the [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) condition. Similarly $b_0>0$ is impossible. Thus the new equilibrium has $z=1$, and all three route delays are two. Consequently

$$
\boxed{\text{Adding a zero-delay link raises equilibrium delay from }3/2\text{ to }2.}
$$

This is an incentive effect, not a loss of feasible allocations: the old half-and-half flow remains feasible after adding the link. For completeness, its social optimality can be checked directly. Write $a_0=(1-z)/2+h$, $b_0=(1-z)/2-h$. Total travel time in the enlarged network is

$$
D=(a_0+z)^2+(b_0+z)^2+a_0+b_0=\frac32+\frac{z^2}{2}+2h^2.
$$

It is minimized at $z=h=0$, giving the original total time $3/2$. The [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md) instead incurs total time two, a factor $4/3$ larger. The [Beckmann potential](../../../../../../beckmann-potential.md) and total-delay objectives differ because an extra traveler ignores the delay their presence imposes on others. More generally, adding routes cannot worsen the optimum of total delay when it leaves the previous feasible flows available, but it can worsen a selfish [Wardrop equilibrium](../../../../../../wardrop-equilibrium.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
