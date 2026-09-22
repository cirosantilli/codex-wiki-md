# Right singular vector

↑ **Parent:** [Singular value](singular-value.md)

A [right singular vector](right-singular-vector.md) $v_j$ is a [unit vector](unit-vector.md) in the input space satisfying $A^*Av_j=\sigma_j^2v_j$. For positive [singular values](singular-value.md), $Av_j=\sigma_j u_j$ determines the matching [left singular vector](left-singular-vector.md). In the [ellipse](ellipse.md) example, $Av_1=(5,0)^T$ is not parallel to $v_1$: a [right singular vector](right-singular-vector.md) need not be an [eigenvector](eigenvector.md) of $A$. Indeed, the [characteristic polynomial](characteristic-polynomial.md) of $A$ is $\lambda^2-(18/5)\lambda+5$, with [eigenvalues](eigenvalue.md) $(9\pm i\sqrt{44})/5$ and no real [eigenvectors](eigenvector.md). Nevertheless, its real [right singular vectors](right-singular-vector.md) give a complete [orthonormal basis](orthonormal-basis.md). [Eigenvectors](eigenvector.md) describe preserved directions; [right singular vectors](right-singular-vector.md) describe orthogonal input channels of stretching.[MIT 18.06SC, Singular value decomposition: paired bases](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/d273f75ee2552a5c3c35ccab37e5edce_MIT18_06SCF11_Ses3.5sum.pdf)

An arbitrary input mixes these channels. For $x=c_1v_1+c_2v_2$, [orthogonality](orthogonal-vectors.md) gives $\|Ax\|_2^2=25|c_1|^2+|c_2|^2$, while $\|x\|_2^2=|c_1|^2+|c_2|^2$. Equal contributions, $c_1=c_2=1/\sqrt2$, produce output [Euclidean norm](euclidean-norm.md) $\sqrt{13}$ from a [unit vector](unit-vector.md). Concentrating the entire input along $v_1$ produces the maximum $5$. This is why the [right singular vectors](right-singular-vector.md) give a direct reading of how any input will behave. For a [compact operator](compact-operator-split.md), the same definition describes the positive terms of its [singular value system](singular-system-of-a-compact-operator.md).

## ↑ Ancestors (7)

1. [Singular value](singular-value.md)
2. [Singular value decomposition](singular-value-decomposition.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Generalized singular vector](generalized-singular-vector.md)
- [Left singular vector](left-singular-vector.md)
- [Low-rank approximation](low-rank-approximation.md)
- [Optimal energy amplification of a linear system](optimal-energy-amplification-of-a-linear-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/4/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/4/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/4/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-331/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/18/d/solution.md)
- [Right singular vector](right-singular-vector.md)
- [Singular value](singular-value.md)
- [Singular value decomposition](singular-value-decomposition.md)
- [Spectral inverse theorem for the matrix-valued U2 quantity](spectral-inverse-theorem-for-the-matrix-valued-u2-quantity.md)
