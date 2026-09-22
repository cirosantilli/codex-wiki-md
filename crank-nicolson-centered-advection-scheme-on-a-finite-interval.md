# Crank-Nicolson centered-advection scheme on a finite interval

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

Let $D$ be the real skew-symmetric tridiagonal matrix with superdiagonal $1$ and subdiagonal $-1$. The centered-space Crank-Nicolson discretization of $u_t=u_x$ has amplification matrix

$$
Q=(I-\mu D/4)^{-1}(I+\mu D/4).
$$

The eigenvalues of $D$ are $2i\cos(j\pi/(M+1))$, so those of $Q$ are Cayley transforms

$$
q_j=\frac{1+i(\mu/2)\cos(j\pi/(M+1))}
{1-i(\mu/2)\cos(j\pi/(M+1))}.
$$

They all have modulus one, and their common orthonormal eigenbasis makes $Q$ normal. Hence the method is stable for every $\mu>0$.

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/40e/b/solution.md)
