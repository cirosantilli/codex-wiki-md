# Exact Newton error identity for a quadratic

↑ **Parent:** [Newton root-finding iteration](newton-root-finding-iteration.md)

For the [quadratic polynomial](quadratic-polynomial.md) $f(x)=(x-a)^2-b^2$ with $b>0$, consider the [Newton root-finding iteration](newton-root-finding-iteration.md) towards the [polynomial root](root-of-a-polynomial.md) $x_*=a+b$. If $x_k\ne a$, its signed error $e_k=x_k-x_*$ satisfies

$$
e_{k+1}=\frac{e_k^2}{2(x_k-a)}.
$$

Indeed the iteration for $u_k=x_k-a$ is $u_{k+1}=(u_k+b^2/u_k)/2$, and subtracting $b$ yields $(u_k-b)^2/(2u_k)$. This exact identity explains [quadratic convergence](quadratic-convergence.md) near the simple [polynomial root](root-of-a-polynomial.md). If an initial error is asymptotic to $C\varepsilon^m$ and $x_k-a\to b\ne0$ as $\varepsilon\to0$, one step changes its leading power to $2m$ and its coefficient to $C^2/(2b)$.

## ↑ Ancestors (6)

1. [Newton root-finding iteration](newton-root-finding-iteration.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/19/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/19/b/iii/solution.md)
