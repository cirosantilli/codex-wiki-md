<h1 id="6/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $e=x-u^*$. If $u^*$ minimizes distance, then for every $v\in\mathcal U_n$ and every real $t$,

$$
\|e-tv\|^2=\|e\|^2-2t\operatorname{Re}(e,v)+t^2\|v\|^2\geq\|e\|^2.
$$

Both signs of arbitrarily small $t$ force $\operatorname{Re}(e,v)=0$. In a complex [inner product space](../../../../../../../inner-product-space.md), apply the same argument to $iv$ to obtain the imaginary part too. Conversely, if $e$ is orthogonal to the subspace, the [Pythagorean theorem for inner product spaces](../../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|x-u\|^2=\|x-u^*\|^2+\|u-u^*\|^2\qquad(u\in\mathcal U_n).
$$

Thus **[orthogonality](../../../../../../../orthogonal-vectors.md) characterizes the unique best approximation**:

$$
\boxed{u^*\text{ is best}\iff(x-u^*,v)=0\quad(v\in\mathcal U_n).}
$$

Finite dimension also guarantees existence by solving the invertible [Gram matrix](../../../../../../../gram-matrix.md) normal equations; completeness of the ambient [inner product space](../../../../../../../inner-product-space.md) is unnecessary.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [6](../../../6.md)
4. [Paper 69](../../../../paper-69-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
