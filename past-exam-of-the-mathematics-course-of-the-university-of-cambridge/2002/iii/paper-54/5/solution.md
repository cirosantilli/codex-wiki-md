<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use fixed spatial coordinates in a stationary heterogeneous Earth and define the operator

$$
(\mathcal L u)_i=\rho(\mathbf x)\partial_t^2u_i
-\partial_{x_j}[c_{ijkl}(\mathbf x)\partial_{x_l}u_k].
$$

Here the [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md) has its minor and major symmetries, and the physical [body force](../../../../../body-force.md) per unit volume is $q_i=\rho f_i$. The retarded [elastodynamic Green tensor](../../../../../elastodynamic-green-tensor.md) $G_i^{\ j}(\mathbf x,\boldsymbol\xi,t)$ is the displacement in direction $i$ due to a unit physical force impulse in direction $j$ at $\boldsymbol\xi$:

$$
\mathcal L_{ik}G_k^{\ j}
=\delta_i^{\ j}\delta(\mathbf x-\boldsymbol\xi)\delta(t),\qquad
G_i^{\ j}=0\quad(t<0).
$$

It satisfies the actual Earth's homogeneous [boundary conditions](../../../../../boundary-condition.md), including zero [traction](../../../../../traction.md) on the free surface and continuity of displacement and [traction](../../../../../traction.md) at bonded internal interfaces. Integration through $t=0$ gives $\rho(\mathbf x)\partial_tG_i^{\ j}(0^+)=\delta_i^{\ j}\delta(\mathbf x-\boldsymbol\xi)$, with $G(0^+)=0$. No spherical symmetry is required.

For zero [initial conditions](../../../../../initial-condition.md), form the [convolution](../../../../../convolution.md)

$$
\boxed{u_i(\mathbf x,t)=\int_0^t\!d\tau\int_V
G_i^{\ j}(\mathbf x,\boldsymbol\xi,t-\tau)\rho(\boldsymbol\xi)f_j(\boldsymbol\xi,\tau)\,dV_\xi.}
$$

Applying $\mathcal L$ to this expression uses the defining [Dirac delta function](../../../../../dirac-delta-function.md) to give $\rho(\mathbf x)f_i(\mathbf x,t)$. Causality gives zero [initial conditions](../../../../../initial-condition.md), and each Green column supplies the required [boundary conditions](../../../../../boundary-condition.md). The positive-energy uniqueness argument then identifies this expression with the physical response. The source factor is $\rho(\boldsymbol\xi)$ because $f$ is force per unit mass, whereas the Green tensor was normalized to unit force.

A force dipole is a limiting pair of opposite point forces separated by a small vector. Put $+F_j$ at $\boldsymbol\xi+\varepsilon\mathbf d/2$ and $-F_j$ at $\boldsymbol\xi-\varepsilon\mathbf d/2$, and hold $D_{jk}=\varepsilon F_jd_k$ fixed as $\varepsilon\to0$. Expansion of the two [Dirac delta functions](../../../../../dirac-delta-function.md) gives

$$
q_j(\boldsymbol\eta,t)=-D_{jk}(t)\partial_{\eta_k}\delta(\boldsymbol\eta-\boldsymbol\xi).
$$

Its resultant force is zero, and [integration by parts](../../../../../integration-by-parts.md) gives its radiated displacement as $\int_0^t D_{jk}(\tau)\partial_{\xi_k}G_i^{\ j}(\mathbf x,\boldsymbol\xi,t-\tau)\,d\tau$. Thus the source derivative of the [elastodynamic Green tensor](../../../../../elastodynamic-green-tensor.md) represents a dipole with force direction $j$ and separation direction $k$.

For the surface source choose a normal $\mathbf n$ from the minus side to the plus side and define

$$
b_i=[u_i]=u_i^+-u_i^-,\qquad [t_i]=(\sigma_{ij}^+-\sigma_{ij}^-)n_j.
$$

The same normal is used in both tractions. If the elastic coefficients are continuous through the surface, the distributional gradient of a piecewise smooth displacement is $\partial_j u_i=(\partial_j u_i)_{\mathrm{reg}}+b_i n_j\delta_\Sigma$. Its [stress](../../../../../stress.md) therefore has a singular part $c_{ijkl}b_k n_l\delta_\Sigma$. Taking the divergence includes the regular [stress](../../../../../stress.md) jump, so a field satisfying the source-free equations on both sides has equivalent source

$$
q_i=-[t_i]\delta_\Sigma-\partial_j[c_{ijkl}b_k n_l\delta_\Sigma].
$$

In particular, the signs follow from the chosen jump convention, not from an unspecified orientation. The [elastodynamic surface-jump representation](../../../../../elastodynamic-surface-jump-representation.md) is consequently

$$
\boxed{u_i=\int_0^t\!d\tau\int_\Sigma
\left[-G_i^{\ j}[t_j]+M_{jk}\partial_{\xi_k}G_i^{\ j}\right]dS_\xi,
\qquad M_{jk}=c_{jk\ell m}b_\ell n_m,}
$$

with the Green tensor evaluated at $(\mathbf x,\boldsymbol\xi,t-\tau)$. The first term is a surface distribution of forces, and the second is a surface distribution of dipoles.

One can derive the same formula without multiplying discontinuous material coefficients by a surface delta. Apply [integration by parts](../../../../../integration-by-parts.md) on the two sides of $\Sigma$ to the field $u$ and the reciprocal Green field $v$. Major symmetry cancels the volume [strain](../../../../../strain.md) terms; the spatial identity is

$$
\int (v_i\mathcal L u_i-u_i\mathcal L v_i)\,dV
=\int_{\partial V}[u_i t_i(v)-v_i t_i(u)]\,dS
$$

when the temporal terms are handled by the retarded time [convolution](../../../../../convolution.md). More explicitly, take $v_i(\boldsymbol\xi,\tau)=G_i^{\ a}(\boldsymbol\xi,\mathbf x,t-\tau)$, extend the zero-initial-data solution causally to $\tau<0$, and integrate over all source times. Integration by parts cancels the two temporal terms, with zero endpoint terms; the causal supports subsequently reduce the representation to $0\leq\tau\leq t$. The Green impulse contributes $-u_a(\mathbf x,t)$ on the left. The two outward face normals are $\mathbf n$ and $-\mathbf n$, so their sum on the right is $-[u_i]t_i(v)+v_i[t_i]$. Moving it to the other side gives $[u_i]t_i(v)-v_i[t_i]$. The same identity applied to two force Green fields with interchanged source and receiver proves the reciprocal relation $G_i^{\ j}(\mathbf x,\boldsymbol\xi,t)=G_j^{\ i}(\boldsymbol\xi,\mathbf x,t)$; hence the displayed surface formula follows. On a bonded material interface the Green displacement and common Green [traction](../../../../../traction.md) are continuous: $[u_i]t_i(v)$ is then the unambiguous version of the dipole term, evaluated with the matching one-sided coefficients. External free-surface terms vanish because both tractions vanish.

For a fault in [isotropic](../../../../../isotropy.md) material, the [Lamé parameters](../../../../../lame-parameter.md) give

$$
c_{jk\ell m}=\lambda\delta_{jk}\delta_{\ell m}
+\mu(\delta_{j\ell}\delta_{km}+\delta_{jm}\delta_{k\ell}),\qquad
M_{jk}=\lambda(\mathbf b\cdot\mathbf n)\delta_{jk}
+\mu(b_jn_k+n_jb_k).
$$

Tangential slip obeys $\mathbf b\cdot\mathbf n=0$, and ordinary fault [traction](../../../../../traction.md) is continuous across the two faces. Therefore **the source is a [double-couple fault source](../../../../../double-couple-fault-source.md)** with

$$
\boxed{M_{jk}=\mu(b_jn_k+n_jb_k),\qquad [t_j]=0.}
$$

For a uniform patch of area $A$ with $\mathbf b=b\mathbf e_1$ and $\mathbf n=\mathbf e_3$, its integrated [seismic moment tensor](../../../../../seismic-moment-tensor.md) is

$$
\mathsf M=\begin{pmatrix}0&0&M_0\\0&0&0\\M_0&0&0\end{pmatrix},\qquad M_0=\mu A b.
$$

The $13$ dipole is a force in the slip direction separated in the normal direction; the $31$ dipole is a normal force separated in the slip direction. Their equal and opposite [torques](../../../../../torque.md) cancel. The symmetric trace-free [seismic moment tensor](../../../../../seismic-moment-tensor.md) has [eigenvalues](../../../../../eigenvalue.md) $M_0,-M_0,0$, with zero resultant force and [torque](../../../../../torque.md). A temporal [stress](../../../../../stress.md) drop on a fault is not a jump of [traction](../../../../../traction.md) between its two simultaneously matching faces; it does not add a single-force layer to this tangential-slip representation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
