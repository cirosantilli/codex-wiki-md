<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

The [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) identity $T_m(\cos\theta)=\cos(m\theta)$ implies $|T_m(x)|\leq1$ on $[-1,1]$. Since $\sum_i\gamma_i<\infty$, the [Weierstrass M-test](../../../../../weierstrass-m-test.md) shows that

$$
f(x)=\sum_{i=1}^{\infty}\gamma_iT_{3^i}(x)
$$

converges uniformly on $[-1,1]$. Every partial sum is continuous, so the [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes $f$ a well-defined continuous function.

Let

$$
P_n=\sum_{i=1}^n\gamma_iT_{3^i},
\qquad
x_k=-\cos\frac{k\pi}{3^{n+1}}
\quad(0\leq k\leq3^{n+1}).
$$

Then $-1=x_0<x_1<\cdots<x_{3^{n+1}}=1$. Since every $3^i$ is odd and, for $i\geq n+1$, $3^{i-n-1}$ is an odd integer,

$$
T_{3^i}(x_k)
=-\cos\left(k\pi3^{i-n-1}\right)=(-1)^{k+1}.
$$

It follows that

$$
\boxed{f(x_k)-P_n(x_k)
=(-1)^{k+1}\sum_{i=n+1}^{\infty}\gamma_i}.
$$

Thus the error has equal alternating extrema at $3^{n+1}+1$ ordered points. The [Chebyshev alternation theorem](../../../../../equioscillation-theorem.md) shows that $P_n$ is a best uniform approximation among polynomials of degree at most $3^{n+1}-1$, and in particular

$$
E_{3^{n+1}-1}(f)
:=\inf_{\deg P\leq3^{n+1}-1}\lVert f-P\rVert_\infty
\geq\sum_{i=n+1}^{\infty}\gamma_i.
$$

Now let $(\delta_N)$ be the prescribed decreasing positive sequence. Define

$$
s_0=\delta_1+1,
\qquad
s_j=\delta_{3^j}+2^{-j}\quad(j\geq1),
\qquad
\gamma_j=s_{j-1}-s_j.
$$

Then $s_j$ decreases strictly to zero, so every $\gamma_j>0$, the series $\sum_j\gamma_j=s_0$ converges, and

$$
\sum_{i=j+1}^{\infty}\gamma_i=s_j\geq\delta_{3^j}.
$$

Given $N\geq1$, choose $j\geq0$ with $3^j\leq N\leq3^{j+1}-1$. Monotonicity of best-approximation errors and of $\delta_N$ gives

$$
E_N(f)\geq E_{3^{j+1}-1}(f)
\geq s_j
\geq\delta_{3^j}
\geq\delta_N.
$$

Hence this continuous $f$ satisfies

$$
\boxed{\sup_{t\in[-1,1]}|f(t)-P(t)|\geq\delta_N}
$$

for every polynomial $P$ of degree at most $N$. This is the polynomial form of [Bernstein's lethargy theorem](../../../../../bernstein-s-lethargy-theorem.md).

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
