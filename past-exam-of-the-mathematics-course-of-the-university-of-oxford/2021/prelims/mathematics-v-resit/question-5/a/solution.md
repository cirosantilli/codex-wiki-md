<h1 id="question-5/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Treat the boundary data as $2\pi$-periodic in the angular variable. Denote the outer data by $g(\theta)$, and set $h(\theta)=f(a,\theta)$ for the inner data. Define their mean and nonconstant [Fourier coefficients](../../../../../../fourier-coefficient.md) by

$$
\begin{aligned}
p_0&=\frac1{2\pi}\int_{-\pi}^{\pi}h(t)\,dt,\\
p_n&=\frac1\pi\int_{-\pi}^{\pi}h(t)\cos(nt)\,dt,\qquad
q_n=\frac1\pi\int_{-\pi}^{\pi}h(t)\sin(nt)\,dt\quad(n\geq1).
\end{aligned}
$$

The outer data have [reflection symmetry](../../../../../../reflection-symmetry.md), so all their sine [Fourier coefficients](../../../../../../fourier-coefficient.md) vanish. Their mean is $1/2$, and their cosine [Fourier coefficients](../../../../../../fourier-coefficient.md) are

$$
c_n=\frac1\pi\int_{-\pi/2}^{\pi/2}\cos(nt)\,dt
=\frac{2\sin(n\pi/2)}{\pi n}.
$$

The angular [Fourier harmonics](../../../../../../fourier-harmonic.md) for a single-valued [harmonic function](../../../../../../harmonic-function.md) in an [annulus](../../../../../../annulus-mathematics.md) are $\cos(n\theta)$ and $\sin(n\theta)$, with [integer](../../../../../../integer-split.md) $n\geq1$. Their radial factors are independent combinations of $r^n$ and $r^{-n}$; the zero angular mode has radial factor $A_0+B_0\log r$. For arbitrary inner data, the sine and cosine modes need independent radial coefficients: forcing them to share one radial factor, as in the product form supplied in the paper, would impose an extra restriction. For either sine or cosine mode, if its outer and inner coefficients are $v$ and $w$, the radial coefficients $\alpha,\beta$ obey

$$
\alpha+\beta=v,\qquad a^n\alpha+a^{-n}\beta=w.
$$

Solving this [linear system](../../../../../../system-of-linear-equations.md) gives

$$
\alpha=\frac{v-a^nw}{1-a^{2n}},\qquad
\beta=\frac{a^n(w-a^nv)}{1-a^{2n}}.
$$

It is convenient to collect the result into the [annular harmonic interpolation factors](../../../../../../annular-harmonic-interpolation-factor.md)

$$
H_n(r)=\frac{r^n-a^{2n}r^{-n}}{1-a^{2n}},\qquad
K_n(r)=\frac{a^n(r^{-n}-r^n)}{1-a^{2n}}.
$$

They satisfy $H_n(1)=1$, $H_n(a)=0$, $K_n(1)=0$ and $K_n(a)=1$. The zero mode satisfies $A_0=1/2$ and $B_0=(p_0-1/2)/\log a$. Therefore the required [separation of variables](../../../../../../separation-of-variables.md) solution is

$$
\boxed{
\begin{aligned}
u(r,\theta)={}&\frac12+\left(p_0-\frac12\right)\frac{\log r}{\log a}\\
&+\sum_{n=1}^{\infty}\left[
c_nH_n(r)\cos(n\theta)
+K_n(r)\bigl(p_n\cos(n\theta)+q_n\sin(n\theta)\bigr)
\right].
\end{aligned}}
$$

All dependence on $f(a,\theta)$ is given by the displayed [integrals](../../../../../../integral-split.md). Substituting $r=a$ leaves its [Fourier series](../../../../../../fourier-series-split.md), and substituting $r=1$ leaves

$$
\frac12+\frac2\pi\sum_{n=1}^{\infty}\frac{\sin(n\pi/2)}n\cos(n\theta),
$$

the [Fourier series](../../../../../../fourier-series-split.md) of the specified outer step. The radial factors satisfy $r^2R''+rR'-n^2R=0$, so each nonconstant term satisfies [Laplace's equation](../../../../../../laplace-equation.md); $1$ and $\log r$ do also. For integrable boundary data the radial factors give exponential decay on every closed subannulus strictly inside $a<r<1$, justifying the necessary termwise [partial derivatives](../../../../../../partial-derivative.md) there.

There is a qualification at the two outer [jump discontinuities](../../../../../../jump-discontinuity.md). By [pointwise convergence of a piecewise smooth Fourier series](../../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md), the outer series gives $1/2$ at $\theta=\pm\pi/2$, whereas the printed data assign $1$ at those two points. Thus **the displayed solution attains the outer data at their continuity points, and has radial limit $1/2$ at the jumps**. One may separately assign the boundary value $1$ at the two exceptional points without changing the interior [harmonic function](../../../../../../harmonic-function.md), but no continuous extension can match the discontinuous data there. For piecewise smooth inner data, the analogous [boundary trace](../../../../../../boundary-trace-of-a-function.md) agrees with $h$ at continuity points and with its midpoint at jumps. Some regularity of $h$ is necessary for a classical interpretation; the problem imposes none explicitly.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [Question 5](../../question-5.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
