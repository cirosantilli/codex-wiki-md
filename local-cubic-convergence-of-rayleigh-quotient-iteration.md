# Local cubic convergence of Rayleigh quotient iteration

↑ **Parent:** [Rayleigh quotient iteration](rayleigh-quotient-iteration.md)

Let a real symmetric matrix have simple eigenpairs $(\lambda_i,w_i)$ and let

$$
x=c^{-1}\left(w_1+\epsilon\sum_{i\geq2}a_iw_i\right).
$$

Then its [Rayleigh quotient](rayleigh-quotient.md) is

$$
R_A(x)=\lambda_1+\epsilon^2D+O(\epsilon^4),
\qquad
D=\sum_{i\geq2}a_i^2(\lambda_i-\lambda_1).
$$

After one shifted inverse solve and normalization, the relative coefficients are

$$
-\epsilon^3\frac{Da_i}{\lambda_i-\lambda_1}+O(\epsilon^5).
$$

Thus the eigenvector direction error is cubed at each sufficiently close iterate.

## ↑ Ancestors (8)

1. [Rayleigh quotient iteration](rayleigh-quotient-iteration.md)
2. [Rayleigh quotient](rayleigh-quotient.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/41e/b/solution.md)
