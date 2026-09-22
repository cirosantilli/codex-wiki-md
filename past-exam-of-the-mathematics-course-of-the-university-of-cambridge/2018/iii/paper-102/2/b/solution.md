<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a [simple root](../../../../../../simple-root.md) $\alpha_i$ and choose generators $e_i,f_i,h_i$ of the [sl2 subalgebra associated with a root](../../../../../../sl2-subalgebra-associated-with-a-root.md), with $h_i=\alpha_i^\vee$ and

$$
[h_i,e_i]=2e_i,\qquad[h_i,f_i]=-2f_i,\qquad[e_i,f_i]=h_i.
$$

The [highest-weight vector](../../../../../../highest-weight-vector.md) satisfies $e_i v=0$ and $h_i v=m_i v$, where $m_i=\langle\lambda,\alpha_i^\vee\rangle$. The [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md) already implies that $m_i$ is a nonnegative integer. One can also see the necessary integrality directly from the [lowering operator](../../../../../../lowering-operator.md).

Indeed, $f_i^k v$, if nonzero, has $h_i$ eigenvalue $m_i-2k$. These distinct [eigenvalues](../../../../../../eigenvalue.md) cannot occur indefinitely in a finite-dimensional space, so there is a largest $r\geq0$ with $f_i^r v\ne0$. The [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) relations imply, by induction on $k$,

$$
e_i f_i^k v=k(m_i-k+1)f_i^{k-1}v.
$$

For $k=r+1$ the left side is zero, hence $(r+1)(m_i-r)f_i^r v=0$. Thus $m_i=r\in\mathbb Z_{\geq0}$. Since this holds for every [simple root](../../../../../../simple-root.md),

$$
\boxed{\lambda\text{ is a dominant integral weight}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
