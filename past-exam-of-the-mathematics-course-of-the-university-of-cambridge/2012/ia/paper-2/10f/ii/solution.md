<h1 id="10f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The independent [uniform distributions](../../../../../../continuous-uniform-distribution.md) give a constant [joint probability density](../../../../../../joint-probability-density.md) $1$ on the unit square. For $0<x<1$, integrate over $x<u<v^2$:

$$
P(V^2>U>x)=\int_x^1\int_{\sqrt u}^1dv\,du=\int_x^1(1-\sqrt u)du
=\boxed{\frac13-x+\frac23x^{3/2}}.
$$

For the [random quadratic with uniform coefficients](../../../../../../random-quadratic-with-uniform-coefficients.md), real roots require its [discriminant](../../../../../../discriminant.md) to be nonnegative, equivalently $U\leq V^2$. The boundary has [probability](../../../../../../probability.md) zero, and the area under this parabola is

$$
\boxed{P(\text{real roots})=\int_0^1v^2dv=\frac13}.
$$

On that event the roots are $-V\pm\sqrt{V^2-U}$, both nonpositive. Bounding both absolute values by one therefore amounts to bounding the more negative root:

$$
V+\sqrt{V^2-U}\leq1.
$$

Since $0\leq V\leq1$, squaring the inequality is legitimate and gives $U\geq2V-1$. The admissible unit-square region is $\max(0,2v-1)\leq u\leq v^2$. Its [probability](../../../../../../probability.md) is

$$
\int_0^{1/2}v^2dv+\int_{1/2}^1(v^2-2v+1)dv=\frac1{24}+\frac1{24}=\frac1{12}.
$$

Dividing by the real-root [probability](../../../../../../probability.md) gives the requested [conditional probability](../../../../../../conditional-probability.md):

$$
\boxed{P(|R_1|\leq1,|R_2|\leq1\mid\text{real roots})=\frac14}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
