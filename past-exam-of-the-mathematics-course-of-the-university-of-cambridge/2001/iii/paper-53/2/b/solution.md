<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The normalization fixes the [critical point](../../../../../../critical-point.md) at zero and its image at one. It removes arbitrary height and spatial scales, so successive renormalized return maps can be compared in one function space rather than drifting through rescaled copies of the same dynamics. The second iterate near the [critical point](../../../../../../critical-point.md) has a minimum; a negative rescaling reverses it back to a maximum.

Because $f(0)=1$, the [period-doubling renormalization operator](../../../../../../period-doubling-renormalization-operator.md) satisfies

$$
\mathcal T(f)(0)=a^{-1}f(f(0))=a^{-1}f(1).
$$

Preservation of normalization therefore forces

$$
\boxed{a=a(f)=f(1)=f^2(0),\qquad
\mathcal T(f)(x)=\frac{f(f(f(1)x))}{f(1)}.}
$$

The scale is a functional of $f$, not an independently adjustable constant. In the renormalizable regime it lies in $(-1,0)$. If $h(x)=ax$, then $\mathcal T(f)=h^{-1}\circ f^2\circ h$ on the central restrictive interval. Thus [topological conjugacy](../../../../../../topological-conjugacy.md) relates one iteration of the renormalized map to two iterations of the original map, and the new critical value is again one. For $f_\mu$, $a=1-\mu$, so this regime starts beyond the superstable two-cycle at $\mu=1$.

Normalization alone does not make every normalized [unimodal map](../../../../../../unimodal-interval-map.md) renormalizable: the central interval and its image must form the appropriate period-two restrictive pair, so that the rescaled second iterate is again an even [unimodal map](../../../../../../unimodal-interval-map.md) into $[-1,1]$. The operator is considered on the neighbourhood where these additional conditions hold.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
