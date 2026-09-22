<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the usual canonical [scalar field theory](../../../../../scalar-field-theory-split.md), subtract the vacuum energy so that the potential $U$ is nonnegative, and write the static energy in $d$ space dimensions as

$$
E[\phi]=T+W,\qquad
T=\frac12\int_{\mathbb R^d}|\nabla\phi|^2,\qquad
W=\int_{\mathbb R^d}U(\phi).
$$

Assume finite energy and sufficient decay to justify the scaling variation, with a fixed vacuum at infinity. Under [Derrick scaling](../../../../../derrick-scaling.md) $\phi_\lambda(x)=\phi(\lambda x)$,

$$
E[\phi_\lambda]=\lambda^{2-d}T+\lambda^{-d}W.
$$

A static solution must be stationary under this admissible variation. Thus the [Derrick virial identity](../../../../../derrick-virial-identity.md) is

$$
(2-d)T-dW=0.
$$

For $d\ge3$ both terms are nonpositive, and the coefficient of $T$ is strictly negative. Therefore $T=W=0$: the field is a constant vacuum. This proves the [Derrick theorem](../../../../../derrick-s-theorem.md) under its hypotheses. Negative potentials, additional derivative terms, gauge fields or time dependence can invalidate this particular obstruction; it is not a theorem about arbitrary energy functionals.

A [non-topological soliton](../../../../../non-topological-soliton.md) can instead be supported by a conserved ordinary [Noether charge](../../../../../noether-charge.md). For a [complex scalar field](../../../../../complex-scalar-field.md) with global $U(1)$ invariance, take $\phi=e^{i\omega t}f(x)$ and let $I=\int f^2$. In the normalization with kinetic density $|\partial\phi|^2/2$, its charge is $Q=\omega I$. At fixed charge, eliminating $\omega$ gives

$$
E_Q[f]=\frac12\int|\nabla f|^2+\int U(f)+\frac{Q^2}{2I}.
$$

The [charge-constrained scalar-field scaling](../../../../../charge-constrained-scalar-field-scaling.md) now reads

$$
E_Q[f_\lambda]=\lambda^{2-d}T+\lambda^{-d}W+\lambda^d\frac{Q^2}{2I}.
$$

The positive scaling power of the charge term can balance the others even for $d\ge3$. Such a [Q-ball](../../../../../q-ball.md) is time-dependent although its energy density is stationary, and the fixed-charge variational problem is different from the static one.

Suitable potentials permit this mechanism in any spatial dimension. For example, suppose $U(f)>0$ for $f\ne0$ and the ratio below attains a strictly positive minimum:

$$
0<\omega_0^2:=\min_{f>0}\frac{2U(f)}{f^2}<U''(0)=m^2
$$

Such a potential can favor a large region of nearly constant nonzero amplitude. At its preferred amplitude, the bulk terms minimize at $I\approx |Q|/\omega_0$, with energy about $\omega_0|Q|$. A wall has surface energy of order $|Q|^{(d-1)/d}$, lower order than the bulk term for every fixed $d\ge1$. For large charge the energy can therefore be below the free-particle threshold $m|Q|$. This explains how a localized fixed-charge solution may exist and resist dispersal. Existence and stability still require a suitable potential and charge range; not every complex-field theory or every member of a rotating family is a constrained minimum.

For the particular one-dimensional profile, substituting the rotating field into the equation gives

$$
f''=(1-\omega^2)f-f^3.
$$

Multiplying by $f'$ shows that

$$
\frac d{dx}\left[\frac12(f')^2-\frac12(1-\omega^2)f^2+\frac14f^4\right]=0.
$$

Both $f$ and $f'$ vanish at infinity, so the integration constant is zero. Hence

$$
\boxed{(f')^2=(1-\omega^2)f^2-\frac12f^4.}
$$

Here $U(f)=f^2/2-f^4/4$. This potential is not globally bounded below; the existence of the displayed localized solutions alone does not prove their nonlinear stability.

Use metric signature $(+,-)$ and set

$$
\gamma=(1-v^2)^{-1/2},\qquad
\xi=\gamma(x-x_0-vt),\qquad
\tau=\gamma(t-v(x-x_0)).
$$

The [Lorentz boost of a Q-ball](../../../../../lorentz-boost-of-a-q-ball.md) gives

$$
\boxed{\phi_v(t,x)=e^{i\omega\tau}f(\xi),\qquad |v|<1.}
$$

The peak follows $x=x_0+vt$. Because the equation is Lorentz invariant and the field is a scalar, this is again a solution.

The [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md) gives the energy and signed physical momentum at fixed time:

$$
E=\int_{\mathbb R}\left[\frac12|\phi_t|^2+
\frac12|\phi_x|^2+\frac12|\phi|^2-\frac14|\phi|^4\right]dx,
\qquad
P=-\int_{\mathbb R}\operatorname{Re}(\overline{\phi_t}\phi_x)\,dx.
$$

The minus sign agrees with the [scalar-field momentum flux](../../../../../scalar-field-momentum-flux.md) in the chosen signature. For the boosted field,

$$
|\phi_t|^2=\gamma^2[\omega^2f^2+v^2(f')^2],\qquad
|\phi_x|^2=\gamma^2[(f')^2+v^2\omega^2f^2],
$$

and

$$
-\operatorname{Re}(\overline{\phi_t}\phi_x)
=\gamma^2v[(f')^2+\omega^2f^2].
$$

The first integral gives $U(f)=\tfrac12[(f')^2+\omega^2f^2]$. Changing variable to $\xi$, so $dx=d\xi/\gamma$, yields

$$
E=\frac{\gamma^2(1+v^2)+1}{2\gamma}
\int_{\mathbb R}[(f')^2+\omega^2f^2]\,d\xi
=\gamma M,\qquad P=\gamma vM.
$$

Thus the rest-energy normalization and the [relativistic energy-momentum relation](../../../../../energy-momentum-relation.md) are

$$
\boxed{M=\int_{\mathbb R}[(f')^2+\omega^2f^2]\,dx,\qquad
E^2-P^2=M^2.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
