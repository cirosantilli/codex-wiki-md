<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a [Feynman parameter](../../../../../../feynman-parameter.md) with $A=k^2+m^2$ and $B=(p-k)^2$. Then

$$
xA+(1-x)B=[k-(1-x)p]^2+\Delta,
\qquad
\Delta=xm^2+x(1-x)p^2.
$$

The identities for [gamma matrices](../../../../../../gamma-matrices.md) give

$$
\gamma^\mu(-i\not k+m)\gamma_\mu
=i(d-2)\not k+dm.
$$

After the shift $\ell=k-(1-x)p$, the term odd in $\ell$ integrates to zero. The rotationally symmetric loop integral is

$$
\int\frac{d^d\ell}{(2\pi)^d}\frac1{(\ell^2+\Delta)^2}
=\frac1{(4\pi)^{d/2}}\Gamma\left(\frac\epsilon2\right)
\Delta^{-\epsilon/2}.
$$

Consequently

$$
\boxed{\Sigma(\not p)=-\frac{e^2}{(4\pi)^{d/2}}
\Gamma\left(\frac\epsilon2\right)
\int_0^1dx\,
\frac{i(2-\epsilon)(1-x)\not p+(4-\epsilon)m}
{[xm^2+x(1-x)p^2]^{\epsilon/2}}.}
$$

Thus

$$
\boxed{C=i(2-\epsilon)(1-x),\qquad F=4-\epsilon,
\qquad\Delta=xm^2+x(1-x)p^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
