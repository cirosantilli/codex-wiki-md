# Spectral error bound for a diagonalizable fixed-point iteration

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)

Suppose $x_{n+1}=Gx_n+c$ has a [fixed point](fixed-point.md) $x_*$ and $G=SDS^{-1}$ with diagonal $D$. For $e_n=x_n-x_*$ and $f_n=S^{-1}e_n$, subtraction gives $f_n=D^nf_0$. In the [Euclidean norm](euclidean-norm.md),

$$
\|f_n\|_2^2=\sum_i|\lambda_i|^{2n}|(f_0)_i|^2\le\rho(G)^{2n}\|f_0\|_2^2.
$$

Thus $\|e_n\|_2\le\|S\|_2\|S^{-1}\|_2\rho(G)^n\|e_0\|_2$. [Spectral radius](spectral-radius.md) below one implies [convergence](convergence.md) for every start. The unit-constant bound belongs to the transformed coordinates; it does not automatically hold in the original [Euclidean norm](euclidean-norm.md) when $S$ is nonorthogonal.

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/6/a/iii/solution.md)
