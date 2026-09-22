# Successive over-relaxation

↑ **Parent:** [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Successive_over-relaxation)

For a splitting $A=D+L+U$, [successive over-relaxation](successive-over-relaxation.md) updates

$$
(D+\omega L)x^{(k+1)}=[(1-\omega)D-\omega U]x^{(k)}+\omega b.
$$

It reduces to the [Gauss-Seidel method](gauss-seidel-method.md) at $\omega=1$. If $A$ is symmetric positive definite, the [Householder-John theorem](householder-john-theorem.md) applies to $M=D/\omega+L$, $N=(1/\omega-1)D-U$, since $M^T+N=(2/\omega-1)D$ is positive definite for $0<\omega<2$.

## ↑ Ancestors (7)

1. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
2. [Numerical linear algebra](numerical-linear-algebra.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gauss-Seidel method](gauss-seidel-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/39a/solution.md)
- [Successive over-relaxation](successive-over-relaxation.md)
