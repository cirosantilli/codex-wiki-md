<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [power iteration](../../../../power-iteration.md) starts from $v_0\ne0$, normally scaled to unit [Euclidean norm](../../../../euclidean-norm.md), and repeats

$$
w_{k+1}=Av_k,\qquad
\boxed{v_{k+1}=\frac{w_{k+1}}{\|w_{k+1}\|_2}.}
$$

Normalization prevents the rapidly growing or decaying magnitudes of $A^kv_0$ from obscuring its direction. The iteration requires $w_{k+1}\ne0$.

Because $A$ is a [diagonalizable matrix](../../../../diagonalizable-matrix.md), choose an [eigenbasis](../../../../eigenbasis.md) $u_1,\ldots,u_n$, with corresponding [eigenvalues](../../../../eigenvalue.md) $\lambda_1=\lambda,\lambda_2,\ldots,\lambda_n$, and expand $v_0=\sum_jc_ju_j$. First suppose the [dominant eigenvalue](../../../../dominant-eigenvalue.md) is simple and $c_1\ne0$. Then

$$
A^kv_0
=c_1\lambda^k\left(u_1+\sum_{j=2}^n\frac{c_j}{c_1}
\left(\frac{\lambda_j}{\lambda}\right)^ku_j\right).
$$

For

$$
q=\max_{j\geq2}\left|\frac{\lambda_j}{\lambda}\right|<1,
$$

the sum in parentheses after $u_1$ is $O(q^k)$ in [Big O notation](../../../../big-o-notation.md). Consequently the [power iteration direction error](../../../../power-iteration-direction-error.md) is $O(q^k)$: the iterates approach the line spanned by $u_1$. For a real [matrix](../../../../matrix.md), a uniquely dominant [eigenvalue](../../../../eigenvalue.md) is real, since otherwise its complex conjugate would have the same [modulus](../../../../modulus.md). If $\lambda>0$, $v_k$ approaches one unit [eigenvector](../../../../eigenvector.md); if $\lambda<0$, successive $v_k$ alternate signs. In either case,

$$
\boxed{\min_{\sigma\in\{-1,1\}}
\left\|v_k-\sigma\frac{u_1}{\|u_1\|_2}\right\|_2=O(q^k).}
$$

This is the [sign and phase in power iteration](../../../../sign-and-phase-in-power-iteration.md) qualification. Also, the necessary assumption is a nonzero coefficient $c_1$ in the [eigenbasis](../../../../eigenbasis.md), rather than merely a nonzero ordinary [inner product](../../../../inner-product-split.md) with $u_1$: those tests can differ for a [nonsymmetric matrix](../../../../nonsymmetric-matrix.md). If $c_1=0$, the method cannot generate the missing component.

If the dominant value $\lambda$ has a higher-dimensional [eigenspace](../../../../eigenspace.md), the same argument replaces $c_1u_1$ by the nonzero sum of all starting components in that [eigenspace](../../../../eigenspace.md). The limiting direction is then that of this sum, which is still an [eigenvector](../../../../eigenvector.md) for $\lambda$. The usual algorithm assumes $\lambda\ne0$; a strict dominance gap guarantees this whenever another [eigenvalue](../../../../eigenvalue.md) is present.

An estimate retaining the sign of $\lambda$ is the [Rayleigh quotient](../../../../rayleigh-quotient.md)

$$
\boxed{\widehat\lambda_k=\frac{v_k^TAv_k}{v_k^Tv_k}\longrightarrow\lambda.}
$$

Continuity of this quotient at a nonzero [eigenvector](../../../../eigenvector.md) proves the limit even when $A$ is a [nonsymmetric matrix](../../../../nonsymmetric-matrix.md). Alternatively, $(Av_k)_i/(v_k)_i\to\lambda$ for a coordinate whose limiting [eigenvector](../../../../eigenvector.md) component is nonzero. The scaling factor $\|Av_k\|_2$ alone tends only to $|\lambda|$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
