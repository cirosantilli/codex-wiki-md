<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put the anticommuting parameter on the left and write $\delta\Phi=\epsilon s\Phi$. Then $s$ is a [left-acting BRST differential](../../../../../../left-acting-brst-differential.md): it is odd and satisfies the graded product rule $s(UV)=(sU)V+(-1)^{|U|}U(sV)$. The [Faddeev-Popov ghost field](../../../../../../faddeev-popov-ghost.md) $c$ and [antighost field](../../../../../../faddeev-popov-antighost-field.md) $b$ are odd, whereas $A_\mu$ and the [Nakanishi-Lautrup field](../../../../../../nakanishi-lautrup-field.md) $h$ are even. Use $sA_\mu=D_\mu c$, $sc=-[c,c]/2$, $sb=h$, $sh=0$.

A total derivative in the Lagrangian variation must be included in the [Noether current](../../../../../../noether-current.md). For constant $\epsilon$, the ghost covariant derivative has $s(D_\mu c)=0$, by the [Jacobi identity](../../../../../../jacobi-identity.md) and the odd statistics of $c$. The Yang-Mills term is invariant, and the remaining variation is

$$
\delta\mathcal L=\epsilon\left[(\partial^\mu h^a)(D_\mu c)^a+h^a\partial^\mu(D_\mu c)^a\right]
=\epsilon\partial_\mu K^\mu,\qquad K^\mu=h^a(D^\mu c)^a.
$$

The term proportional to $\xi$ does not vary because $sh=0$.

To obtain the signs without an ambiguity about fermionic canonical momenta, now allow $\epsilon=\epsilon(x)$. In particular,

$$
\delta(D_\mu c)^a=-\frac12(\partial_\mu\epsilon)f^a{}_{bc}c^bc^c.
$$

The coefficients of $\partial_\mu\epsilon$ in the Yang-Mills, ghost, and multiplier terms are respectively

$$
-\frac1{g^2}F^{\mu\nu a}(D_\nu c)^a,\qquad
h^a(D^\mu c)^a+\frac12(\partial^\mu b^a)f^a{}_{bc}c^bc^c,\qquad
h^a(D^\mu c)^a.
$$

The positive sign of the last ghost expression results from moving $\partial_\mu\epsilon$ past the odd $\partial^\mu b^a$. Subtracting the total-derivative term $K^\mu$ therefore gives the [Yang-Mills BRST Noether current](../../../../../../yang-mills-brst-noether-current.md)

$$
\boxed{j_{\mathrm{BRST}}^\mu=-\frac1{g^2}F^{\mu\nu a}(D_\nu c)^a+h^a(D^\mu c)^a+\frac12(\partial^\mu b^a)f^a{}_{bc}c^bc^c.}
$$

Indeed, the full localized variation is $\delta\mathcal L=(\partial_\mu\epsilon)j^\mu+\partial_\mu(\epsilon K^\mu)$. The [Noether theorem](../../../../../../noether-theorem.md) then gives $\partial_\mu j^\mu=0$ on the field equations. With spatial boundary terms vanishing, the corresponding [BRST charge](../../../../../../brst-charge.md) in four spacetime dimensions is

$$
\boxed{Q_{\mathrm{BRST}}=\int d^3\mathbf x\left[-\frac1{g^2}F^{0\nu a}(D_\nu c)^a+h^a(D^0c)^a+\frac12(\partial^0b^a)f^a{}_{bc}c^bc^c\right].}
$$

It is odd and has ghost number one. Overall generator phases depend on the convention relating this [Noether charge](../../../../../../noether-charge.md) to quantum commutators; one may use $s\mathcal O=i[Q_{\mathrm{BRST}},\mathcal O\}$. The displayed current fixes the classical Noether normalization for the left-parameter convention.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
