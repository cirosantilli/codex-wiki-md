# Gauss-Seidel iteration can diverge for an invertible matrix

↑ **Parent:** [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)

An [invertible matrix](invertible-matrix.md) and nonzero diagonal entries make the update well defined, but do not guarantee convergence. For the original [linear system](system-of-linear-equations.md)

$$
A=\begin{pmatrix}1&2\\2&1\end{pmatrix},\qquad b=\begin{pmatrix}1\\1\end{pmatrix},\qquad x_*=\begin{pmatrix}1/3\\1/3\end{pmatrix},\qquad \det A=-3,
$$

the [Gauss-Seidel method](gauss-seidel-method.md) updates $x^{(k+1)}=1-2y^{(k)}$ and $y^{(k+1)}=1-2x^{(k+1)}=-1+4y^{(k)}$. Starting at zero gives $(1,-1)$, then $(3,-5)$. The second-coordinate [forward error](forward-error.md) is $e_y^{(k)}=-4^k/3$, and the [iteration matrix](iteration-matrix.md) $H=\begin{pmatrix}0&-2\\0&4\end{pmatrix}$ has [spectral radius](spectral-radius.md) $4$. The [linear system](system-of-linear-equations.md) has a unique solution while this particular [stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md) diverges.

## ↑ Ancestors (9)

1. [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)
2. [Gauss-Seidel method](gauss-seidel-method.md)
3. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
4. [Numerical linear algebra](numerical-linear-algebra-split.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
