<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Balance streamwise convection of order one with transverse viscous diffusion $Re^{-1}\partial_y^2u$. This requires a thickness $Re^{-1/2}$. Continuity then makes the normal [velocity](../../../../../velocity.md) of that same small order. Set

$$
\boxed{Y=Re^{1/2}y,\qquad V=Re^{1/2}v.}
$$

The normal momentum equation makes the leading [pressure](../../../../../pressure-split.md) independent of $Y$. It equals the outer [pressure](../../../../../pressure-split.md), whose inviscid tangential momentum balance gives $-p_x=U_sU_s'$. The leading tangential equation and continuity are consequently

$$
\boxed{uu_x+Vu_Y=U_sU_s'+u_{YY},\qquad u_x+V_Y=0.}
$$

The [divergence](../../../../../divergence.md)-free field $(u,V)$ has a [streamfunction](../../../../../stream-function.md) with $u=\Psi_Y$, $V=-\Psi_x$. Substituting yields

$$
\boxed{\Psi_Y\Psi_{xY}-\Psi_x\Psi_{YY}=U_sU_s'+\Psi_{YYY}.}
$$

The stationary impermeable wall has $u=V=0$, so $\Psi_Y(x,0)=0$ and $\Psi(x,0)$ is constant, chosen to be zero. Matching to the outer slip [velocity](../../../../../velocity.md) gives $\Psi_Y(x,\infty)=U_s(x)$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
