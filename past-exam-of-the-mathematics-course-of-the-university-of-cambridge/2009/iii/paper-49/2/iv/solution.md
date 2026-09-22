<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Since $|\Phi|\to1$, the [Higgs field](../../../../../../higgs-field.md) is nonzero outside a sufficiently large disk. On a large positively oriented circle write $\Phi=\rho e^{i\chi}$ locally, where $\rho>0$. Its normalized phase is a map from the circle to the unit circle. The phase need not be a globally single-valued real function, but its total change is $2\pi N$ for an integer [winding number](../../../../../../winding-number.md) $N$. This integer is the same on all sufficiently large circles because the intervening annulus contains no zeros.

The [gauge covariant derivative](../../../../../../gauge-covariant-derivative.md) gives

$$
D\Phi=e^{i\chi}[d\rho+i\rho(d\chi-A)],\qquad
A=d\chi-\frac{\operatorname{Im}(\overline\Phi D\Phi)}{\rho^2}.
$$

Integrate around the circle. The assumed rapid decay makes the integral of the second term tend to zero. For example, uniform $|D\Phi|=o(R^{-1})$ and $\rho\to1$ on radius-$R$ circles suffice. Hence

$$
\lim_{R\to\infty}\oint_{|x|=R}A_jdx^j=2\pi N.
$$

By [Stokes theorem](../../../../../../stokes-theorem.md), $\oint_{|x|=R}A=\int_{|x|\leq R}B\,d^2x$. Integrability of $B$ allows the limit, giving the [magnetic flux quantization of an Abelian Higgs vortex](../../../../../../magnetic-flux-quantization-of-an-abelian-higgs-vortex.md):

$$
\boxed{\int_{\mathbb R^2}B\,d^2x=2\pi N.}
$$

The [topological charge](../../../../../../topological-charge.md) $N$ is the degree of $\Phi/|\Phi|$ at infinity, counting net phase winding around the cores. For isolated zeros it is the sum of their signed local winding numbers. In the positive [Abelian Higgs vortex](../../../../../../nielsen-olesen-vortex.md) construction, each core of multiplicity $m_a$ has local phase $m_a\arg(z-z_a)$, so

$$
\boxed{N=\sum_am_a,}
$$

the number of vortices counted with multiplicity. Antivortices have the opposite sign. The integer is invariant under smooth gauge transformations defined throughout the disk, whose boundary winding is zero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
