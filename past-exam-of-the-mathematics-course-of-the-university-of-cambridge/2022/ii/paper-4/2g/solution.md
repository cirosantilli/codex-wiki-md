<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

For $t<1/2$, the number $f(t)$ is negative real, so the proposed identity would force

$$
\phi(t)\in(2\mathbb Z+1)\pi.
$$

Continuity on the connected interval $[0,1/2)$ makes $\phi$ equal to one fixed odd multiple of $\pi$ there. For $t>1/2$, the number $f(t)$ is positive real, so $\phi$ must instead equal one fixed even multiple of $\pi$. These two constants cannot agree, and their one-sided limits at $1/2$ therefore contradict continuity. The fact that $f(1/2)=0$ removes the phase condition at that one point but does not repair the discontinuity.

Now let $g:[0,1]\to\mathbb C\setminus\{0\}$ and put $h=g/|g|$. This is a continuous path in the [unit circle](../../../../../complex-unit-circle.md). The exponential map $\theta\mapsto e^{i\theta}$ is a [covering map](../../../../../covering-space.md), so the [path lifting theorem](../../../../../path-lifting-theorem.md) supplies a continuous lift $\theta:[0,1]\to\mathbb R$ after one value of $\theta(0)$ is chosen. Hence

$$
g(t)=|g(t)|e^{i\theta(t)}.
$$

One can obtain the same lift directly from the allowed special case: by uniform continuity, subdivide $[0,1]$ so that on each subinterval $h(t)/h(t_j)$ lies in the right half-plane, choose its continuous local argument there, and add a multiple of $2\pi$ to match the preceding endpoint.

If $\theta$ and $\widetilde\theta$ are two such phases, then

$$
\frac{\theta(t)-\widetilde\theta(t)}{2\pi}\in\mathbb Z.
$$

This integer-valued function is continuous and hence constant. Therefore

$$
r(g)=\theta(1)-\theta(0)
$$

does not depend on the chosen lift.

For $u(t)=g(t^2)$, the phase $\theta(t^2)$ gives

$$
\boxed{r(u)=r(g)}.
$$

For $v(t)=g(t)^2$, the phase $2\theta(t)$ gives

$$
\boxed{r(v)=2r(g)}.
$$

Finally, take

$$
g_1(t)=1,
\qquad
g_2(t)=e^{2\pi it}.
$$

They have the same two endpoints, but $r(g_1)=0$ and $r(g_2)=2\pi$. This endpoint discrepancy records the [winding number](../../../../../winding-number.md) of the closed path.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
