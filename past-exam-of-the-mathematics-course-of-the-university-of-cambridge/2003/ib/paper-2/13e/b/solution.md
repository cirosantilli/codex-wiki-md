<h1 id="13e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The set $Y$ is [path-connected](../../../../../../path-connected-space.md) as the continuous image of $[1,\infty)$, hence connected. Its closure is $Y$ together with the unit circle. Indeed $g(k+\theta/(2\pi))\to e^{i\theta}$ as $k\to\infty$, and any convergent sequence of spiral points either has bounded parameters, giving a point of $Y$, or has parameters tending to infinity along a subsequence, giving radius one. The closure of a connected set is connected: a separation of its closure would induce a separation of the dense original set, with neither open part missing that set. The closed disk is connected and meets this closure in the unit circle; their union $Y\cup\overline D$ is therefore **connected**.

To show it is not [path-connected](../../../../../../path-connected-space.md), suppose a path $\alpha:[0,1]\to Y\cup\overline D$ starts in $Y$ and ends in the disk. Let $u_*$ be its first contact with the disk. The disk is closed, so this first contact exists, and $u_*>0$. Before it, the path belongs to $Y$ and has a continuous uniquely determined parameter

$$
t(u)=\frac1{|\alpha(u)|-1},\qquad\alpha(u)=g(t(u)).
$$

[Continuity](../../../../../../continuous-function.md) at contact forces $|\alpha(u_*)|=1$, and hence $t(u)\to\infty$ as $u\uparrow u_*$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) supplies times approaching $u_*$ at which $t(u)$ is an integer, and other times at which it is an integer plus $1/2$. These times must approach contact because $t$ is bounded on every compact interval strictly before it. Along the first sequence $\alpha(u)\to1$; along the second it tends to $-1$. This contradicts [continuity](../../../../../../continuous-function.md) at $u_*$. Thus **no path joins the spiral to the disk**, proving failure of path-[connectedness](../../../../../../connected-space.md) for the [spiral accumulating on a circle](../../../../../../spiral-accumulating-on-a-circle.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13E](../../13e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
