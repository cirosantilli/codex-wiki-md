<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the given [Pestov identity for a geodesic flow](../../../../../../pestov-identity-for-a-geodesic-flow.md) for the function $\varphi$ constructed above. Since $VX\varphi=-2H\varphi$, its left side is $-4\|H\varphi\|_{L^2(\mu)}^2$. Moving this to the right gives

$$
0=\|X\varphi\|_{L^2(\mu)}^2+5\|H\varphi\|_{L^2(\mu)}^2
+\int_{SM}(-K)(V\varphi)^2\,d\mu.
$$

All terms are nonnegative, and $-K$ is uniformly positive by compactness. The smooth derivatives therefore vanish pointwise:

$$
X\varphi=H\varphi=V\varphi=0.
$$

Since $X,H,V$ span the tangent bundle, $\varphi=c$ is constant, component by component if necessary.

On each circle fibre, $V^2u+u=c$ is the elementary periodic differential equation $u_{\vartheta\vartheta}+u=c$. Its solutions are

$$
u(x,\vartheta)=c+a(x)\cos\vartheta+b(x)\sin\vartheta.
$$

The first harmonics transform as a covector when the local oriented orthonormal frame changes. Their coefficients are smooth, either directly from the smooth fibre equation or from their sine/cosine integral formulas. Thus they define a smooth [one-form](../../../../../../one-form.md) $\eta$ on $M$ with $u(x,v)=c+\eta_x(v)$.

Along a geodesic, the velocity is parallel, so differentiating gives

$$
Xu(x,v)=\left.\frac d{dt}\eta_{\gamma(t)}(\dot\gamma(t))\right|_{t=0}
=(\nabla_v\eta)(v)=\langle\nabla_v\eta^\sharp,v\rangle.
$$

Set $Z=\eta^\sharp/2$. Then

$$
\boxed{\beta_x(v,v)=2\langle\nabla_vZ,v\rangle}.
$$

Equality initially holds on unit vectors, then on every vector by homogeneity. The [polarization identity](../../../../../../polarization-identity.md) yields the tensor identity

$$
\beta(v,w)=\langle\nabla_vZ,w\rangle+\langle\nabla_wZ,v\rangle
=(\mathcal L_Zg)(v,w).
$$

This proves that $\beta$ is a [potential symmetric 2-tensor](../../../../../../potential-symmetric-2-tensor.md), with the precise factor of two in the requested convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
