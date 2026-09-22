# Unconditionally stable corrected directional diffusion splitting

↑ **Parent:** [One-implicit-direction diffusion splitting](one-implicit-direction-diffusion-splitting.md)

Adding the correction

$$
u^{n+1}=\widetilde u^{n+1}+\mu A_x(u^{n+1}-u^n)
$$

gives

$$
D=(I-\mu A_x)^{-1}(I+\mu^2A_xA_y)(I-\mu A_y)^{-1}.
$$

Its common-basis eigenvalues are

$$
d_{pq}=\frac{1+\mu^2\lambda_p\lambda_q}
{(1-\mu\lambda_p)(1-\mu\lambda_q)}.
$$

Since $\lambda_p,\lambda_q<0$, one has $0<d_{pq}\leq1$ for every $\mu>0$.

## ↑ Ancestors (10)

1. [One-implicit-direction diffusion splitting](one-implicit-direction-diffusion-splitting.md)
2. [Five-point Dirichlet Laplacian as a Kronecker sum](five-point-dirichlet-laplacian-as-a-kronecker-sum.md)
3. [Dirichlet discrete Laplacian](dirichlet-discrete-laplacian.md)
4. [Finite difference method](finite-difference-method.md)
5. [Finite difference](finite-difference-split.md)
6. [Numerical analysis](numerical-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/41c/c/solution.md)
