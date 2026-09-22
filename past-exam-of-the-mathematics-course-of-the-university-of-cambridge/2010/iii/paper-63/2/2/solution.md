<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a real [Hilbert space](../../../../../../hilbert-space-split.md), differentiate along an arbitrary direction $w$:

$$
\left.\frac d{d\varepsilon}I(v+\varepsilon w)\right|_{\varepsilon=0}
=\langle Lv,w\rangle+\langle Lw,v\rangle-2\langle f,w\rangle
=2\langle Lv-f,w\rangle.
$$

The last equality uses the symmetry in the definition of a [positive definite symmetric operator](../../../../../../positive-definite-symmetric-operator.md). Vanishing of this [first variation](../../../../../../first-variation.md) for every $w$ is equivalent to $Lv=f$, giving

$$
\boxed{Lu=f\quad\text{as the Euler-Lagrange equation}.}
$$

If $u$ solves it, expand the functional about $u$ to find

$$
I(u+w)-I(u)=\langle Lw,w\rangle.
$$

This is strictly positive for nonzero $w$, so $u$ is the unique minimizer. Conversely a minimizer has zero [first variation](../../../../../../first-variation.md) and solves the equation. On a complex [Hilbert space](../../../../../../hilbert-space-split.md), use the real functional $\langle Lv,v\rangle-2\operatorname{Re}\langle f,v\rangle$ and real directional derivatives; varying $w$ and $iw$ yields the same result.

This proves the [quadratic variational principle for a symmetric positive operator](../../../../../../quadratic-variational-principle-for-a-symmetric-positive-operator.md), conditional on existence. Strict positivity in infinite dimension does not by itself guarantee a minimizer for every $f$: on $\ell^2$, the operator $(Lv)_j=v_j/j$ is strictly positive, but $f_j=1/j$ would require the non-square-summable solution $v_j=1$. A [coercive bilinear form](../../../../../../coercive-bilinear-form.md) supplies existence through the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) under its usual boundedness assumptions.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
