<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [fixed point](../../../../fixed-point.md) $x_*$ satisfies $f(x_*,\mu)=x_*$. A [perturbation](../../../../perturbation.md) obeys $u_{n+1}=m u_n+O(u_n^2)$, where the [periodic-orbit multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is $m=f_x(x_*,\mu)$. It is linearly [attracting](../../../../attraction-in-a-dynamical-system.md) for $|m|<1$ and [repelling](../../../../repulsion-in-a-dynamical-system.md) for $|m|>1$; at $m=\pm1$ nonlinear terms decide [Lyapunov stability](../../../../lyapunov-stability.md). A crossing through $+1$ can produce a saddle-node, transcritical or [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md), depending on the [mathematical model parameter](../../../../mathematical-model-parameter.md) dependence and [symmetry](../../../../symmetry-physics.md). A crossing through $-1$ generically gives a [period-doubling bifurcation](../../../../period-doubling-bifurcation.md). A real one-dimensional [function](../../../../function-split.md) cannot have the [complex conjugate](../../../../complex-conjugate.md) pair needed for a [Neimark–Sacker bifurcation](../../../../neimark-sacker-bifurcation.md).

For a genuine [period-two orbit](../../../../period-two-orbit.md), study the [return map](../../../../poincare-map.md) $f\circ f$ at either point. By the [chain rule](../../../../chain-rule.md) its [periodic-orbit multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is

$$
\boxed{m_2=f_x(x_1,\mu)f_x(x_2,\mu).}
$$

Its modulus determines [linear stability](../../../../linear-stability.md) by the same criterion, now per two [iterates](../../../../iterate.md).

For the [real quadratic iteration map](../../../../real-quadratic-iteration-map.md), the fixed-point equation gives

$$
x_\pm=\frac{-1\pm\sqrt{1+4\mu}}2,\qquad \mu\ge-\frac14.
$$

The [derivative](../../../../derivative.md) is $-2x$. The lower branch $x_-$ is [repelling](../../../../repulsion-in-a-dynamical-system.md) whenever $\mu>-1/4$. The upper branch satisfies $|-2x_+|<1$ exactly for

$$
\boxed{-\frac14<\mu<\frac34.}
$$

At $\mu=-1/4$ the two [fixed points](../../../../fixed-point.md) merge in a [saddle-node bifurcation](../../../../saddle-node-bifurcation.md). With $u=x+1/2$ at that [mathematical model parameter](../../../../mathematical-model-parameter.md), $u'=u-u^2$, so the point attracts from the right and is [repelling](../../../../repulsion-in-a-dynamical-system.md) from the left. At $\mu=3/4$, $x_+=1/2$ has [periodic-orbit multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) $-1$ and undergoes a [period-doubling bifurcation](../../../../period-doubling-bifurcation.md). At the threshold itself $u'= -u-u^2$ and the two-step return is $u''=u-2u^3-u^4$, proving weak [asymptotic stability](../../../../asymptotic-stability.md) there despite the inconclusive linear test.

Factor the second-iterate equation:

$$
f(f(x),\mu)-x=-(x^2+x-\mu)(x^2-x+1-\mu).
$$

Removing the fixed-point factor yields the [periodic orbit](../../../../periodic-orbit.md) points

$$
x_1=\frac{1-\sqrt{4\mu-3}}2,\qquad x_2=\frac{1+\sqrt{4\mu-3}}2.
$$

They are distinct and exchanged by $f$ exactly when $\mu>3/4$; at equality they coincide with the [fixed point](../../../../fixed-point.md). Their product is $1-\mu$, hence their [periodic-orbit multiplier](../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is $4(1-\mu)$. Thus

$$
\boxed{\text{the two-cycle exists for }\mu>\frac34,\quad\text{and is linearly attracting for }\frac34<\mu<\frac54.}
$$

It is [repelling](../../../../repulsion-in-a-dynamical-system.md) for $\mu>5/4$ and reaches its next [period-doubling bifurcation](../../../../period-doubling-bifurcation.md) threshold at $\mu=5/4$. At that exact endpoint it is weakly [attracting](../../../../attraction-in-a-dynamical-system.md): if $f^2$ is expanded about either [periodic orbit](../../../../periodic-orbit.md) point as $v'=-v+Av^2+Bv^3+O(v^4)$, then $A=2\mu-6x_i^2$, $B=-4x_i$, and $A^2+B=20\pm10\sqrt2>0$. Its second return is $v''=v-2(A^2+B)v^3+O(v^4)$.

At $\mu=2$ put $h(y)=4\sin^2(\pi y)-2=-2\cos(2\pi y)$. The double-angle identity gives

$$
f(h(y),2)=2-4\cos^2(2\pi y)=-2\cos(4\pi y)=h(2y\bmod1).
$$

This verifies the printed relation to the [Bernoulli shift](../../../../bernoulli-shift.md). Precisely, it is a [semiconjugacy](../../../../semiconjugacy-of-dynamical-systems.md): $h(y)=h(1-y)$, so it is not invertible on the circle. To obtain a genuine interval [topological conjugacy](../../../../topological-conjugacy.md), use the [homeomorphism](../../../../homeomorphism.md) $H(u)=-2\cos(\pi u)$ from $[0,1]$ onto $[-2,2]$, and the full [tent map](../../../../tent-map.md)

$$
T(u)=\begin{cases}2u,&0\le u\le1/2,\\2-2u,&1/2\le u\le1.\end{cases}
$$

The same identity proves $f(H(u),2)=H(T(u))$.

The full [tent map](../../../../tent-map.md) has [dense periodic points](../../../../dense-periodic-points.md), is [topologically mixing](../../../../topological-mixing.md) and has [sensitive dependence on initial conditions](../../../../butterfly-effect.md). To see these properties directly, its $n$th iterate has $2^n$ monotone branches on dyadic intervals of length $2^{-n}$, each mapping onto $[0,1]$. Every nonempty open interval contains such a branch domain, and a later iterate covers all of $[0,1]$, proving [topological mixing](../../../../topological-mixing.md). On any branch, the [function graph](../../../../graph-of-a-function.md) of the iterate has a [fixed point](../../../../fixed-point.md) by the [intermediate value theorem](../../../../intermediate-value-theorem.md), so [periodic points](../../../../periodic-point.md) occur in every open interval. Given any initial point and any neighborhood, some iterate of that neighborhood covers the interval; one can choose a nearby point whose image differs from the initial point's image by at least a fixed positive distance. This proves [sensitive dependence on initial conditions](../../../../butterfly-effect.md). [Uniform continuity](../../../../uniform-continuity.md) of the inverse [homeomorphism](../../../../homeomorphism.md) transfers these properties to $f$ on $[-2,2]$.

Consequently the [real quadratic iteration map](../../../../real-quadratic-iteration-map.md) is [chaotic](../../../../chaos.md) on its [invariant interval](../../../../invariant-interval.md) in the Devaney sense: **[topological transitivity](../../../../topological-transitivity.md), [dense periodic points](../../../../dense-periodic-points.md) and [sensitive dependence on initial conditions](../../../../butterfly-effect.md)**, with all these orbits bounded. There are also aperiodic orbits: [periodic points](../../../../periodic-point.md) form a countable union of finite sets of [roots of an equation](../../../../root-of-an-equation.md) of the equations $f^n(x)=x$, whereas the interval is uncountable. The [semiconjugacy](../../../../semiconjugacy-of-dynamical-systems.md) alone would not justify treating $h$ as invertible; the tent-map argument supplies the missing rigorous transfer.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../split.md)
5. [Topics in applied mathematics course of the University of Oxford](../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
