<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in a gas region with $\rho,p>0$ and physical adiabatic exponent $\gamma>1$. With $\xi=x/t$, each time derivative is $-\xi/t$ times differentiation in $\xi$, and each spatial derivative is $1/t$ times it. The [continuity equation](../../../../../../continuity-equation.md), [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) and the [entropy advection equation](../../../../../../entropy-advection-equation.md) for pressure reduce to

$$
(u-\xi)\rho'+\rho u'=0,\qquad (u-\xi)u'+p'/\rho=0,\qquad (u-\xi)p'+\gamma p u'=0.
$$

Their coefficient determinant is $(u-\xi)[(u-\xi)^2-c^2]$, where the [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md) is $c=\sqrt{\gamma p/\rho}$. If the determinant is nonzero, all derivatives vanish and the solution is uniform.

The apparent third characteristic $u=\xi$ does not give a smooth fan: on such an interval $u'=1$, whereas continuity requires $\rho u'=0$, impossible for $\rho>0$. It cannot support an isolated smooth [entropy](../../../../../../entropy.md) variation either. Subtracting $\gamma$ times the logarithmic density equation from the logarithmic [pressure](../../../../../../pressure.md) equation gives $(u-\xi)(\ln(p/\rho^\gamma))'=0$. A nonzero continuous [entropy](../../../../../../entropy.md) derivative would force $u=\xi$ on an interval and give the same contradiction. Thus the [specific entropy](../../../../../../specific-entropy.md) is constant throughout each smooth branch.

Every nonconstant branch therefore lies in one acoustic characteristic family. Let $\sigma=\pm1$ denote it, with $\xi=u+\sigma c$, so $u-\xi=-\sigma c$. The constant [entropy](../../../../../../entropy.md) means $p=K\rho^\gamma$, $K>0$, and $c'/c=(\gamma-1)\rho'/(2\rho)$. Continuity gives $u'=\sigma c\rho'/\rho=2\sigma c'/(\gamma-1)$. Differentiating $\xi=u+\sigma c$ then proves

$$
\boxed{u'=\frac2{\gamma+1},\qquad c'=\sigma\frac{\gamma-1}{\gamma+1},\qquad s=s_0+c_v\ln K=\text{constant}.}
$$

In particular, $u-2\sigma c/(\gamma-1)=J$ is a constant [Riemann invariant](../../../../../../riemann-invariant.md). All nonconstant smooth local solutions have the explicit form

$$
\boxed{u(\xi)=\frac{2\xi+(\gamma-1)J}{\gamma+1},\quad c(\xi)=\frac{\sigma(\gamma-1)(\xi-J)}{\gamma+1},\quad\rho=\left(\frac{c^2}{\gamma K}\right)^{1/(\gamma-1)},\quad p=K\rho^\gamma,}
$$

on an interval where $c>0$. Along the left-going family ($\sigma=-1$) sound speed decreases with $\xi$; along the right-going family ($\sigma=+1$) it increases. These are the two [self-similar ideal-gas rarefaction](../../../../../../self-similar-ideal-gas-rarefaction.md) branches. Together with arbitrary uniform positive states they exhaust the smooth local solutions. A global solution can join them piecewise at fan edges, where derivatives generally jump, and can also have discontinuities; those do not constitute additional smooth branches.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
