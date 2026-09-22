<h1 id="7b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We prove [independence of eigenvectors for distinct eigenvalues](../../../../../../independence-of-eigenvectors-for-distinct-eigenvalues.md) by induction on the number of vectors. A single [eigenvector](../../../../../../eigenvector.md) is nonzero and hence independent. Suppose the first $d-1$ are independent, and let $\sum_{j=1}^d c_jv_j=0$. Applying $A-\lambda_dI$ gives

$$
\sum_{j=1}^{d-1}c_j(\lambda_j-\lambda_d)v_j=0.
$$

By the induction hypothesis every coefficient in this shorter relation vanishes. The [eigenvalues](../../../../../../eigenvalue.md) are distinct, so $c_j=0$ for $j<d$. The original relation becomes $c_dv_d=0$, and $v_d\ne0$ gives $c_d=0$. Thus **the entire family of [eigenvectors](../../../../../../eigenvector.md) is [linearly independent](../../../../../../linear-independence.md)**. The argument works over either the real or complex field.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
