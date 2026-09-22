# Dirichlet-Robin eigenvalues on a finite interval

↑ **Parent:** [Sturm-Liouville problem](sturm-liouville-problem.md)

For $\ell>0$ and $k>0$, the [Sturm-Liouville problem](sturm-liouville-problem.md) with one [Dirichlet boundary condition](dirichlet-boundary-condition.md) and one [Robin boundary condition](robin-boundary-condition.md) has positive [eigenvalues](eigenvalue.md). Indeed, [integration by parts](integration-by-parts.md) gives

$$
\lambda\int_0^\ell y^2\,dx=\int_0^\ell(y')^2\,dx+k y(\ell)^2>0
$$

for every nonzero [eigenfunction](eigenfunction.md). Let $z=\ell\sqrt\lambda$ and $\kappa=k\ell$. The [eigenfunctions](eigenfunction.md) are proportional to $\sin(zx/\ell)$, with

$$
\tan z=-\frac z\kappa.
$$

For each $n\geq1$, there is exactly one root $z_n$ in $((n-1/2)\pi,n\pi)$: on that interval $\tan z+z/\kappa$ increases strictly from $-\infty$ to a positive value. There are no other positive roots. The apparent root $z=0$ gives only the zero sine function and is not an [eigenvalue](eigenvalue.md).

For fixed $k,\ell$, write $z_n=(n-1/2)\pi+\varepsilon_n$. The root equation becomes $\kappa\cot\varepsilon_n=(n-1/2)\pi+\varepsilon_n$, hence

$$
\varepsilon_n=\frac{\kappa}{(n-1/2)\pi}+O(n^{-3}),\qquad
\lambda_n=\frac{(n-1/2)^2\pi^2}{\ell^2}+\frac{2k}{\ell}+O(n^{-2}).
$$

An optional unit normalization uses $\int_0^\ell\sin^2(\sqrt{\lambda_n}x)\,dx=\ell/2+k/[2(k^2+\lambda_n)]$. The positive sign of the Robin boundary term matters: reversing it can introduce nonpositive modes, as in [nonpositive modes in a Dirichlet-Robin interval expansion](nonpositive-modes-in-a-dirichlet-robin-interval-expansion.md).

## ↑ Ancestors (6)

1. [Sturm-Liouville problem](sturm-liouville-problem.md)
2. [Sturm-Liouville theory](sturm-liouville-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/1/e/solution.md)
