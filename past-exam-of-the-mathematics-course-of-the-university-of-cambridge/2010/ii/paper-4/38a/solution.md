<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

For one-dimensional isentropic [compressible flow](../../../../../compressible-flow-split.md), [continuity](../../../../../continuous-function.md) and momentum balance are

$$
\rho_t+u\rho_x+\rho u_x=0,\qquad
u_t+uu_x+\frac{c^2}{\rho}\rho_x=0,\qquad c^2=\frac{dp}{d\rho}.
$$

Set $Q(\rho)=\int_{\rho_0}^{\rho}c(s)\,ds/s$. Combining the equations gives the [Riemann invariants](../../../../../riemann-invariant.md)

$$
\boxed{[\partial_t+(u\pm c)\partial_x](u\pm Q)=0.}
$$

For the power-law [equation of state](../../../../../equation-of-state.md), $c=c_0(\rho/\rho_0)^{(\gamma-1)/2}$ and direct integration gives $Q=2(c-c_0)/(\gamma-1)$.

In the expansion into the region left of the undisturbed gas, the invariant $u-Q$ remains zero. Hence $c=c_0+(\gamma-1)u/2$. In the centred simple wave, the other characteristic speed equals $\xi=x/t=u+c$, giving

$$
u=\frac{2(\xi-c_0)}{\gamma+1},\qquad
c=\frac{2c_0+(\gamma-1)\xi}{\gamma+1}.
$$

When the gas follows the piston, $u=-V$ at the piston and $c_p=c_0-(\gamma-1)V/2$. This requires $V<2c_0/(\gamma-1)$ for positive density. The three gas regions are

$$
\boxed{(u,c)=
\begin{cases}
(-V,c_p),&-Vt\le x\le[c_0-(\gamma+1)V/2]t,\\
\left(\dfrac{2(x/t-c_0)}{\gamma+1},
\dfrac{2c_0+(\gamma-1)x/t}{\gamma+1}\right),
&[c_0-(\gamma+1)V/2]t\le x\le c_0t,\\
(0,c_0),&x\ge c_0t.
\end{cases}}
$$

At the threshold the uniform region collapses. If $V$ exceeds the threshold, a vacuum gap separates the piston from the gas, whose free edge moves at $-2c_0/(\gamma-1)$.

A particle initially at $x_0>0$ stays at rest until the fan head arrives at $t_0=x_0/c_0$. Afterwards it lies in the fan and satisfies

$$
\frac{dx}{dt}=\frac2{\gamma+1}\left(\frac xt-c_0\right).
$$

Multiplication by $t^{-2/(\gamma+1)}$ and integration give $x=Ct^{2/(\gamma+1)}-2c_0t/(\gamma-1)$. Matching $x(t_0)=x_0$ determines $C$, yielding

$$
\boxed{x(t)=\frac{\gamma+1}{\gamma-1}x_0
\left(\frac{c_0t}{x_0}\right)^{2/(\gamma+1)}
-\frac{2c_0t}{\gamma-1}.}
$$

Since $2/(\gamma+1)<1$, differentiating proves

$$
\boxed{\dot x(t)\longrightarrow-\frac{2c_0}{\gamma-1}.}
$$

Thus each fixed particle approaches the velocity of the vacuum edge.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
