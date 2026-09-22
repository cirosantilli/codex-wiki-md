<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $Y_\pm=\overline y_\pm$, $y_0=y(0)$ and $d_\pm=y'(0\pm)$. In a common convergence strip, two integrations by parts on each half-line give

$$
\int_0^\infty y''e^{ikx}\,dx=-d_++iky_0-k^2Y_+,\qquad
\int_{-\infty}^0y''e^{ikx}\,dx=d_--iky_0-k^2Y_-.
$$

The [boundary](../../../../../boundary-of-a-set.md) terms at [infinity](../../../../../infinity.md) vanish by exponential decay; the [ordinary differential equations](../../../../../ordinary-differential-equation.md) also give decay of the required first [derivatives](../../../../../derivative.md). Substituting the two equations for $y''$ yields

$$
(a^2-k^2)Y_+=d_+-iky_0,\qquad(b^2-k^2)Y_-=-d_-+iky_0.
$$

[Continuity](../../../../../continuous-function.md) makes the $y_0$ terms cancel on addition, while the unit [derivative](../../../../../derivative.md) jump gives

$$
(a^2-k^2)Y_++(b^2-k^2)Y_-=1.
$$

Multiply by $-1/((k-a)(k+b))$ and factor the quadratics. Since $\operatorname{Im}(a+b)>0$, their sum is nonzero, and partial fractions give

$$
\boxed{\frac{k+a}{k+b}Y_++\frac{k-b}{k-a}Y_-=\frac1{a+b}\left(\frac1{k+b}-\frac1{k-a}\right).}
$$

This is the [Wiener-Hopf equation](../../../../../wiener-hopf-equation.md) for the two [half-line Fourier transforms](../../../../../half-line-fourier-transform.md). The plus and minus subscripts refer to support in physical space; their [holomorphic](../../../../../holomorphic-function-split.md) domains in transform space are determined next.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the applied complex variables course of the University of Oxford](../../../../split.md)
6. [Applied complex variables course of the University of Oxford](../../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
