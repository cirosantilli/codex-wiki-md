<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Choose one free, massless [complex scalar field](../../../../../../complex-scalar-field.md) with unit charge magnitude and bosonic statistics, minimally coupled to $A$. To fix the sign, use the conventional [gauge covariant derivative](../../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu-iqA_\mu$ and take $q=-1$, so $D_\mu=\partial_\mu+iA_\mu$ and $\varphi\mapsto e^{-i\alpha}\varphi$. Its antiparticle has charge $+1$. The matter data are

$$
\boxed{m_\varphi=0,\qquad q=-1\ \text{in }D=\partial-iqA,\qquad\text{spin }0,\qquad\text{bosonic statistics}.}
$$

There is no scalar self-interaction. For real fields before formal continuation, its action is $S_\varphi=\int(D_\mu\varphi)^*(D_\mu\varphi)\,d^4x=\int\bar\varphi(-D^2)\varphi\,d^4x$, by [integration by parts](../../../../../../integration-by-parts.md). The [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) gives the inverse [functional determinant](../../../../../../functional-determinant.md) and thus $\Gamma_\varphi=+\operatorname{Tr}'\log(-D^2)$, up to normalization.

The key operator identity is

$$
D^2=\partial^2+2iA\cdot\partial+i\partial\cdot A-A^2=M_A+iF[A].
$$

On the formal complex gauge slice, $-D^2=-M_A=\mathcal O_A$. With matching regulators and omitted zero modes, this gives [ghost-scalar determinant cancellation in a complex quadratic gauge](../../../../../../ghost-scalar-determinant-cancellation-in-a-complex-quadratic-gauge.md), leaving the [Maxwell action](../../../../../../maxwell-action.md) as the background functional:

$$
\boxed{\Gamma_\varphi[A]+\Gamma_{\mathrm{gh}}[A]=0,\qquad S_{\mathrm{eff}}[A]=S_{\mathrm{Maxwell}}[A]=\frac14\int F_{\mu\nu}F_{\mu\nu}\,d^4x,}
$$

where gauge-fixing terms and field-independent constants are understood separately. For a fixed background the [complex scalar field](../../../../../../complex-scalar-field.md) and [Faddeev-Popov ghost field](../../../../../../faddeev-popov-ghost.md) integrals are Gaussian, so this determinant cancellation is exact within the formal construction. It is a cancellation of closed bosonic matter loops against [ghost loops](../../../../../../ghost-loop.md) in that background functional. It does not prove that physical [scalar quantum electrodynamics](../../../../../../scalar-electrodynamics.md) has no radiative corrections: the printed real Euclidean gauge slice contains only $A=0$ and misses every nonzero-curvature orbit. On that literal slice the equality is trivial; a nontrivial version requires the additional complex-contour interpretation.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
