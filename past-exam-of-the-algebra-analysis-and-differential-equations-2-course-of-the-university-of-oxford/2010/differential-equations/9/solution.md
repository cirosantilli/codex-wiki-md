<h1 id="differential-equations/9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

For an azimuth-independent product $u=R(r)\Theta(\theta)$, multiply [Laplace's equation](../../../../laplace-equation.md) by $r^2/(R\Theta)$ where the factors are nonzero. The radial and angular expressions must equal opposite constants:

$$
\boxed{r^2R''+2rR'=\lambda R,\qquad(\sin\theta\,\Theta')'=-\lambda\sin\theta\,\Theta.}
$$

The resulting differential identities extend across isolated zeros by [continuity](../../../../continuous-function.md). Put $\rho=\cos\theta$. Then $\Theta'=-\sin\theta P'$ and

$$
(\sin\theta\,\Theta')'=\sin\theta\frac d{d\rho}\bigl((1-\rho^2)P'\bigr).
$$

This gives $((1-\rho^2)P')'+\lambda P=0$ on $(-1,1)$.

A nonzero angular factor must be regular at both poles: it must be bounded as $\rho\to\pm1$ and extend smoothly as an axisymmetric function on the [sphere](../../../../sphere.md). Equivalently one may use the regular endpoint solution at each end; the logarithmic endpoint solutions are excluded. These two endpoint conditions select $\boxed{\lambda=n(n+1),\ n=0,1,2,\ldots}$ and the multiples of $P_n$. It is not sufficient to impose no condition at the endpoints, since local solutions exist for arbitrary $\lambda$. One way to see the quantization is the regular Legendre series about one endpoint: unless it terminates at $\lambda=n(n+1)$, continuation to the other endpoint has a logarithmic singularity.

Direct differentiation verifies

$$
\begin{array}{c|c|c}
P&\lambda&R(r)\\\hline
1&0&A+B/r\\
\rho&2&Ar+Br^{-2}\\
(3\rho^2-1)/2&6&Ar^2+Br^{-3}
\end{array}
$$

Indeed $R=r^m$ gives $m(m+1)=\lambda$, so the two powers for degree $n$ are $r^n$ and $r^{-n-1}$.

For the shell assume $a>1$. The outer datum decomposes as $\rho^2=\tfrac13P_0(\rho)+\tfrac23P_2(\rho)$. Normalize each [radial solution](../../../../radial-function.md) to vanish at $1$ and equal $1$ at $a$; [superposition](../../../../superposition-principle.md) gives

$$
\boxed{u(r,\theta)=\frac13\frac{1-r^{-1}}{1-a^{-1}}+\frac23\frac{r^2-r^{-3}}{a^2-a^{-3}}P_2(\cos\theta).}
$$

Every term is [harmonic](../../../../harmonic-function.md) in the shell and regular at the angular poles; substitution at each boundary gives precisely the two prescribed data. For uniqueness among functions [harmonic](../../../../harmonic-function.md) in the shell and [continuous](../../../../continuous-function.md) on its closure, subtract any two solutions. Their difference is [harmonic](../../../../harmonic-function.md), zero on both boundary spheres, and by the [maximum principle](../../../../maximum-principle.md) is both at most zero and at least zero on the bounded shell. It vanishes identically. Thus **the classical [Dirichlet solution](../../../../dirichlet-problem.md) is unique**. The usual [continuity](../../../../continuous-function.md) at the boundary is the interpretation of the stated [boundary conditions](../../../../boundary-condition.md); allowing singular boundary behavior would remove that hypothesis.

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Differential Equations](../../differential-equations.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
