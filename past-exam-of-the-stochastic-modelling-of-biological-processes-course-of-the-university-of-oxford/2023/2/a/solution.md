<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The native PDF repeats $dW_y$ in its list of independent noise terms, whereas its third [stochastic differential equation](../../../../stochastic-differential-equation.md) uses $dW_z$. We use the intended three independent coordinate [Brownian motions](../../../../brownian-motion-split.md) $W_x,W_y,W_z$.

Put $\mathbf X=(X,Y,Z)$, $r=|\mathbf X|$ and $S=r^2$. Before the origin is reached, [Itô's formula](../../../../ito-s-lemma.md) gives

$$
\begin{aligned}
dS&=2\mathbf X\mathbin{\cdot}d\mathbf X+(dX)^2+(dY)^2+(dZ)^2\\
&=(6-2\alpha)\,dt+2\sqrt2\,\mathbf X\mathbin{\cdot}d\mathbf W.
\end{aligned}
$$

The $6$ is the sum of three [quadratic variation](../../../../quadratic-variation.md) terms, each $2\,dt$. The [drift](../../../../drift-coefficient.md) contribution is $-2\alpha\,dt$ because the numerator is $|\mathbf X|^2$. The radial [stochastic integral](../../../../stochastic-integral.md) can be written using a scalar [Brownian motion](../../../../brownian-motion-split.md) $B$:

$$
dS=2(3-\alpha)\,dt+2\sqrt{2S}\,dB,
\qquad
d(S/2)=(3-\alpha)\,dt+2\sqrt{S/2}\,dB.
$$

Thus $S/2$ is a [squared Bessel process](../../../../squared-bessel-process.md) of dimension $\delta=3-\alpha$ until it reaches zero. If this equation is taken globally with the usual nonnegative [squared Bessel process](../../../../squared-bessel-process.md) continuation, taking [expected values](../../../../expected-value-split.md) gives

$$
\mathbb E S(t)=r_0^2+2(3-\alpha)t,
\qquad
\boxed{\lim_{t\to\infty}\frac{\mathbb E S(t)}t=6-2\alpha.}
$$

The [stochastic integral](../../../../stochastic-integral.md) has zero [expected value](../../../../expected-value-split.md): stopping first at large levels bounds the integrands, yields a finite first [moment](../../../../moment.md) for $S$, and then makes $\mathbb E\int_0^tS(u)\,du$ finite, so the unrestricted integral is a square-integrable [martingale](../../../../martingale-split.md).

**Boundary qualification.** The punctured domain in the question does not itself specify that continuation. The boundary classification of a [Bessel process](../../../../bessel-process.md) says that the origin is inaccessible from $r_0>0$ when $\delta\geq2$, equivalently $\alpha\leq1$. In this parameter range the original [stochastic differential equation](../../../../stochastic-differential-equation.md) is global in the stated domain and the boxed result holds as written.

For $1<\alpha<3$, we have $0<\delta<2$: the origin is reached in finite time with [probability](../../../../probability.md) one. One can also see accessibility directly from the radial [generator of an SDE diffusion](../../../../generator-of-an-sde-diffusion.md)

$$
L_rf=f''+\frac{2-\alpha}{r}f'.
$$

For $r<b$, the [harmonic function](../../../../harmonic-function.md) $1-(r/b)^{\alpha-1}$ is the [probability](../../../../probability.md) of reaching zero before $b$. Finite-time access follows by using the nonnegative function

$$
v_b(r)=\frac{b^{3-\alpha}r^{\alpha-1}-r^2}{2(3-\alpha)},
\qquad L_rv_b=-1,\qquad v_b(0)=v_b(b)=0,
$$

in the stopped [Itô formula](../../../../ito-s-lemma.md); it bounds the [expected value](../../../../expected-value-split.md) of the time to reach zero or $b$. Letting $b\to\infty$ gives almost sure finite hitting of zero. The coefficients of the original vector [stochastic differential equation](../../../../stochastic-differential-equation.md) are undefined there, so its stated punctured-domain version has no prescribed long-time evolution in this range.

The natural continuing radial [squared Bessel process](../../../../squared-bessel-process.md) gives $6-2\alpha$, but stopping and holding the particle at the origin would give a different answer. Indeed, with $T_0$ the first hit of zero, [Itô's formula](../../../../ito-s-lemma.md) for the stopped process gives

$$
\mathbb E S(t\wedge T_0)=r_0^2+2(3-\alpha)\mathbb E(t\wedge T_0).
$$

Since $T_0<\infty$ almost surely, [dominated convergence](../../../../dominated-convergence-theorem.md) applied to $(t\wedge T_0)/t\leq1$ gives

$$
\lim_{t\to\infty}\frac{\mathbb E S(t\wedge T_0)}t=0.
$$

Therefore **$6-2\alpha$ is the usual continued-radial answer; for $1<\alpha<3$ a boundary convention is necessary.** It is not a uniquely defined limit for the punctured-domain model alone.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
