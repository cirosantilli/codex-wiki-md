<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Cover the product by $U_0=\mathbb C_z\times\mathbb C_w$ and $U_\infty=\mathbb C_\zeta\times\mathbb C_w$, with $\zeta=1/z$ on their intersection $\mathbb C^*\times\mathbb C$. The permitted vanishing and the [Dolbeault theorem](../../../../../../dolbeault-theorem.md) make this an [acyclic cover](../../../../../../acyclic-cover.md) for both $\mathcal O$ and $\Omega^2$. The [acyclic cover theorem](../../../../../../leray-s-theorem.md) lets its two-term Čech complex compute the cohomology. In particular, all groups with $q\geq2$ vanish.

For $p=0$, a global [holomorphic function](../../../../../../holomorphic-function.md) is constant on each compact [complex projective line](../../../../../../complex-projective-line.md) fibre, by the [maximum modulus principle](../../../../../../maximum-modulus-principle.md). Its remaining dependence on $w$ is entire. Hence $H^{0,0}_{\bar\partial}=\mathcal O(\mathbb C)$. For the first Čech group, a function on the intersection has a [Laurent series](../../../../../../laurent-series.md)

$$
 F(z,w)=\sum_{j\in\mathbb Z}a_j(w)z^j.
$$

Each coefficient is entire in $w$ by its [Cauchy integral formula](../../../../../../cauchy-integral-formula.md). The nonnegative powers extend to $U_0$, and the negative powers extend to $U_\infty$ in coordinate $\zeta$. These two series converge locally uniformly with the parameter $w$, by the usual Laurent estimates on compact parameter sets. Thus every intersection function is a [Čech coboundary](../../../../../../cech-coboundary.md) and $H^{0,1}_{\bar\partial}=0$.

For $p=2$, write a two-form on the intersection as $F(z,w)dz\wedge dw$. The other chart has

$$
 d\zeta\wedge dw=-z^{-2}dz\wedge dw.
$$

Forms extending from $U_0$ have coefficient powers $j\geq0$; those extending from $U_\infty$ have powers $j\leq-2$. A globally defined two-form would need to have both types of expansion, so it is zero. In the first Čech quotient, precisely the $z^{-1}$ term remains, and its coefficient is an arbitrary [entire function](../../../../../../entire-function.md) of $w$. Consequently

$$
 \boxed{
 H_{\bar\partial}^{p,q}(\mathbb P^1\times\mathbb C)\cong
 \begin{cases}
 \mathcal O(\mathbb C),&(p,q)=(0,0),\\
 \mathcal O(\mathbb C),&(p,q)=(2,1),\\
 0,&p\in\{0,2\}\text{ and all other }q.
 \end{cases}}
$$

The second nonzero group is represented in [Čech cohomology](../../../../../../cech-cohomology.md) by $a(w)z^{-1}dz\wedge dw$. This explicit residue description is the [Dolbeault cohomology of the projective line times the affine line](../../../../../../dolbeault-cohomology-of-the-projective-line-times-the-affine-line.md); it also identifies that group naturally with the holomorphic one-forms on the affine factor.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
