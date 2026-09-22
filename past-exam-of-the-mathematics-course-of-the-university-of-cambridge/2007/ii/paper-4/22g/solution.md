<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

For a bounded operator on a complex [Banach space](../../../../../banach-space-split.md), the [resolvent set](../../../../../resolvent-set-of-an-operator.md) is $\rho(T)=\{\lambda:\lambda I-T\text{ is bijective with bounded inverse}\}$, and the [resolvent operator](../../../../../resolvent-of-an-operator.md) is $R_T(\lambda)=(\lambda I-T)^{-1}$. The [spectrum](../../../../../spectrum-functional-analysis.md) is its complement $\sigma(T)=\mathbb C\setminus\rho(T)$; the [point spectrum](../../../../../point-spectrum.md) consists of $\lambda$ with $\ker(\lambda I-T)\ne0$. For a real Banach space these definitions use its complexification.

If $|\lambda|>\|T\|$, the norm-convergent [Neumann series](../../../../../neumann-series.md) gives $R_T(\lambda)=\lambda^{-1}\sum_{n\geq0}(T/\lambda)^n$, so the spectrum is bounded. If $\lambda_0\in\rho(T)$, factor

$$
\lambda I-T=(\lambda_0I-T)[I+(\lambda-\lambda_0)R_T(\lambda_0)].
$$

The second factor is invertible by a Neumann series whenever $|\lambda-\lambda_0|\|R_T(\lambda_0)\|<1$. Thus the resolvent set is open and **the spectrum is closed and bounded**.

The point spectrum need not be closed. On $\ell^2$, define $Te_n=e_n/n$. Every $1/n$ is an [eigenvalue](../../../../../eigenvalue.md), but zero is not: $Tx=0$ forces every coordinate of $x$ to vanish. No other [eigenvalues](../../../../../eigenvalue.md) occur, so $\sigma_p(T)=\{1/n:n\geq1\}$ is not closed.

Finally, if $T$ is self-adjoint and $Tv=\lambda v$, $v\ne0$, then $\langle Tv,v\rangle$ is real and equals $\lambda\|v\|^2$ under the convention linear in the first argument. Therefore **every [eigenvalue](../../../../../eigenvalue.md) of a self-adjoint operator is real**.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
