<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a shift $\mu$ which is not an [eigenvalue](../../../../eigenvalue.md). [Inverse iteration](../../../../inverse-iteration.md) applies [power iteration](../../../../power-iteration.md) to $B=(A-\mu I)^{-1}$, implemented by a [linear system](../../../../system-of-linear-equations.md) solve rather than by forming an explicit [matrix inverse](../../../../matrix-inverse-split.md):

$$
\boxed{(A-\mu I)w_{k+1}=v_k,\qquad
v_{k+1}=\frac{w_{k+1}}{\|w_{k+1}\|_2}.}
$$

A single [LU decomposition](../../../../lu-decomposition.md) of $A-\mu I$ can be reused for all the solves at this fixed shift. An [eigenpair](../../../../eigenpair.md) $Au_j=\lambda_ju_j$ transforms into

$$
Bu_j=\frac1{\lambda_j-\mu}u_j.
$$

Thus an [eigenvalue](../../../../eigenvalue.md) $\lambda_*$ uniquely closest to $\mu$ becomes the [dominant eigenvalue](../../../../dominant-eigenvalue.md) of $B$. For a [diagonalizable matrix](../../../../diagonalizable-matrix.md), the argument in the preceding subpart gives [convergence of diagonalizable fixed-shift inverse iteration](../../../../convergence-of-diagonalizable-fixed-shift-inverse-iteration.md), provided the starting coefficient in the target [eigenspace](../../../../eigenspace.md) is nonzero, with [power iteration direction error](../../../../power-iteration-direction-error.md) $O(q_\mu^k)$, where

$$
\boxed{q_\mu=
\frac{|\lambda_*-\mu|}{\min_{j:\lambda_j\ne\lambda_*}|\lambda_j-\mu|}<1.}
$$

For any prescribed [simple eigenvalue](../../../../simple-eigenvalue.md), taking a sufficiently close but unequal shift makes the numerator small while the denominator stays close to its positive separation from the remaining [eigenvalues](../../../../eigenvalue.md). This makes $q_\mu$ small and gives very fast convergence per iteration. The [Rayleigh quotient](../../../../rayleigh-quotient.md) of $v_k$ estimates $\lambda_*$ directly. If $\beta_k$ estimates the associated [eigenvalue](../../../../eigenvalue.md) of $B$, the corresponding estimate is $\mu+\beta_k^{-1}$.

The selection principle also applies when the other [eigenvalues](../../../../eigenvalue.md) have nontrivial blocks in the [Jordan normal form](../../../../jordan-normal-form.md): their contributions acquire powers of $k$, multiplying strictly smaller geometric factors. A simple uniquely closest [eigenvalue](../../../../eigenvalue.md) still attracts the direction when the [Riesz projection](../../../../riesz-projection.md) of $v_0$ onto its generalized [eigenspace](../../../../eigenspace.md) is nonzero. For nonreal target [eigenvalues](../../../../eigenvalue.md), allow complex shifts and arithmetic; a real shift cannot distinguish a conjugate pair of equal distances. Setting $\mu=\lambda_*$ makes the solve singular, and an exactly zero starting target component prevents convergence to that target in exact arithmetic. When $\lambda_*<\mu$ is real, account for the [sign behavior of fixed-shift inverse iteration](../../../../sign-behavior-of-fixed-shift-inverse-iteration.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
