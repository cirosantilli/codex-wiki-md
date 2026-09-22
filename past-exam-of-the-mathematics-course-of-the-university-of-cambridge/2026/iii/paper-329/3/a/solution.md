<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $y$ measure distance normal to the plane. The normal momentum balance and capillary pressure condition give

$$
p=\rho g\cos\theta\,(h-y)-\gamma h_{xx},
\qquad
p_x=\rho g\cos\theta\,h_x-\gamma h_{xxx}.
$$

The downslope lubrication equation is

$$
\mu u_{yy}=p_x-\rho g\sin\theta.
$$

Apply no slip $u(0)=-U$ and zero tangential stress $u_y(h)=0$. Integration gives the flux

$$
q=-Uh+\frac{h^3}{3\mu}
\left(\rho g\sin\theta-
ho g\cos\theta\,h_x+\gamma h_{xxx}\right).
$$

The [thin-film equation](../../../../../../thin-film-equation.md) $h_t+q_x=0$ is therefore

$$
\boxed{
h_t-Uh_x+\frac{\rho g\sin\theta}{3\mu}(h^3)_x
=\frac1{3\mu}\frac\partial{\partial x}
\left[h^3\left(\rho g\cos\theta\,h_x-\gamma h_{xxx}\right)\right]}.
$$

Long-wave information near a uniform film propagates with the kinematic speed

$$
c=q'(h_0)=-U+\frac{\rho g h_0^2\sin\theta}{\mu}.
$$

When $c>0$, disturbances travel from $x=-\infty$ into the domain, so $h\to h_0$ is an admissible upstream boundary condition. When $c<0$, information travels toward $x=-\infty$ from the pool, so the same condition cannot independently be imposed there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
