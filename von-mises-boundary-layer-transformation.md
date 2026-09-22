# Von Mises boundary-layer transformation

↑ **Parent:** [Boundary layer](boundary-layer.md)

In an attached two-dimensional [boundary layer](boundary-layer.md) with zero pressure gradient, use the [stream function](stream-function.md) $\Psi$ as transverse coordinate, assuming $\Psi_Y=u>0$ away from the wall. If $u=U(x,\Psi)$ and $\Psi_x=-V$, the chain rule gives $u_x=U_x-VU_\Psi$, $u_Y=UU_\Psi$ and $u_{YY}=U(UU_\Psi)_\Psi$. Substitution into $uu_x+Vu_Y=u_{YY}$ proves the displayed degenerate nonlinear diffusion equation. Its flat-plate similarity form $U=g(\Psi/\sqrt x)$ obeys $(gg')'+\eta g'/2=0$, $g(0)=0$, $g(\infty)=1$.

The wall coordinate is singular: finite physical shear corresponds to $g\sim C\sqrt\eta$, rather than a finite transformed derivative. A monotone profile exists by putting $q=gg'$, $q(0)=a>0$. Then $q'/q=-\eta/(2g)$ and $(g^2)'=2q$. Since $q\leq a$, $g\leq\sqrt{2a\eta}$; this forces $q$ to decay at least as $\exp[-c\eta^{3/2}]$. Thus $g$ has a finite positive limit, which can be normalized to one by $g(\eta)\mapsto A g(\eta/\sqrt A)$.

## ↑ Ancestors (5)

1. [Boundary layer](boundary-layer.md)
2. [Continuum mechanics](continuum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-theoretical-mechanics-course-of-the-university-of-oxford/2009/a/2/b/solution.md)
