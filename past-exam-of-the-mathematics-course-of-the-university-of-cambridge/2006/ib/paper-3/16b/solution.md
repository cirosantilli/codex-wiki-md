<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

For a normalized state and an [observable](../../../../../observable.md) $A$, define $\langle A\rangle=\langle\psi,A\psi\rangle$ and $\Delta_\psi A=\|(A-\langle A\rangle)\psi\|$. Suppose first that the position and momentum [variances](../../../../../variance-split.md) are finite and the state has the regularity needed for the usual position-momentum quadratic forms. Put $a=\langle x\rangle$, $b=\langle p\rangle$, $u=(x-a)\psi$ and $v=(-i\hbar\partial_x-b)\psi$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
(\Delta_\psi x)^2(\Delta_\psi p)^2\ge|\langle u,v\rangle|^2\ge(\Im\langle u,v\rangle)^2.
$$

The term involving $b$ has zero imaginary part. Integration by parts gives

$$
2\Re\int_{\mathbb R}(x-a)\bar\psi\psi'\,dx
=\int_{\mathbb R}(x-a)(|\psi|^2)'\,dx=-1.
$$

Consequently $\Im\langle u,v\rangle=\hbar/2$, and

$$
\boxed{(\Delta_\psi x)(\Delta_\psi p)\ge\frac\hbar2.}
$$

This proves the [Heisenberg uncertainty relation](../../../../../heisenberg-uncertainty-relation.md). For smooth rapidly decaying states the boundary terms vanish directly. The same proof extends to $x\psi\in L^2$ and weak derivative $\psi'\in L^2$ using smooth cutoffs and taking their radius to infinity; the necessary mixed products are integrable by Cauchy-Schwarz. Normalization alone need not give finite [variances](../../../../../variance-split.md) or an operator-domain momentum expectation. A state with infinite spread is interpreted through the corresponding extended bound, rather than assigning a finite uncertainty to an undefined expression.

For the specified [Gaussian wave packet](../../../../../gaussian-wave-packet.md), write $s=\hbar t$ and $a_t=1+is$. Its [probability density](../../../../../probability-density.md) is

$$
|\psi(x,t)|^2=\frac1{\sqrt{2\pi}\sqrt{1+s^2}}
\exp\left[-\frac{x^2}{2(1+s^2)}\right].
$$

It is a normalized centered [normal distribution](../../../../../normal-distribution.md) with [variance](../../../../../variance-split.md) $1+s^2$. Symmetry gives $\langle x\rangle=0$, and hence

$$
\boxed{\Delta_\psi x=\sqrt{1+\hbar^2t^2}.}
$$

Also $\partial_x\psi=-x\psi/(2a_t)$, so $p\psi=i\hbar x\psi/(2a_t)$ and $\langle p\rangle=0$ by oddness. Integration by parts, or directly taking the squared norm, gives

$$
\langle p^2\rangle=\hbar^2\int|\psi'|^2\,dx
=\frac{\hbar^2}{4|a_t|^2}\langle x^2\rangle=\frac{\hbar^2}{4}.
$$

Thus

$$
\boxed{\Delta_\psi p=\frac\hbar2,\qquad
(\Delta_\psi x)(\Delta_\psi p)=\frac\hbar2\sqrt{1+\hbar^2t^2}\ge\frac\hbar2.}
$$

The packet saturates the bound at $t=0$ and has a larger position-momentum uncertainty product at every nonzero time. Its spatial spreading does not change the momentum distribution.

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
