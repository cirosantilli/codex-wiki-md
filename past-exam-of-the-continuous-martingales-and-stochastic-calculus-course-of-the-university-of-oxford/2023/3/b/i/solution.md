<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\rho=|z_0|$ and $f(x,y)=\log\sqrt{x^2+y^2}$. On the [annulus](../../../../../annulus-mathematics.md) $r<\sqrt{x^2+y^2}<R$, its [gradient](../../../../../gradient.md) and [Laplace operator](../../../../../laplace-operator.md) are

$$
f_x=\frac{x}{x^2+y^2},\qquad f_y=\frac{y}{x^2+y^2},
\qquad \Delta f=0.
$$

Thus $f$ is a [harmonic function](../../../../../harmonic-function.md) there. The stopped [Itô formula](../../../../../ito-s-lemma.md) gives

$$
\log|B_{t\wedge\tau}|=\log\rho
+\int_0^{t\wedge\tau}\frac{B_1(s)}{|B_s|^2}\,dB_1(s)
+\int_0^{t\wedge\tau}\frac{B_2(s)}{|B_s|^2}\,dB_2(s).
$$

The sum of the squared coefficients is $|B_s|^{-2}\leq r^{-2}$ before $\tau$. The [Itô isometry](../../../../../ito-isometry.md) therefore makes the stochastic term a true [square-integrable](../../../../../square-integrable-function.md) [martingale](../../../../../martingale-split.md) on every finite interval. Continuity prevents overshoot at exit, so $\log r\leq\log|B_{t\wedge\tau}|\leq\log R$. This proves the required bounded [martingale](../../../../../martingale-split.md) property.

Before taking the terminal [expectation](../../../../../expected-value-split.md), prove that $\tau$ is finite. Set $\theta_R=\inf\{t\geq0:|B_t|=R\}$. The [Itô formula](../../../../../ito-s-lemma.md) for $|B|^2$ shows that

$$
|B_{t\wedge\theta_R}|^2-\rho^2-2(t\wedge\theta_R)
$$

is a [martingale](../../../../../martingale-split.md), since its stopped stochastic integrands are bounded. Taking [expectations](../../../../../expected-value-split.md) yields

$$
2\mathbb E(t\wedge\theta_R)
=\mathbb E|B_{t\wedge\theta_R}|^2-\rho^2\leq R^2-\rho^2.
$$

The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives $\mathbb E\theta_R\leq(R^2-\rho^2)/2<\infty$. Hence $\tau\leq\theta_R<\infty$ [almost surely](../../../../../almost-sure-convergence.md).

The [bounded convergence theorem](../../../../../bounded-convergence-theorem.md), equivalently the [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to this bounded [martingale](../../../../../martingale-split.md), gives $\mathbb E\log|B_\tau|=\log\rho$. The two exit events partition the sample space up to a null set. Writing $p=\mathbb P(\tau_r<\tau_R)$,

$$
\log\rho=p\log r+(1-p)\log R.
$$

Solving gives the [planar Brownian annulus hitting probability](../../../../../planar-brownian-annulus-hitting-probability.md)

$$
\boxed{\mathbb P(|B_\tau|=r)=\mathbb P(\tau_r<\tau_R)
=\frac{\log(R/\rho)}{\log(R/r)}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
