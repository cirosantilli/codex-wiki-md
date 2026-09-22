<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Bed and sidewall stress, turbulent mixing at the interface, wave radiation and [hydraulic jumps](../../../../../../hydraulic-jump.md) convert or remove mechanical energy. In the specified local head-loss model, differentiate $B=u^2/2+g'h$ while keeping $Q=bhu$ constant:

$$
B'=g'(1-F^2)h'-u^2\frac{b'}b.
$$

At a regular [hydraulic control](../../../../../../hydraulic-control.md) the coefficient of $h'$ vanishes. Therefore $B'=-\alpha$ requires

$$
\boxed{\alpha=u_c^2\frac{b'(x_c)}{b(x_c)}
=g'h_c\frac{2x_c}{L^2+x_c^2},\qquad
h_c=\left[\frac{Q^2}{g'b(x_c)^2}\right]^{1/3}.}
$$

Thus the control moves to the widening downstream side, $x_c>0$. This is the exact local compatibility condition; it is the [head-loss correction to hydraulic control](../../../../../../head-loss-correction-to-hydraulic-control.md) with loss expressed as Bernoulli potential per unit length.

For a small loss and a control remaining near the throat, use the lossless depth $h_c=2H/3+O(\alpha)$ and $b'/b=2x_c/L^2+O(x_c^3/L^4)$. The leading displacement is

$$
\boxed{x_c\simeq\frac{\alpha L^2}{2g'h_c}\simeq\frac{3\alpha L^2}{4g'H}.}
$$

For a finite loss, the local derivative alone does not specify the accumulated loss from the far-upstream reservoir, so it does not fix a unique revised discharge or numerical control depth. Given $Q$, the exact condition can instead be solved implicitly for $x_c$; if the inviscid discharge is imposed, it becomes $\alpha=(4g'H/3L)(x_c/L)[1+(x_c/L)^2]^{-5/3}$. The small-displacement root is the one continuous from the throat. This distinction avoids treating the original upstream energy as unchanged after an unspecified finite upstream loss.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
