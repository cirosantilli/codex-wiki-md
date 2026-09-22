<h1 id="1/d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The time-changed diffusion has generator $\mathcal A=(\kappa/2)\partial_{zz}+2(1/z+1/(z-1))\partial_z$. For $1<z<R$, its [boundary hitting probability from a diffusion scale function](../../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md) is

$$
\mathbb P_z(\tau_R<\tau_1)=\frac{s_\kappa(z)}{s_\kappa(R)}.
$$

To see this directly, stop the scale [local martingale](../../../../../../../local-martingale.md) on $[1+\epsilon,R]$ and pass to $\epsilon\downarrow0$. Exit from $(1,R)$ occurs in finite clock time: the scale density behaves as $(z-1)^{-4/\kappa}$ and the speed density as $(z-1)^{4/\kappa}$, so the usual scale-times-speed exit integral is finite at $1$. More explicitly, with $m(v)=2/(\kappa s_\kappa'(v))$ the [finite-interval diffusion exit Green kernel](../../../../../../../finite-interval-diffusion-exit-green-kernel.md) gives

$$
\mathbb E_z\tau_{1,R}=\int_1^R
\frac{s_\kappa(z\wedge v)[s_\kappa(R)-s_\kappa(z\vee v)]}{s_\kappa(R)}\,m(v)\,dv.
$$

The equation $\mathcal A u=-1$ follows by differentiation and the derivative jump at $v=z$, so stopping the corresponding Itô identity gives this exit bound. The integrand near $1$ is $O(v-1)$; elsewhere it is bounded. At large $z$ the drift is bounded, excluding explosion at infinity in finite clock time.

Here is why these exits describe the original swallowing event. In clock time,

$$
D(u)=D(0)\exp\left(-2\int_0^u\frac{dv}{\widehat Z_v(\widehat Z_v-1)}\right).
$$

If $\widehat Z$ hits $1$ at finite $u$, its integrated [stochastic differential equation](../../../../../../../stochastic-differential-equation.md) shows $\int_0^{\tau_1}(\widehat Z_v-1)^{-1}dv<\infty$: the Brownian term has a finite limit and both positive drift integrals must then have finite limits. Consequently $D(\tau_1)>0$, $X$ hits zero and $Y$ stays positive. This gives $T(x)<T(y)$.

Conversely $T(x)$ is finite by part (b). If its clock ends at a finite value, the diffusion must hit $1$; an interior endpoint with positive $D$ would leave $X$ positive. If the clock runs forever without hitting $1$, the standard one-dimensional scale classification gives escape to infinity whenever $S_\kappa<\infty$. This cannot represent a strict swallowing event, which has $D\to Y_{T(x)}>0$ and $Z\to1$. Hence the surviving event represents $T(x)=T(y)$. This reasoning also explains why a simultaneous collision must be treated separately rather than assigned the boundary value at $1$.

For $\kappa\geq8$, the scale is unbounded. The [maximal inequality for a nonnegative supermartingale](../../../../../../../maximal-inequality-for-a-nonnegative-supermartingale.md) gives $\mathbb P(\sup s_\kappa(\widehat Z)\geq s_\kappa(R))\leq s_\kappa(z)/s_\kappa(R)$; letting $R\to\infty$ rules out escape. Finite-interval exit then forces a hit at $1$. For $4<\kappa<8$, taking $R\to\infty$ gives

$$
\boxed{F(x,y)=1-\frac{s_\kappa(y/(y-x))}{S_\kappa},\qquad
\mathbb P(T(x)=T(y))=\frac{s_\kappa(y/(y-x))}{S_\kappa}>0.}
$$

The strict-event probability is also positive, since $0<s_\kappa(z)<S_\kappa$ for finite $z$.

For $\kappa\geq8$, first intersect the probability-one strict-order events over rational $0<a<b$. The real boundary flow gives nondecreasing swallowing times on $(0,\infty)$. For any $0<x<y$, choose rational $x<a<b<y$; then $T(x)\leq T(a)<T(b)\leq T(y)$. This proves the simultaneous assertion

$$
\boxed{\text{almost surely }T(x)<T(y)\text{ for every }0<x<y,\quad\kappa\geq8.}
$$

The range is positive points, as in the definition of $F$; reflection reverses the ordering on the negative axis. At the printed endpoint $\kappa=4$, each fixed positive point has $T=\infty$. Thus $\mathbb P(T(x)=T(y))=1$ if equality of extended times is allowed, but there is no finite simultaneous-swallowing assertion there. The preceding formulas assume $\kappa>4$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
