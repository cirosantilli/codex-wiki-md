<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the invariants by the [characteristic polynomial](../../../../characteristic-polynomial.md)

$$
\det(tI-B)=t^3-I_Bt^2+II_Bt-III_B.
$$

Because $B=FF^T$ has positive [eigenvalues](../../../../eigenvalue.md) $\lambda_j^2$, its invariants are the [elementary symmetric functions](../../../../elementary-symmetric-polynomial.md) in those [eigenvalues](../../../../eigenvalue.md):

$$
I_B=\lambda_1^2+\lambda_2^2+\lambda_3^2,\qquad
II_B=\lambda_1^2\lambda_2^2+\lambda_1^2\lambda_3^2+\lambda_2^2\lambda_3^2,\qquad
III_B=\lambda_1^2\lambda_2^2\lambda_3^2.
$$

The [Frobenius norm](../../../../frobenius-norm.md) gives $|F|^2=\operatorname{tr}(F^TF)=\sum_j\lambda_j^2$. Write $J=\det F>0$. Since $\operatorname{cof}F=JF^{-T}$, its [singular values](../../../../singular-value.md) are $J/\lambda_j$, so

$$
|\operatorname{cof}F|^2=J^2\sum_j\lambda_j^{-2}
=\lambda_2^2\lambda_3^2+\lambda_1^2\lambda_3^2+\lambda_1^2\lambda_2^2.
$$

Finally $\det B=\det F\det F^T=J^2$. Therefore

$$
\boxed{I_B=|F|^2,\qquad II_B=|\operatorname{cof}F|^2,\qquad III_B=(\det F)^2.}
$$

These identities also give $I_B=\operatorname{tr}B$ and $II_B=((\operatorname{tr}B)^2-\operatorname{tr}(B^2))/2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
