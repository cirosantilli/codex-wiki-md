# Symmetric positive-definite preconditioning

↑ **Parent:** [Matrix preconditioning](matrix-preconditioning.md)

Let $A$ and $M$ be real [symmetric positive-definite matrices](symmetric-positive-definite-matrix.md). The [principal square root of a positive semidefinite matrix](principal-square-root-of-a-positive-semidefinite-matrix.md) construction gives an [invertible matrix](invertible-matrix.md) for each. Set

$$
S=M^{1/2},\qquad B=S^{-1}AS^{-1},\qquad y=Sx,\qquad c=S^{-1}b.
$$

Then $Ax=b$ is equivalent to $By=c$. This is a [matrix congruence](matrix-congruence.md), and $B$ is a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md): $B^T=B$, and for every nonzero [vector](vector.md) $v$,

$$
v^TBv=(S^{-1}v)^TA(S^{-1}v)>0,
$$

since $S^{-1}v\ne0$. This short proof establishes both requirements for applying the [Conjugate gradient method](conjugate-gradient-method.md) to the transformed [linear system](system-of-linear-equations.md).

The left transformed [matrix](matrix.md) has the same [eigenvalues](eigenvalue.md) because

$$
M^{-1}A=S^{-1}BS.
$$

Its correct geometry uses the [weighted inner product](weighted-inner-product.md) $\langle u,v\rangle_M=u^TMv$: $\langle u,M^{-1}Av\rangle_M=u^TAv=\langle M^{-1}Au,v\rangle_M$. Thus it is symmetric in this [inner product](inner-product-split.md), even when it is not a [symmetric matrix](symmetric-matrix.md) in ordinary coordinates. The spectral [condition number](condition-number.md) governing the transformed symmetric problem is $\kappa_2(B)$, not generally $\kappa_2(M^{-1}A)$.

The [Preconditioned conjugate gradient method](preconditioned-conjugate-gradient-method.md) realizes this transformation using auxiliary solves $Mz_k=r_k$, without constructing $S$ or its [matrix inverse](matrix-inverse-split.md). With fixed $M$, initialize $r_0=b-Ax_0$ and $p_0=z_0$; while $r_k\ne0$, use

$$
\alpha_k=\frac{r_k^Tz_k}{p_k^TAp_k},\quad x_{k+1}=x_k+\alpha_kp_k,\quad r_{k+1}=r_k-\alpha_kAp_k,
$$

then solve $Mz_{k+1}=r_{k+1}$ and set

$$
\beta_k=\frac{r_{k+1}^Tz_{k+1}}{r_k^Tz_k},\qquad p_{k+1}=z_{k+1}+\beta_kp_k.
$$

Stop at a zero [linear-system residual](linear-system-residual.md) before forming another ratio. Positive definiteness makes the denominators positive before termination.[Math 221, Matrix Computations, Fall 2023; Notes for Ma221 Lecture 15, Dec 1, 2023; PDF p. 1, equivalent symmetric system and Preconditioned CG algorithm](math-221-matrix-computations-fall-2023/notes-for-ma221-lecture-15-dec-1-2023.md)

An [invertible matrix](invertible-matrix.md) alone is insufficient: with $A=I$ and $M=\operatorname{diag}(-1,1)$, the left transformed [matrix](matrix.md) has [eigenvalues](eigenvalue.md) $-1,1$, and $M$ has no real [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) square root. Even a valid [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) can worsen conditioning if its scaling is unsuitable, as the next worked example shows.

**Table of contents**

- [Symmetric preconditioning as energy geometry](symmetric-preconditioning-as-energy-geometry.md)

## ↑ Ancestors (7)

1. [Matrix preconditioning](matrix-preconditioning.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Diagonal scaling for a two-dimensional linear system](diagonal-scaling-for-a-two-dimensional-linear-system.md)
- [Left preconditioning](left-preconditioning.md)
- [Symmetric preconditioning as energy geometry](symmetric-preconditioning-as-energy-geometry.md)
