<h1 id="32a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
U(x)=\frac{x^2}{(1+x^2)^2},
\qquad
E(x,y)=\frac12y^2+U(x).
$$

The stated identity gives

$$
U'(x)=\frac{2x(1-x^2)}{(1+x^2)^3}.
$$

Hence, along the system,

$$
\begin{aligned}
\dot E
&=y\dot y+U'(x)\dot x\\
&=y[-U'(x)-ky]+U'(x)y\\
&=-ky^2\leq0.
\end{aligned}
$$

Near the origin, $E$ is positive definite because $U(x)>0$ for $x\ne0$. The [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) therefore gives stability.

Choose a sufficiently small compact [invariant sublevel set](../../../../../../invariant-sublevel-set.md)

$$
\Omega_c=\{(x,y):E(x,y)\leq c\},
\qquad 0<c<\frac14.
$$

On $\{\dot E=0\}$ we have $y=0$. A trajectory can remain there only if

$$
\dot y=-U'(x)=0,
$$

which occurs at $x=0,\pm1$. The choice $c<1/4=U(\pm1)$ excludes the two latter points, so the largest invariant subset of $\{\dot E=0\}\cap\Omega_c$ is the origin. [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) now gives convergence to the origin. Thus, for every $k>0$,

$$
\boxed{(0,0)\text{ is asymptotically stable}.}
$$

This is an instance of [damped mechanical energy as a Lyapunov function](../../../../../../damped-mechanical-energy-as-a-lyapunov-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
