<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Using the [singular value system](../../../../../../../singular-system-of-a-compact-operator.md) with $Au_j=\sigma_jv_j$ and $A^*v_j=\sigma_ju_j$, the formal minimum-norm inverse is

$$
x=\sum_j\frac{(y,v_j)}{\sigma_j}u_j.
$$

It defines an element of the unknown [Hilbert space](../../../../../../../hilbert-space-split.md) only if $\sum_j|(y,v_j)|^2/\sigma_j^2<\infty$, the [Picard criterion](../../../../../../../picard-criterion.md). A null-space component is undetermined by the data.

Adding an error along a single [left singular vector](../../../../../../../left-singular-vector.md) changes precisely one coefficient:

$$
x_\delta-x=\frac\delta{\sigma_j}u_j,\qquad
\boxed{\|x_\delta-x\|=\frac\delta{\sigma_j}.}
$$

Although this perturbation has data [norm](../../../../../../../norm.md) $\delta$, its amplification factor is $1/\sigma_j$. If $\sigma_j\to0$, these factors are unbounded. More explicitly choose $y^{(j)}=\sigma_jv_j$, tending to zero, while the minimum-norm inverse is $u_j$, of [norm](../../../../../../../norm.md) one. Thus the inverse is discontinuous at zero. It may also fail to exist for data outside its nonclosed range, so merely minimizing a residual does not guarantee that the formal inverse exists. This is **[ill-posedness](../../../../../../../ill-posed-problem.md) by unbounded small-singular-value amplification**, not a claim that every finite-dimensional or bounded forward map has an unstable inverse.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 70](../../../../paper-70-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
