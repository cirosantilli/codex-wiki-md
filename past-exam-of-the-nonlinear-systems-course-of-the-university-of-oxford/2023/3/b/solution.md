<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the real [logistic map](../../../../logistic-map.md), $f(x)=x$ factors as

$$
x\bigl(\mu-1-\mu x\bigr)=0.
$$

There is always the [fixed point](../../../../fixed-point.md) $x_0=0$. If $\mu\ne0$ there is also $x_*=1-1/\mu$, distinct from zero unless $\mu=1$. At $\mu=0$ the map is constant and zero is its only [fixed point](../../../../fixed-point.md). Negative $\mu$ must be retained because the paper specifies $x\in\mathbb R$.

Since $f'(x)=\mu(1-2x)$, the [fixed-point multipliers](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) are

$$
\lambda_0=\mu,\qquad \lambda_*=2-\mu.
$$

The [fixed point stability for an iteration](../../../../fixed-point-stability-for-an-iteration.md) criterion gives **$x_0$ attracting for $-1<\mu<1$, and $x_*$ attracting for $1<\mu<3$**. The respective [fixed points](../../../../fixed-point.md) are repelling when $|\mu|>1$ and $|2-\mu|>1$. At the unit-modulus boundaries the linear criterion needs a nonlinear supplement.

At $\mu=1$, the two [fixed point](../../../../fixed-point.md) branches meet and exchange stability: this is a [transcritical bifurcation](../../../../transcritical-bifurcation.md). Explicitly, with $\delta=\mu-1$,

$$
f(x)-x=\delta x-(1+\delta)x^2,
$$

which has the required nonzero parameter and quadratic terms. At the critical value itself, $f(x)=x-x^2$ attracts small positive points and pushes negative points away, so the merged [fixed point](../../../../fixed-point.md) is not stable from both sides.

At $\mu=-1$ the origin’s [fixed-point multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) crosses $-1$, while at $\mu=3$ the nonzero [fixed-point multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) crosses $-1$. Both are [period-doubling bifurcations](../../../../period-doubling-bifurcation.md). To check existence and stability of the new [periodic orbit](../../../../periodic-orbit.md), factor the second [iteration of a map](../../../../iterated-function.md):

$$
f^2(x)-x=-x(\mu x-\mu+1)
\left(\mu^2x^2-\mu(\mu+1)x+\mu+1\right).
$$

The two non-fixed roots are

$$
q_\pm=\frac{\mu+1\pm\sqrt{(\mu-3)(\mu+1)}}{2\mu}.
$$

They form a real [period-two orbit](../../../../period-two-orbit.md) for $\mu<-1$ or $\mu>3$. Its [periodic-orbit multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is

$$
f'(q_-)f'(q_+)=4+2\mu-\mu^2.
$$

It is less than one in [absolute value](../../../../absolute-value.md) just below $-1$ and just above $3$, respectively. Thus these are [supercritical bifurcations](../../../../supercritical-bifurcation.md) in the direction where the parent [fixed point](../../../../fixed-point.md) loses stability. At the critical values the [fixed points](../../../../fixed-point.md) themselves are weakly attracting: at $\mu=-1$, $f^2(x)=x-2x^3+x^4$; at $\mu=3$, setting $u=x-2/3$ gives $u\mapsto u-18u^3-27u^4$ after two steps. Both shrink sufficiently small nonzero [absolute values](../../../../absolute-value.md). The [bifurcation](../../../../bifurcation.md) values for finite [fixed points](../../../../fixed-point.md) are therefore

$$
\boxed{\mu=-1\text{ (period doubling)},\quad1\text{ (transcritical)},\quad3\text{ (period doubling)}.}
$$

The disappearance of the formula for $x_*$ at $\mu=0$ corresponds to that branch going to infinity, not a local [bifurcation](../../../../bifurcation.md) at a finite [fixed point](../../../../fixed-point.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the nonlinear systems course of the University of Oxford](../../../split.md)
5. [Nonlinear systems course of the University of Oxford](../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
