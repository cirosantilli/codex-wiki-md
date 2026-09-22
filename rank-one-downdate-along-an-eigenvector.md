# Rank-one downdate along an eigenvector

↑ **Parent:** [Positive-definite matrix](positive-definite-matrix.md)

Let $A$ be a real symmetric [positive-definite matrix](positive-definite-matrix.md), and let $b$ be a unit [eigenvector](eigenvector.md) with [eigenvalue](eigenvalue.md) $\lambda>0$. The [rank-one matrix update](rank-one-matrix-update.md) $C=A-\rho bb^T$ changes only the [eigenvalue](eigenvalue.md) along $b$, to $\lambda-\rho$. [Symmetry](symmetry-physics.md) makes the [orthogonal complement](orthogonal-complement.md) $b^\perp$ invariant, and $Cw=Aw$ there because $b^Tw=0$.

In detail, write $x=tb+w$ with $w\perp b$. Then

$$
x^TCx=(\lambda-\rho)t^2+w^TAw.
$$

Consequently $C$ is a [positive-definite matrix](positive-definite-matrix.md) for $\rho<\lambda$, singular for $\rho=\lambda$, and has exactly one negative [eigenvalue](eigenvalue.md) for $\rho>\lambda$. In dimension at least two the last case is indefinite. In dimension one it is [negative definite](negative-definite-matrix.md) instead: there is no nonzero orthogonal-complement direction. The distinction matters when classifying a [stationary point](stationary-point.md) of a [quadratic form](quadratic-form-split.md).

## ↑ Ancestors (8)

1. [Positive-definite matrix](positive-definite-matrix.md)
2. [Definite matrix](definite-matrix.md)
3. [Quadratic form](quadratic-form-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/5/b/ii/solution.md)
