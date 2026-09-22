<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fixed-point equation for $u$ factors as

$$
u\bigl[(1+u^2)^2-4u\bigr]=u(u-1)(u^3+u^2+3u-1)=0.
$$

The cubic derivative is $3u^2+2u+3>0$ for every real $u$; its values at zero and one have opposite signs. Thus the possible first coordinates in the stated domain are exactly $u=0,u_*,1$.

For finite $v$, the second fixed-point equation is $v[v^3-(1+u^2)^2]=0$. The [renormalization-group fixed points](../../../../../../renormalization-group-fixed-point.md) are consequently

$$
\boxed{(a,0),\quad \bigl(a,(1+a^2)^{2/3}\bigr),\quad (a,\infty),\qquad a\in\{0,u_*,1\}.}
$$

There are six finite points and three boundary points at infinity. Infinity is interpreted in a compactified domain, not as an ordinary real number. The [reciprocal coordinate at infinite coupling](../../../../../../reciprocal-coordinate-at-infinite-coupling.md) $w=1/v$ transforms as $w'=(1+u^2)^2w^4$, making $w=0$ a well-defined boundary fixed point.

At any finite fixed point $(\tilde u,\tilde v)$, let $\delta u=u-\tilde u$, $\delta v=v-\tilde v$. The [Jacobian matrix](../../../../../../jacobian-matrix.md) linearization is

$$
\begin{pmatrix}\delta u'\\\delta v'\end{pmatrix}=\begin{pmatrix}\dfrac{8\tilde u(1-\tilde u^2)}{(1+\tilde u^2)^3}&0\\[5pt]-\dfrac{4\tilde u\tilde v^4}{(1+\tilde u^2)^3}&\dfrac{4\tilde v^3}{(1+\tilde u^2)^2}\end{pmatrix}\begin{pmatrix}\delta u\\\delta v\end{pmatrix}+O(\|(\delta u,\delta v)\|^2).
$$

The only point with both coordinates strictly interior is $\tilde u=u_*$, $\tilde v=(1+u_*^2)^{2/3}$. Using its fixed-point relations, the [matrix](../../../../../../matrix.md) becomes

$$
M_* =\begin{pmatrix}\rho&0\\c&4\end{pmatrix},\qquad \rho=\frac{2(1-u_*^2)}{1+u_*^2},\qquad c=-\frac{4u_*\tilde v}{1+u_*^2}.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are $\rho$ and $4$. In particular, $u_*<1/\sqrt3$ because the increasing cubic is already positive there, so $\rho>1$ (numerically about $1.68$). The corresponding [eigenvectors](../../../../../../eigenvector.md) can be chosen as $(1,c/(\rho-4))^T$ and $(0,1)^T$. Both discrete multipliers exceed one, hence

$$
\boxed{\text{the unique interior fixed point is repulsive in both directions}.}
$$

Both perturbations are [relevant directions of a fixed point](../../../../../../relevant-direction-of-a-fixed-point.md) under repeated coarse-graining, rather than one stable and one unstable direction. A length-rescaling factor was not specified, so these multipliers should not be assigned numerical critical scaling exponents without additional information. At $a=0,1$, the $u$ multiplier is zero; at $v=0$ or $w=0$ the other multiplier is also zero. Thus the four corner points attract locally within the domain, the two positive finite boundary points at $a=0,1$ are saddles, and the points $(u_*,0),(u_*,\infty)$ have one repulsive and one attractive direction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
