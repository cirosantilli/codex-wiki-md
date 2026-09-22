# Asymptotic regularization

↑ **Parent:** [Spectral regularization method](spectral-regularization-method.md)

Asymptotic regularization stops the [gradient flow](gradient-flow.md) $x'=-A^*(Ax-f)$ at $t=1/\alpha$, starting from zero. With the [singular system of a compact operator](singular-system-of-a-compact-operator.md) convention $Av_j=\sigma_j u_j$, its spectral filter gives

$$
R_\alpha f=\sum_j\frac{1-e^{-\sigma_j^2/\alpha}}{\sigma_j}\langle f,u_j\rangle v_j.
$$

The scalar coefficient solves $c_j'=-\sigma_j^2c_j+\sigma_j\langle f,u_j\rangle$ with zero initial value. Since $1-e^{-s}\leq\min(s,1)$ for $s\geq0$, the [operator norm](operator-norm.md) is at most $\alpha^{-1/2}$. On the domain of the [Moore–Penrose inverse of an operator](moore-penrose-inverse-of-an-operator.md), [dominated convergence theorem](dominated-convergence-theorem.md) of the squared spectral coefficients proves $R_\alpha f\to A^\dagger f$. The [noise-bias decomposition for linear regularization](noise-bias-decomposition-for-linear-regularization.md) then gives noisy-data convergence when $\delta/\sqrt\alpha\to0$.

## ↑ Ancestors (7)

1. [Spectral regularization method](spectral-regularization-method.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326/1/c/solution.md)
