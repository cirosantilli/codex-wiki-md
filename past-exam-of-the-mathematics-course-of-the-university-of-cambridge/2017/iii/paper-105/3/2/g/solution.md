<h1 id="3/2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

If $u_0=v_0$, the right-hand side of the [local L1 contraction for scalar conservation laws](../../../../../../../local-l1-contraction-for-scalar-conservation-laws.md) estimate is zero. Applying it on a countable collection of rational intervals and final times proves $u=v$ almost everywhere in space-time. Thus

$$
\boxed{\text{bounded entropy solutions with the same data are unique}.}
$$

To deduce nonnegativity one needs a one-sided comparison, rather than merely putting $v=0$ in the absolute-value estimate. The difference $w=u-v$ satisfies the weak equation with flux $f(u)-f(v)$. Subtract its weak integral identity from the [Kato inequality for scalar conservation laws](../../../../../../../kato-inequality-for-scalar-conservation-laws.md) and divide by two. The result is the same inequality for

$$
w_-=(|w|-w)/2,\qquad q_-=(Q(u,v)-f(u)+f(v))/2.
$$

When $w\ge0$ both expressions vanish; when $w<0$, $|q_-|\le Mw_-$. The shrinking-interval proof therefore bounds the negative part by its initial negative part. This is [order preservation for scalar entropy solutions](../../../../../../../order-preservation-for-scalar-entropy-solutions.md).

The constant $v=0$ is an [entropy solution](../../../../../../../entropy-solution.md) for every $f$, even if $f(0)\ne0$, because the constant flux has zero spatial [derivative](../../../../../../../derivative.md). If $u_0\ge0$, its initial negative part is zero, and comparison gives

$$
\boxed{u(t,x)\ge0\quad\text{almost everywhere}.}
$$

This explicitly establishes the additional sign conclusion without incorrectly identifying uniqueness alone with order preservation.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
