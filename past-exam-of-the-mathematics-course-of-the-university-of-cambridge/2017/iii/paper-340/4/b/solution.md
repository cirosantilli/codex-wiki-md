<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [indicator function](../../../../../../indicator-function.md) $u(x_1,x_2)=\chi_{\{x_1>1/2\}}$ inside $(0,1)^2$. For a compactly supported test [vector field](../../../../../../vector-field.md), integration in $x_1$ and then $x_2$ gives

$$
\int_\Omega u\,\operatorname{div}\xi\,dx=-\int_0^1\xi_1(1/2,x_2)\,dx_2.
$$

The vertical [derivative](../../../../../../derivative.md) term integrates to zero. The absolute pairing is at most one, and test [vector fields](../../../../../../vector-field.md) with $\xi_1=-1$ along all but arbitrarily short endpoint pieces approach one. Thus $|Du|(\Omega)=1$. More explicitly, the [distributional derivative](../../../../../../distributional-derivative.md) is $Du=e_1\mathcal H^1\!\restriction\{(1/2,x_2):0<x_2<1\}$, where $\mathcal H^1$ is [Hausdorff measure](../../../../../../hausdorff-measure.md) along the segment. Also $\|u\|_1=1/2$.

A [Sobolev space](../../../../../../sobolev-space-split.md) [function](../../../../../../function-split.md) in $W^{1,1}(\Omega)$ has each weak [derivative](../../../../../../derivative.md) represented by an $L^1$ density with respect to planar [Lebesgue measure](../../../../../../lebesgue-measure.md). The nonzero segment measure here is singular with respect to that measure, so this requirement fails. Equivalently, the [Sobolev fundamental theorem of calculus on lines](../../../../../../sobolev-fundamental-theorem-of-calculus-on-lines.md) would require an absolutely [continuous](../../../../../../continuous-function.md) representative on almost every horizontal slice, whereas each slice has a jump. Therefore

$$
\boxed{u\in BV(\Omega)\setminus W^{1,1}(\Omega),\qquad\|u\|_{BV}=\tfrac32.}
$$

This is the [bounded-variation step outside W11](../../../../../../bounded-variation-step-outside-w11.md) example.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
