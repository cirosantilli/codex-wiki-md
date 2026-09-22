<h1 id="33a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $y=\dot x$. The first-order system is

$$
\dot x=y,
\qquad
\dot y=-2x(1-x^2)^2-\mu y.
$$

At an [equilibrium point of a dynamical system](../../../../../../equilibrium-point-of-a-dynamical-system.md), $y=0$ and $x(1-x^2)^2=0$, so the three fixed points are

$$
\boxed{(0,0),\ (1,0),\ (-1,0).}
$$

Define

$$
U(x)=x^2-x^4+\frac{x^6}{3},
\qquad
E(x,y)=\frac12y^2+U(x).
$$

Then $U'(x)=2x(1-x^2)^2=-F(x)$ and

$$
\dot E
=y\dot y+U'(x)\dot x
=-\mu y^2\leq0.
$$

Moreover,

$$
U(x)=x^2\left(1-x^2+\frac{x^4}{3}\right)>0
\quad(x\ne0),
$$

so $E$ is positive definite at the origin. It is therefore a [damped mechanical energy as a Lyapunov function](../../../../../../damped-mechanical-energy-as-a-lyapunov-function.md), and the [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) proves that the origin is Lyapunov stable.

Since $U(\pm1)=1/3$, choose a compact energy sublevel $\{E\leq c\}$ with $0<c<1/3$. In this set, $\dot E=0$ means $y=0$. A trajectory can remain in $y=0$ only when $F(x)=0$, and the chosen sublevel excludes $x=\pm1$. Thus the largest invariant subset of $\{\dot E=0\}$ is the origin. The [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) proves that the origin is asymptotically stable.

Finally, $E$ is radially unbounded because its leading terms are $x^6/3+y^2/2$. Every forward trajectory is therefore bounded. LaSalle's principle puts its [omega-limit set](../../../../../../omega-limit-set.md) inside

$$
\{(x,0):F(x)=0\}
=\{(-1,0),(0,0),(1,0)\}.
$$

An omega-limit set of a bounded continuous trajectory is nonempty and connected. A connected subset of this three-point set is a singleton, so every trajectory has precisely one of the three fixed points as its omega-limit set.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33A](../../33a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
