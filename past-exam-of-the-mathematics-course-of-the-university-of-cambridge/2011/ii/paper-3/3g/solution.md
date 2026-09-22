<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

A [Kleinian group](../../../../../kleinian-group.md) is a [discrete subgroup](../../../../../discrete-subgroup.md) of $\operatorname{PSL}_2(\mathbb C)$, acting by [Möbius transformations](../../../../../mobius-transformation.md) on the [Riemann sphere](../../../../../riemann-sphere.md), equivalently by orientation-preserving [isometries](../../../../../isometry.md) of [hyperbolic space](../../../../../hyperbolic-space.md) $\mathbb H^3$.

Consider the classes of

$$
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},\qquad B=\begin{pmatrix}1&0\\2&1\end{pmatrix}.
$$

They generate a discrete subgroup because their matrix representatives have integer entries: a sequence of such matrices converging to $I$ or $-I$ is eventually constant. On the real projective line set $X=\{x:|x|>1\}\cup\{\infty\}$ and $Y=\{x:|x|<1\}$. For every nonzero integer $m$,

$$
A^m(x)=x+2m,\qquad B^m(x)=\frac{x}{2mx+1},\qquad A^m(Y)\subset X,\quad B^m(X)\subset Y.
$$

The last inclusion follows from $|2mx+1|\geq2|x|-1>|x|$ when $|x|>1$; also $B^m(\infty)=1/(2m)\in Y$. The [ping-pong lemma](../../../../../ping-pong-lemma.md) therefore says that the subgroup is the [free product](../../../../../free-product.md) $\langle A\rangle*\langle B\rangle$. Both generators have infinite order, so

$$
\boxed{\langle A,B\rangle\cong\mathbb Z*\mathbb Z,}
$$

a [free group](../../../../../free-group.md) on two generators. The ping-pong inclusions ensure that no nonempty reduced word can act as the identity, which is the essential freeness argument.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
