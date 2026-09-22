<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Define on $H$ the [bilinear form](../../../../../../../bilinear-form.md)

$$
a(u,v)=\int_0^1u'v'+\int_0^1\frac{uv}{x^2}-\int_0^1u'v
$$

and the linear functional

$$
\ell(v)=\int_0^1\frac fx\frac vx.
$$

The [Hardy inequality on an interval](../../../../../../../hardy-inequality-on-an-interval.md), [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md), and the one-sided [Poincaré inequality](../../../../../../../poincare-inequality.md) show that $a$ is a [bounded bilinear form](../../../../../../../bounded-bilinear-form.md) and that

$$
|\ell(v)|\leq2\|f/x\|_2\|v'\|_2\leq C\|f/x\|_2\|v\|_{H^1}.
$$

For $v\in H$, $v(x)=\int_0^xv'(t)\,dt$, so [Cauchy--Schwarz](../../../../../../../cauchy-schwarz-inequality.md) and [Fubini's theorem](../../../../../../../fubini-s-theorem.md) give

$$
\|v\|_2^2\leq\frac12\|v'\|_2^2.
$$

Hence

$$
\begin{aligned}
a(v,v)
&=\|v'\|_2^2+\|v/x\|_2^2-\int_0^1v'v\\
&\geq\left(1-\frac1{\sqrt2}\right)\|v'\|_2^2\\
&\geq c\|v\|_{H^1}^2.
\end{aligned}
$$

Thus $a$ is a [coercive bilinear form](../../../../../../../coercive-bilinear-form.md). The [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md) supplies a unique $u\in H$ satisfying $a(u,v)=\ell(v)$ for every $v\in H$. This is precisely the unique weak solution described by the [weak boundary value problem with an inverse-square potential](../../../../../../../weak-boundary-value-problem-with-an-inverse-square-potential.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
