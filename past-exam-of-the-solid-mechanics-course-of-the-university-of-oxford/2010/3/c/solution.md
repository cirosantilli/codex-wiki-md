<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a differentiable [crack](../../../../crack-in-a-solid.md) path, the local quasistatic Griffith laws with constant positive toughness are

$$
\boxed{\dot\ell(t)\geq0,\qquad
G(\ell(t),t)\leq G_c,\qquad
\dot\ell(t)[G_c-G(\ell(t),t)]=0.}
$$

They express irreversibility, local stability, and energy balance during growth. A strictly subcritical release rate forces the [crack](../../../../crack-in-a-solid.md) to stop.

Fix a [crack](../../../../crack-in-a-solid.md) parameter $s$ and let $u(s,t)$ denote the equilibrium [displacement](../../../../displacement.md) with the prescribed time-dependent loads. The scalar equilibrium problem is linear and has a unique solution for its fixed Dirichlet data. Both body force and boundary [displacement](../../../../displacement.md) scale by $t$, so

$$
\boxed{u(s,t)=t\,u(s,1).}
$$

The minimized potential energy is quadratic under this scaling: the strain term scales by $t^2$ and so does the load term $-f(t)u(s,t)$. Hence $E(s,t)=t^2E(s,1)$ and

$$
\boxed{G(s,t)=t^2G(s,1).}
$$

Equivalently the [crack](../../../../crack-in-a-solid.md)-tip coefficient scales by $t$ and its squared energy-release formula gives the same result.

Put $s_0=\ell(0)$. Finiteness and [continuity](../../../../continuous-function.md) of $G(s,1)$ make it bounded by some finite $M\geq0$ on a neighborhood of $s_0$. [Continuity](../../../../continuous-function.md) of $\ell$ supplies a positive interval on which $\ell(t)$ stays in that neighborhood. Shorten it to $[0,t_0]$ so that $t_0^2M<G_c$. Then $G(\ell(t),t)\leq t_0^2M<G_c$, and complementarity forces $\dot\ell(t)=0$ throughout. Therefore

$$
\boxed{\ell(t)=\ell(0)\quad(0\leq t\leq t_0).}
$$

No differentiating an unknown [crack](../../../../crack-in-a-solid.md) path or assuming its length already constant is needed; its [continuity](../../../../continuous-function.md) first gives the local release-rate bound.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
