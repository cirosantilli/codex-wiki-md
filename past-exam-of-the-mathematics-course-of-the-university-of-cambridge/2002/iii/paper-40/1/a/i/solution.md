<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $H=\int_{\mathbb R}h(x)\,dx$, and assume $0<H<\infty$; a [uniform distribution](../../../../../../../continuous-uniform-distribution.md) on the region requires positive area. Set $x=V/U$, $s=U$, so the inverse transformation is $U=s$, $V=sx$. Its [Jacobian determinant](../../../../../../../jacobian-determinant.md) has absolute value $s$ for $s>0$. The region becomes $x\in\mathbb R$, $0<s\leq\sqrt{h(x)}$, and its area is

$$
|C_h|=\int_{\mathbb R}\int_0^{\sqrt{h(x)}}s\,ds\,dx=\frac H2.
$$

The original [joint probability density function](../../../../../../../joint-probability-density.md) is therefore $2/H$ on $C_h$. The [change of variables](../../../../../../../change-of-variables-formula.md) formula gives

$$
\boxed{f_{X_1,X_2}(x,s)=\frac{2s}{H}\,\mathbf1_{\{0<s\leq\sqrt{h(x)}\}}.}
$$

The boundary $U=0$ has [probability](../../../../../../../probability.md) zero, so division by $U$ causes no ambiguity for the resulting [random variable](../../../../../../../random-variable-split.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
