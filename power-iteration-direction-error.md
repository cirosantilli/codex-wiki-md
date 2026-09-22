# Power iteration direction error

↑ **Parent:** [Power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md)

For a [unit vector](unit-vector.md) $u$ spanning the target [eigenspace](eigenspace.md) and a normalized iterate $x_k$, define

$$
\varepsilon_k=\|(I-uu^*)x_k\|_2=\sqrt{1-|u^*x_k|^2}.
$$

This is the [norm](norm.md) of the component in the [orthogonal complement](orthogonal-complement.md) of $u$, equivalently the sine of the acute [angle](angle.md) to its line. It ignores the arbitrary sign or complex unit factor of an [eigenvector](eigenvector.md). Under [power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md), $\varepsilon_k=O(\gamma^k)$ in [Big O notation](big-o-notation.md). The [orthogonal projection](orthogonal-projection.md) defines how we measure direction; it does not assume that the [eigenbasis](eigenbasis.md) of $A$ is [orthogonal](orthogonal-vectors.md). In computation, the projection form avoids subtracting nearly equal numbers inside the square root.

## ↑ Ancestors (8)

1. [Power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md)
2. [Power iteration](power-iteration.md)
3. [Numerical linear algebra](numerical-linear-algebra.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Exact two-dimensional power iteration](exact-two-dimensional-power-iteration.md)
- [Sign and phase in power iteration](sign-and-phase-in-power-iteration.md)
