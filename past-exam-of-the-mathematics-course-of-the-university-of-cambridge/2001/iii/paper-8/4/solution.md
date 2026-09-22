<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For fixed $\operatorname{Im}\tau>0$, Gaussian decay of $|q|^{n^2}$ gives locally uniform convergence of the [theta function](../../../../../theta-function.md) series and all its $z$-derivatives. It is therefore entire. Shifting the series argument and reindexing gives

$$
\theta_3(z+\pi)=\theta_3(z),\qquad
\theta_3(z+\pi\tau)=q^{-1}e^{-2iz}\theta_3(z).
$$

Since $\theta_4(z)=\theta_3(z+\pi/2)$, the corresponding second multiplier for $\theta_4$ has the opposite sign:

$$
\theta_4(z+\pi)=\theta_4(z),\qquad
\theta_4(z+\pi\tau)=-q^{-1}e^{-2iz}\theta_4(z).
$$

Thus $h=\theta_3/\theta_4$ obeys $h(z+\pi)=h(z)$ and $h(z+\pi\tau)=-h(z)$. These give candidate [period lattices](../../../../../period-lattice.md); to show they are exact, first locate every zero.

At $z_*=(\pi+\pi\tau)/2$,

$$
\theta_3(z_*)=\sum_{n\in\mathbb Z}(-1)^nq^{n(n+1)}=0,
$$

because the terms with indices $n$ and $-n-1$ cancel. The absolute convergence justifies that pairing. Quasi-periodicity propagates this zero to every $z_*+m\pi+n\pi\tau$.

For exhaustiveness and simplicity, let $v=\theta_3'/\theta_3$. It satisfies $v(z+\pi)=v(z)$ and $v(z+\pi\tau)=v(z)-2i$. Take a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) for $\Lambda_0=\pi\mathbb Z+\pi\tau\mathbb Z$, translated so its boundary has no zero. The two sloping edges cancel by the first identity; the bottom and reversed top give

$$
\oint v(z)\,dz=\int_{z_0}^{z_0+\pi}\bigl(v(z)-v(z+\pi\tau)\bigr)dz=2\pi i.
$$

The [argument principle](../../../../../argument-principle.md) therefore counts one zero with multiplicity in every cell. Since a known zero class already exists, all zeros are simple and exactly

$$
\boxed{z=\frac\pi2+\frac{\pi\tau}{2}+m\pi+n\pi\tau,\qquad m,n\in\mathbb Z}.
$$

The denominator's simple zeros are instead $\pi\tau/2+\Lambda_0$. These two cosets are disjoint: $\pi/2$ cannot lie in $\Lambda_0$ because $\operatorname{Im}\tau>0$. Thus there are no cancelled zeros or [poles](../../../../../pole.md) in the quotient.

Any period of $h$ or $h^2$ must translate its [zero set](../../../../../zero-set.md) onto itself, so must belong to $\Lambda_0$. A translation $m\pi+n\pi\tau$ multiplies $h$ by $(-1)^n$; the quotient is nonconstant, so an odd $n$ cannot be a period of $h$. Squaring removes precisely that sign. This proves the [period lattice of theta3 over theta4](../../../../../period-lattice-of-theta3-over-theta4.md) and its squared counterpart:

$$
\boxed{\operatorname{Per}\left(\frac{\theta_3}{\theta_4}\right)=\pi\mathbb Z+2\pi\tau\mathbb Z},\qquad
\boxed{\operatorname{Per}\!\left[\left(\frac{\theta_3}{\theta_4}\right)^2\right]=\pi\mathbb Z+\pi\tau\mathbb Z}.
$$

The second lattice is for the squared function; no additional translation can preserve its [zero set](../../../../../zero-set.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
