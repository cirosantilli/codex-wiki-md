<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let a dot denote differentiation with respect to an affine [geodesic](../../../../../geodesic.md) parameter $s$. The five-dimensional [geodesic Lagrangian](../../../../../geodesic-lagrangian.md) is

$$
L=\frac12\gamma_{ij}\dot x^i\dot x^j+\frac12(\dot z+A_i\dot x^i)^2.
$$

Because $z$ is cyclic, its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) gives the conserved quantity

$$
\boxed{k=\frac{\partial L}{\partial\dot z}=\dot z+A_i\dot x^i,\qquad \dot k=0.}
$$

This is the conserved momentum per unit five-dimensional mass associated with the [Killing vector field](../../../../../killing-vector-field.md) $\partial_z$. For the other coordinates, differentiate $\partial L/\partial\dot x^i=\gamma_{ij}\dot x^j+kA_i$. Using $\dot k=0$ gives

$$
\frac{d}{ds}(\gamma_{ij}\dot x^j)-\frac12\partial_i\gamma_{jl}\dot x^j\dot x^l
+k(\partial_jA_i-\partial_iA_j)\dot x^j=0.
$$

The first two terms combine into $\gamma_{ij}(\ddot x^j+\Gamma^j{}_{lm}\dot x^l\dot x^m)$, with the [Christoffel symbols](../../../../../christoffel-symbol.md) of $\gamma$. Define the four-dimensional [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) $F_{ij}=\partial_iA_j-\partial_jA_i$ and raise its index with $\gamma$. The complete reduced [geodesic equations](../../../../../geodesic-equation.md) are

$$
\boxed{\frac{D\dot x^i}{ds}:=\ddot x^i+\Gamma^i{}_{jl}\dot x^j\dot x^l=kF^i{}_j\dot x^j,\qquad \dot z=k-A_i\dot x^i.}
$$

This is the [Kaluza-Klein geodesic Lorentz force](../../../../../kaluza-klein-geodesic-lorentz-force.md). The [Christoffel symbols](../../../../../christoffel-symbol.md) describe the gravitational motion in [general relativity](../../../../../general-relativity-split.md) in the four-dimensional [metric tensor](../../../../../metric-tensor.md), while the right-hand side is antisymmetric in its lowered indices and gives the [relativistic Lorentz force](../../../../../relativistic-lorentz-force.md). In particular,

$$
\frac{d}{ds}(\gamma_{ij}\dot x^i\dot x^j)=2kF_{ij}\dot x^i\dot x^j=0.
$$

Thus the force preserves the four-dimensional velocity norm, as a [Lorentz force](../../../../../lorentz-force.md) must. A particle with $k=0$ is neutral and follows an ordinary four-dimensional [geodesic](../../../../../geodesic.md). Nonzero compact momentum gives electric charge, with its sign determined by the direction of motion around the circle.

To identify the actual charge-to-mass ratio, suppose the five-dimensional particle has mass $M>0$ and $s$ is its five-dimensional [proper time](../../../../../proper-time.md), so $g_5(\dot X,\dot X)=-1$. Then $\gamma(\dot x,\dot x)=-(1+k^2)$. Four-dimensional [proper time](../../../../../proper-time.md) obeys $d\tau/ds=\sqrt{1+k^2}$; since $k$ is constant, $u^i=dx^i/d\tau$ satisfies

$$
\boxed{\frac{Du^i}{d\tau}=\frac{k}{\sqrt{1+k^2}}F^i{}_ju^j=\frac{q}{m}F^i{}_ju^j,\qquad
q=p_z=Mk,\qquad m=\sqrt{M^2+p_z^2}.}
$$

Here $q$ is in the geometric normalization of the supplied potential $A$. The relation $m^2=M^2+p_z^2$ also follows directly from the five-dimensional mass shell, and continues to identify the effective mass when the higher-dimensional particle is massless. The distinction between the two [proper times](../../../../../proper-time.md) prevents mistaking $k$ itself for the physical four-dimensional charge-to-mass ratio. A rescaling of $A$ to a canonically normalized electromagnetic potential correspondingly rescales $q$.

For the wave calculation, take a [scalar field](../../../../../scalar-field.md) of five-dimensional mass $M$ in units $\hbar=c=1$, obeying $(\Box_5-M^2)\Psi=0$. In the coordinate order $(x^i,z)$, direct inversion of the [metric tensor](../../../../../metric-tensor.md) gives

$$
g_5^{ij}=\gamma^{ij},\qquad g_5^{iz}=-A^i,\qquad g_5^{zz}=1+A_iA^i,\qquad \det g_5=\det\gamma.
$$

The determinant follows by the triangular change of coframe from $(dx^i,dz)$ to $(dx^i,dz+A_idx^i)$, whose determinant is one. Write $J=\sqrt{|\det\gamma|}$. Since all coefficients are $z$-independent, the scalar [covariant wave operator](../../../../../covariant-wave-operator.md) is

$$
\Box_5\Psi=J^{-1}(\partial_i-A_i\partial_z)\left[J\gamma^{ij}(\partial_j-A_j\partial_z)\Psi\right]+\partial_z^2\Psi.
$$

Expanding the right-hand side verifies both cross terms $-2A^i\partial_i\partial_z\Psi$, the term $-J^{-1}\partial_i(JA^i)\partial_z\Psi$, and the coefficient $1+A_iA^i$ of $\partial_z^2\Psi$.

Single-valuedness under the compact coordinate period requires the [Fourier series](../../../../../fourier-series-split.md)

$$
\Psi(x,z)=\sum_{n\in\mathbb Z}\psi_n(x)e^{inz/R}.
$$

For the $n$th [Kaluza-Klein mode](../../../../../kaluza-klein-mode.md), put $q_n=n/R$ and $D_i=\partial_i-iq_nA_i$. The five-dimensional [Klein-Gordon equation](../../../../../klein-gordon-equation.md) reduces to

$$
\boxed{\left[J^{-1}D_i\left(J\gamma^{ij}D_j\right)-m_n^2\right]\psi_n=0,\qquad
m_n^2=M^2+\frac{n^2}{R^2}.}
$$

This is the charged four-dimensional [Klein-Gordon equation](../../../../../klein-gordon-equation.md): the divergence expression includes both the spacetime connection and the gauge connection. Its interpretation as electric charge can also be checked directly. Under the fibre coordinate change $z'=z-\chi(x)$, the metric retains its form with $A'=A+d\chi$, and the scalar Fourier coefficient changes by $\psi'_n=e^{iq_n\chi}\psi_n$. Hence $D'_i\psi'_n=e^{iq_n\chi}D_i\psi_n$, exactly the transformation law for a field of charge $q_n$.

The [Kaluza-Klein charge quantization](../../../../../kaluza-klein-charge-quantization.md) is therefore

$$
\boxed{q_n=\frac nR,\qquad q_{\rm unit}=\frac1R\quad(\hbar=1).}
$$

Positive and negative integers give opposite charges, and the zero mode is neutral. Restoring $\hbar$ gives compact momenta $p_z=n\hbar/R$, so their fundamental spacing is $\hbar/R$. These are charges in the metric's geometric normalization. If $A_i=\kappa\mathcal A_i$ for a physically normalized electromagnetic potential $\mathcal A_i$, the physical charge unit is $\kappa/R$ in natural units, or $\kappa\hbar/R$ with $\hbar$ restored. Determining $\kappa$ requires an electromagnetic action normalization not specified by the metric ansatz alone.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
