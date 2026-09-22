<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an integral [Minimal Weierstrass equation](../../../../../../minimal-weierstrass-equation.md) over $\mathbb Z_p$. Let $E_0(\mathbb Q_p)$ be the points with nonsingular reduction, and let $E_1(\mathbb Q_p)$ be those reducing to $O$. This distinction matters at [bad reduction of an elliptic curve](../../../../../../bad-reduction-of-an-elliptic-curve.md): the whole singular reduced cubic is not a group. The smooth locus is a group under the induced [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md), and [Hensel's lemma](../../../../../../hensel-s-lemma.md) lifts each of its [rational points](../../../../../../rational-point.md), giving

$$
0\longrightarrow E_1(\mathbb Q_p)\longrightarrow E_0(\mathbb Q_p)\longrightarrow\widetilde E_{\mathrm{ns}}(\mathbb F_p)\longrightarrow0.
$$

The [formal kernel of a minimal Weierstrass equation](../../../../../../formal-kernel-of-a-minimal-weierstrass-equation.md) identifies $E_1(\mathbb Q_p)$ with $p\mathbb Z_p$ equipped with $F$. Indeed, the integral series $w(t)$ converges there, and $x=t/w(t)$, $y=-1/w(t)$ give the unique point for each nonzero parameter. If $v_p(t)=r>0$, then $v_p(x)=-2r$ and $v_p(y)=-3r$; the parameter zero gives $O$. Conversely a point reducing to $O$ has these local coordinates of positive [valuation](../../../../../../valuation.md), so is recovered by the series.

Define $E_m$ for $m\ge1$ by $t\in p^m\mathbb Z_p$. The linear part of the [formal group law](../../../../../../formal-group-law.md) is addition, and the higher terms have degree at least two. Hence the [filtration of elliptic-curve points over a local field](../../../../../../filtration-of-elliptic-curve-points-over-a-local-field.md) has

$$
E_m/E_{m+1}\cong(p^m\mathbb Z_p/p^{m+1}\mathbb Z_p,+)\cong(\mathbb F_p,+).
$$

At [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), $E_0=E$ and $E/E_1\cong\widetilde E(\mathbb F_p)$. At [bad reduction](../../../../../../bad-reduction-of-an-elliptic-curve.md), there is also the finite quotient $E/E_0$: $E(\mathbb Q_p)$ is a [compact group](../../../../../../compact-group.md) because the curve is projective, and $E_0$ is an open subgroup, so its [index of a subgroup](../../../../../../index-of-a-subgroup.md) is finite. Together these quotients and the formal filtration describe the group, including the extra components at bad primes.

The [formal logarithm](../../../../../../formal-logarithm.md) makes the deepest part explicit. Write $L(T)=T+\sum_{n\ge2}c_nT^n$. Since its derivative is the integral [invariant differential of a formal group law](../../../../../../invariant-differential-of-a-formal-group-law.md), $nc_n\in\mathbb Z_p$. Consequently

$$
v_p(c_nt^n)\ge n\,v_p(t)-v_p(n).
$$

The inequality $v_p(n)\le(n-1)/(p-1)$ shows that for an integer $m>1/(p-1)$ every nonlinear term on $p^m\mathbb Z_p$ has strictly higher [valuation](../../../../../../valuation.md) than the linear term. After scaling, $L$ is the identity plus a strictly contracting series; solving $L(t)=u$ by successive correction gives its inverse [formal group exponential](../../../../../../formal-group-exponential.md). Thus the [deep logarithm subgroup of a formal group](../../../../../../deep-logarithm-subgroup-of-a-formal-group.md) gives

$$
\boxed{E_m(\mathbb Q_p)\cong(p^m\mathbb Z_p,+)\quad\text{when }m>1/(p-1).}
$$

One may take $m=1$ for odd $p$ and $m=2$ for $p=2$. In particular, $E(\mathbb Q_p)$ contains an open subgroup isomorphic to the additive [p-adic integers](../../../../../../p-adic-integer.md), and the remaining information is in finite quotients and their group extensions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
