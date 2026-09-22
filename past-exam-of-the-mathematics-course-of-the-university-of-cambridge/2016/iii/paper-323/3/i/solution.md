<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [absolute value of an operator](../../../../../../absolute-value-of-an-operator.md), [trace norm](../../../../../../trace-norm.md), and [operator norm](../../../../../../operator-norm.md) are respectively

$$
|L|=\sqrt{L^\dagger L},\qquad
\|L\|_1=\operatorname{Tr}|L|,\qquad
\|L\|_{\rm op}=\sup_{\|v\|=1}\|Lv\|.
$$

The [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md) makes $|L|$ well defined. Its [eigenvalues](../../../../../../eigenvalue.md) $s_j\geq0$ are the [singular values](../../../../../../singular-value.md) of $L$, so $\|L\|_1=\sum_js_j$ and $\|L\|_{\rm op}=\max_js_j$.

Use the [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) $L=U|L|$, with the given [unitary operator](../../../../../../unitary-operator.md) $U$. In an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) $e_j$ for $|L|$,

$$
\operatorname{Tr}(ZL)=\sum_js_j\langle e_j|ZU|e_j\rangle.
$$

The [operator norm](../../../../../../operator-norm.md) assumption and unitarity imply $|\langle e_j|ZU|e_j\rangle|\leq\|Z\|_{\rm op}\leq1$. The [triangle inequality](../../../../../../triangle-inequality.md) therefore yields **the required trace estimate**:

$$
\boxed{|\operatorname{Tr}(ZL)|\leq\sum_js_j=\|L\|_1.}
$$

Choosing $Z=U^\dagger$ attains equality, which also gives the finite-dimensional [trace duality](../../../../../../trace-duality.md) formula $\|L\|_1=\max_{\|Z\|_{\rm op}\leq1}|\operatorname{Tr}(ZL)|$. A singular $L$ causes no difficulty: in a finite-dimensional square space the polar factor can be extended to a [unitary operator](../../../../../../unitary-operator.md) on the complementary subspaces.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
