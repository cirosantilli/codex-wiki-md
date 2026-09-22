<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $|\uparrow\rangle,|\downarrow\rangle$ for the two $S_3$ [eigenstates](../../../../eigenstate.md), of [eigenvalues](../../../../eigenvalue.md) $\pm\hbar/2$. The [spin-spin interaction](../../../../spin-spin-interaction.md) can be evaluated using

$$
\mathbf S^{(1)}\cdot\mathbf S^{(2)}=S_3^{(1)}S_3^{(2)}+\frac12\left(S_+^{(1)}S_-^{(2)}+S_-^{(1)}S_+^{(2)}\right).
$$

For $|\beta|\gg|\alpha|$, take $H_0=\beta(S_3^{(1)}-S_3^{(2)})/\hbar$ and $V=\alpha\mathbf S^{(1)}\cdot\mathbf S^{(2)}/\hbar^2$. The unperturbed [energy eigenvalues](../../../../energy-eigenvalue-split.md) are $\beta,-\beta,0,0$ on $|\uparrow\downarrow\rangle,|\downarrow\uparrow\rangle,|\uparrow\uparrow\rangle,|\downarrow\downarrow\rangle$, respectively. For an isolated normalized [energy eigenstate](../../../../energy-eigenstate.md) $|n\rangle$, [first-order nondegenerate perturbation theory](../../../../first-order-nondegenerate-perturbation-theory.md) gives $\Delta E_n^{(1)}=\langle n|V|n\rangle$. The two antiparallel [spins](../../../../spin.md) have expectation $-\alpha/4$, so

$$
\boxed{E_{\uparrow\downarrow}=\beta-\frac\alpha4+O(\alpha^2/|\beta|),\qquad E_{\downarrow\uparrow}=-\beta-\frac\alpha4+O(\alpha^2/|\beta|).}
$$

For the zero-[energy](../../../../energy-split.md) [degenerate eigenspace](../../../../degenerate-eigenspace.md), [degenerate perturbation theory](../../../../degenerate-perturbation-theory.md) requires diagonalizing the restriction of $V$. On the ordered [basis](../../../../basis.md) $(|\uparrow\uparrow\rangle,|\downarrow\downarrow\rangle)$ it is $(\alpha/4)I$: the [ladder operators](../../../../ladder-operator.md) cannot take one parallel state to the other. Indeed neither parallel state couples to anything else under $H$, so **the remaining two levels are exactly $\alpha/4$**, retaining their twofold [quantum degeneracy](../../../../degenerate-energy-levels.md).

For $|\alpha|\gg|\beta|$, take $H_0=\alpha\mathbf S^{(1)}\cdot\mathbf S^{(2)}/\hbar^2$ and $V=\beta D$, where $D=(S_3^{(1)}-S_3^{(2)})/\hbar$. The [spin-one-half triplet state](../../../../spin-one-half-triplet-state.md) [basis](../../../../basis.md) and [spin-one-half singlet state](../../../../spin-one-half-singlet-state.md) are

$$
|t_+\rangle=|\uparrow\uparrow\rangle,\quad |t_0\rangle=\frac{|\uparrow\downarrow\rangle+|\downarrow\uparrow\rangle}{\sqrt2},\quad |t_-\rangle=|\downarrow\downarrow\rangle,\quad |s\rangle=\frac{|\uparrow\downarrow\rangle-|\downarrow\uparrow\rangle}{\sqrt2}.
$$

The identity $\mathbf S^{(1)}\cdot\mathbf S^{(2)}=(\mathbf J^2-3\hbar^2/2)/2$ gives unperturbed [energy eigenvalues](../../../../energy-eigenvalue-split.md) $E_t^{(0)}=\alpha/4$ and $E_s^{(0)}=-3\alpha/4$. Direct action gives

$$
D|t_\pm\rangle=0,\qquad D|t_0\rangle=|s\rangle,\qquad D|s\rangle=|t_0\rangle.
$$

Consequently the restriction of $V$ to the entire triplet [degenerate eigenspace](../../../../degenerate-eigenspace.md) is zero, so no first-order splitting is missed. The singlet expectation is also zero. In [second-order nondegenerate perturbation theory](../../../../second-order-nondegenerate-perturbation-theory.md), $\Delta E_n^{(2)}=\sum_{r\ne n}|\langle r|V|n\rangle|^2/(E_n^{(0)}-E_r^{(0)})$. Within the triplet, the corresponding second-order effective [matrix](../../../../matrix.md) is $\beta^2|t_0\rangle\langle t_0|/\alpha$, already diagonal in this [basis](../../../../basis.md). Thus, through second order,

$$
\boxed{E_{t_\pm}=\frac\alpha4,\qquad E_{t_0}=\frac\alpha4+\frac{\beta^2}{\alpha},\qquad E_s=-\frac{3\alpha}{4}-\frac{\beta^2}{\alpha}.}
$$

The last two expressions have higher corrections beginning at $O(\beta^4/|\alpha|^3)$, as the exact calculation in part (d) also verifies. For positive $\alpha$, coupling to the lower singlet raises the triplet's $M=0$ level and lowers the singlet; the signs are precisely the [energy](../../../../energy-split.md) denominators above.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
