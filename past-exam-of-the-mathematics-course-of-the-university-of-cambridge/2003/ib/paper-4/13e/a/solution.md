<h1 id="13e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a closed piecewise smooth [contour](../../../../../../complex-integration-contour.md) $\Gamma$ in a domain, null-homologous there and avoiding the [poles](../../../../../../pole.md) of a [meromorphic function](../../../../../../meromorphic-function.md) $F$, the [residue theorem](../../../../../../residue-theorem.md) is

$$
\int_\Gamma F(z)\,dz=2\pi i\sum_a n(\Gamma,a)\operatorname{Res}(F;a),
$$

where $n(\Gamma,a)=(2\pi i)^{-1}\int_\Gamma dz/(z-a)$ is the [winding number](../../../../../../winding-number.md) and the sum runs over enclosed [poles](../../../../../../pole.md) with their indices. Suppose now $f$ is meromorphic and has neither zeros nor [poles](../../../../../../pole.md) on $\Gamma$. At a zero or [pole](../../../../../../pole.md) $a$, write $f(z)=(z-a)^m h(z)$ with $h$ [holomorphic](../../../../../../complex-differentiability-at-a-point.md) and nonzero, where $m>0$ for a zero and $m<0$ for a [pole](../../../../../../pole.md). Then

$$
\frac{f'}f=\frac m{z-a}+\frac{h'}h,
$$

so its [residue](../../../../../../residue.md) is $m$. Substituting into the [residue theorem](../../../../../../residue-theorem.md) and changing variables along the [image](../../../../../../image-of-a-function.md) [contour](../../../../../../complex-integration-contour.md) gives the [argument principle](../../../../../../argument-principle.md):

$$
\boxed{n(f\circ\Gamma,0)=\sum_{f(a)=0}m_a n(\Gamma,a)
-\sum_{a\text{ pole}}p_a n(\Gamma,a)}.
$$

For a positively oriented simple boundary, this is the number of zeros minus [poles](../../../../../../pole.md) inside, counted with [multiplicity](../../../../../../multiplicity-mathematics.md). The winding-number form also applies to self-intersecting [image](../../../../../../image-of-a-function.md) paths.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13E](../../13e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
