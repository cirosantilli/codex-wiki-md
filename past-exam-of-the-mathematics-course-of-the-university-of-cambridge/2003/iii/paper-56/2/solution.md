<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use units $G=\hbar=c=k_B=1$ and put $\ell=\sqrt{3/\Lambda}$. The [static patch of de Sitter spacetime](../../../../../static-patch-of-de-sitter-spacetime.md) has radial factor $f=1-r^2/\ell^2$. A [Wick rotation](../../../../../wick-rotation.md) $t=-i\tau$ makes its radial-time metric positive:

$$
ds_E^2=f\,d\tau^2+\frac{dr^2}{f}+r^2d\Omega_2^2.
$$

Near the [cosmological horizon](../../../../../cosmological-horizon.md), write $r=\ell-\rho^2/(2\ell)$. Then $f=\rho^2/\ell^2+O(\rho^4)$ and

$$
ds_E^2=d\rho^2+\rho^2d(\tau/\ell)^2+\ell^2d\Omega_2^2+O(\rho^2)
$$

in the radial-time directions. Thus $\tau/\ell$ must be an angle of period $2\pi$. A larger integer multiple would give a conical excess rather than a smooth origin. The [Euclidean black-hole regularity condition](../../../../../euclidean-black-hole-regularity-condition.md) gives

$$
\boxed{\beta=2\pi\ell=2\pi\sqrt{3/\Lambda},\qquad T=\beta^{-1}=\frac1{2\pi}\sqrt{\Lambda/3}.}
$$

This [de Sitter horizon temperature](../../../../../de-sitter-horizon-temperature.md) uses the time normalization at $r=0$, where $t$ is [proper time](../../../../../proper-time.md); static observers at other radii see the corresponding [Tolman temperature law](../../../../../tolman-ehrenfest-relation.md) redshift.

Vary the gravitational [Euclidean action](../../../../../euclidean-action.md) with respect to $g^{ab}$. The identities $\delta\sqrt g=-\tfrac12\sqrt g\,g_{ab}\delta g^{ab}$ and the integrated variation of the [scalar curvature](../../../../../scalar-curvature.md) yield, after discarding the assumed boundary term,

$$
\delta I_E=-\frac1{16\pi}\int\sqrt g\,\left(R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}\right)\delta g^{ab}\,d^4x.
$$

The resulting vacuum [Einstein field equations](../../../../../einstein-field-equations.md) are therefore

$$
\boxed{R_{ab}-\frac12Rg_{ab}+\Lambda g_{ab}=0.}
$$

Tracing in four dimensions gives $R=4\Lambda$, and substitution gives $R_{ab}=\Lambda g_{ab}$.

The smooth Euclidean geometry is compact. Explicitly, in Euclidean five-space use

$$
X_0=\sqrt{\ell^2-r^2}\cos(\tau/\ell),\quad
X_1=\sqrt{\ell^2-r^2}\sin(\tau/\ell),\quad
(X_2,X_3,X_4)=r\,\mathbf n,\quad |\mathbf n|=1.
$$

These obey $\sum X_A^2=\ell^2$ and induce precisely the above metric, so $0\leq r\leq\ell$ with the identified Euclidean time covers a round four-sphere once. Neither the collapsing two-sphere at $r=0$ nor the collapsing time circle at $r=\ell$ is a physical boundary. Since $\sqrt g=r^2\sin\theta$, its volume and on-shell [Euclidean action](../../../../../euclidean-action.md) are

$$
\operatorname{Vol}=\beta\,4\pi\int_0^\ell r^2dr=\frac{8\pi^2\ell^4}{3}=\frac{24\pi^2}{\Lambda^2},
\qquad
\boxed{I_E=-\frac{2\Lambda}{16\pi}\operatorname{Vol}=-\frac{3\pi}{\Lambda}.}
$$

The semiclassical [partition function](../../../../../canonical-partition-function.md) is $Z\simeq e^{-I_E}$, and $I_E=\beta F=\beta E-S$ follows from the [free energy](../../../../../thermodynamic-free-energy.md) relation $F=E-TS$. With the stipulated zero internal energy,

$$
\boxed{S=-I_E=\frac{3\pi}{\Lambda}=\frac{A_H}{4},\qquad A_H=4\pi\ell^2.}
$$

Thus the [Euclidean de Sitter action and entropy](../../../../../euclidean-de-sitter-action-and-entropy.md) reproduce the [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md) of the [cosmological horizon](../../../../../cosmological-horizon.md) without a boundary contribution. Restoring constants, $S=k_Bc^3A_H/(4G\hbar)$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
