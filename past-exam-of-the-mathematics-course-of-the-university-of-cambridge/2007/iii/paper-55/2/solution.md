<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the canonical [chiral-superfield component expansion](../../../../../chiral-superfield-component-expansion.md) $\Phi=\phi+\sqrt2\theta\psi+\theta\theta F$ in chiral coordinates, with $\psi\psi=\psi^\alpha\psi_\alpha$. Multiplication of the [Grassmann variables](../../../../../grassmann-variable.md) gives

$$
[\Phi^2]_{\theta\theta}=2\phi F-\psi\psi,\qquad [\Phi^3]_{\theta\theta}=3\phi^2F-3\phi\psi\psi.
$$

For example, the two linear-in-$\theta$ factors in $\Phi^2$ contribute $-\theta\theta\psi\psi$, while each of the three choices of the remaining scalar in $\Phi^3$ gives the same contribution. Thus the required [F-term](../../../../../f-term.md) is

$$
\boxed{[W]_{\theta\theta}=(m\phi+g\phi^2)F-\frac12(m+2g\phi)\psi\psi.}
$$

Adding its Hermitian conjugate and the canonical $F^*F$ term eliminates the [auxiliary field](../../../../../auxiliary-field.md) through $F=-\overline{m\phi+g\phi^2}$ and yields the [F-term scalar potential](../../../../../f-term-scalar-potential.md)

$$
V=|m\phi+g\phi^2|^2=|\phi|^2|m+g\phi|^2.
$$

It is nonnegative, and for $g\ne0$ its absolute minima are **$\phi=0$ and $\phi=-m/g$**, each with zero energy. They coincide when $m=0$. If $g=0,m\ne0$, only $\phi=0$ is a minimum; if $g=m=0$, every $\phi$ is a minimum. These exhaust the local minima as well: at any other [stationary point](../../../../../stationary-point.md) $V_{\phi}=W''\overline{W'}=0$ forces $W''=0$; for $mg\ne0$ this is $\phi=-m/(2g)$, whose quadratic variation has opposite signs in two real directions and is a saddle.

Expand around $\phi=0$, writing $\phi=h=(h_1+ih_2)/\sqrt2$. The [scalar potential](../../../../../scalar-potential.md) and fermionic terms are

$$
\begin{aligned}
V&=|m|^2|h|^2+m^*g\,h^2h^*+mg^*\,h(h^*)^2+|g|^2|h|^4,\\
\mathcal L_{\mathrm{fermion}}&\supset-\frac12m\psi\psi-g h\psi\psi+\mathrm{h.c.}
\end{aligned}
$$

The canonical [kinetic term](../../../../../kinetic-term.md) is $\frac12[(\partial h_1)^2+(\partial h_2)^2]$. Its quadratic potential is $\frac12|m|^2(h_1^2+h_2^2)$, while the [Weyl fermion](../../../../../weyl-spinor.md) has mass $|m|$. Hence

$$
\boxed{m_{h_1}=m_{h_2}=m_\psi=|m|.}
$$

At the other minimum, $W''=-m$, so the same mass equality holds. The quartic and [Yukawa interaction](../../../../../yukawa-interaction.md) are both fixed by $g$: defining $V\supset\lambda|h|^4$ and $\mathcal L\supset-yh\psi\psi+\mathrm{h.c.}$ gives

$$
\boxed{y=g,\qquad\lambda=|g|^2=|y|^2.}
$$

This is the [supersymmetric relation between quartic and Yukawa couplings](../../../../../supersymmetric-relation-between-quartic-and-yukawa-couplings.md). The printed equality of the two couplings refers to their common supersymmetric origin; literal equality of the conventional coefficients $\lambda$ and $y$ is not true for arbitrary $g$. If instead the Yukawa term is defined as $-\frac12yh\psi\psi$, then $y=2g$ and $\lambda=|y|^2/4$.

To establish perturbative [superpotential non-renormalization](../../../../../non-renormalization-theorem.md), use a [Wilsonian effective action](../../../../../wilsonian-effective-action.md) with a fixed positive infrared cutoff, so integrating out modes does not introduce massless infrared singularities. Promote $m,g$ to nondynamical [chiral superfields](../../../../../chiral-superfield.md), or [spurions](../../../../../spurion.md). The [holomorphic superpotential](../../../../../superpotential.md) depends holomorphically on $\Phi,m,g$, not on their complex conjugates. Assign an ordinary $U(1)$ charge and an [R-charge](../../../../../r-charge.md) by

$$
\begin{array}{c|ccc}
&\Phi&m&g\\\hline
q&1&-2&-3\\
R&1&0&-1
\end{array}.
$$

The [superspace](../../../../../superspace.md) coordinate has $R(\theta)=1$, so $d^2\theta$ has charge $-2$ and $W$ must have [R-charge](../../../../../r-charge.md) $2$. Both original monomials satisfy the two selection rules. A [holomorphic](../../../../../complex-differentiability-at-a-point.md) perturbative monomial $m^ag^b\Phi^c$ must obey

$$
-2a-3b+c=0,\qquad-b+c=2,
$$

which gives $c=b+2$ and $a=1-b$. Equivalently,

$$
W_{\mathrm{eff}}=m\Phi^2f(g\Phi/m),\qquad W_{\mathrm{eff}}^{\mathrm{pert}}=\sum_{b\geq0}c_b\,g^b m^{1-b}\Phi^{b+2}.
$$

The nonnegative integer $b$ follows from perturbative analyticity in $g$. Regularity as $m\to0$ at the fixed Wilsonian cutoff excludes $b\geq2$, which would require negative powers of $m$. The remaining quadratic coefficient is fixed to $c_0=1/2$ by the free theory at $g=0$. The coefficient $c_1$ is $1/3$: a three-point contribution at first order in $g$ has just one cubic vertex, uses all three legs externally, and cannot contain a loop. A loop correction would require additional interactions, whereas the selection rules and [holomorphy](../../../../../holomorphic-function.md) have already excluded the corresponding monomials. Therefore

$$
\boxed{W_{\mathrm{eff}}^{\mathrm{pert}}=\frac12m\Phi^2+\frac13g\Phi^3.}
$$

This proof concerns the local Wilsonian [superpotential](../../../../../superpotential.md). The [Kähler potential](../../../../../kahler-potential.md) can acquire a wave-function factor $Z$, and canonical normalization changes the couplings to $m_c=m/Z$ and $g_c=g/Z^{3/2}$. Such running, and nonlocal infrared terms in a one-particle-irreducible action, do not contradict the [holomorphic](../../../../../complex-differentiability-at-a-point.md) result.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
