<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In infinitesimal [elasticity](../../../../../elasticity-physics.md) and [plasticity in continuum mechanics](../../../../../plasticity-physics.md), decompose the symmetric [strain](../../../../../strain.md) as $e=e^e+e^p$. For incompressible isotropic elasticity, $\sigma'=2G e^e$, with $G$ the [shear modulus](../../../../../shear-modulus.md) and both strains traceless. The [associated flow rule](../../../../../associated-flow-rule.md) for the [Von Mises yield criterion](../../../../../von-mises-yield-criterion.md) has $\dot e^p=\Lambda\sigma'$ after absorbing a positive factor into $\Lambda\geq0$. [Plane strain](../../../../../plane-strain.md) has $e_{33}=0$, so

$$
0=\dot e^e_{33}+\dot e^p_{33}=\frac{\dot\sigma'_{33}}{2G}+\Lambda\sigma'_{33}.
$$

If $\sigma'_{33}=0$ initially, it remains zero by this homogeneous scalar differential equation. Then $e^e_{33}=0$ and $\dot e^p_{33}=0$, so $e^p_{33}=0$ is consistent with zero initial plastic component. This proves consistency, not a claim that arbitrary prestressed plane-strain histories must have zero separate components. The out-of-plane shear components can consistently be zero by the same argument.

Write $p=-\operatorname{tr}\sigma/3$, so $\sigma_{33}=-p$. The proposed in-plane parameterization has

$$
\sigma'=k\begin{pmatrix}\sin2\phi&-\cos2\phi&0\\-\cos2\phi&-\sin2\phi&0\\0&0&0\end{pmatrix}.
$$

Its squared contraction is $2k^2(\sin^22\phi+\cos^22\phi)=2k^2$, proving the yield condition identically. Its principal deviatoric stresses are $k,-k,0$. Define the two [slip line](../../../../../slip-line.md) families by tangent unit vectors

$$
a=(\cos\phi,\sin\phi),\qquad b=(-\sin\phi,\cos\phi).
$$

Thus $\alpha$ lines have tangent angle $\phi$ and $\beta$ lines have tangent angle $\phi+\pi/2$. Their normal extensions from the associated plastic strain rate vanish, while their shear stresses have maximum magnitude $k$; they are not the principal stress directions.

In the absence of body force, differentiate the stress parameterization in the two equilibrium equations. One obtains

$$
p_{,1}=2k(\cos2\phi\,\phi_{,1}+\sin2\phi\,\phi_{,2}),\qquad
p_{,2}=2k(\sin2\phi\,\phi_{,1}-\cos2\phi\,\phi_{,2}).
$$

The symmetric matrix multiplying $2k\nabla\phi$ has eigenvectors $a,b$ with eigenvalues $+1,-1$. Taking its contraction with these vectors proves

$$
a\cdot\nabla(p-2k\phi)=0,\qquad b\cdot\nabla(p+2k\phi)=0.
$$

Hence the [Hencky stress relations](../../../../../hencky-stress-relations.md) are

$$
\boxed{p-2k\phi=\text{constant on each }\alpha\text{ line},\qquad p+2k\phi=\text{constant on each }\beta\text{ line}}.
$$

Constants can differ between lines, and these signs depend on the specified negative shear-stress convention.

Place the notch tip at the origin, with the opening towards negative $x_1$ and tensile loading in the transverse direction. For a usual reentrant notch, $0\leq\gamma\leq\pi/2$. The upper face has tangent angle $\vartheta_f=\pi-\gamma$. Choose its tangent $t=(\cos\vartheta_f,\sin\vartheta_f)$ directed away from the tip and outward material normal $n=(-\sin\vartheta_f,\cos\vartheta_f)$ pointing into the notch. Direct rotation of the stress gives the normal and tangential [traction](../../../../../traction.md) components

$$
\boxed{t_n=n\cdot\sigma n=-p-k\sin(2\phi-2\vartheta_f),\qquad t_t=t\cdot\sigma n=-k\cos(2\phi-2\vartheta_f)}.
$$

Take the notch faces traction-free, as intended by the notch problem. Then the cosine vanishes. Select the tensile branch $\sin(2\phi-2\vartheta_f)=1$, for which the face-tangential normal stress is $2k$. Thus the upper face has $\boxed{p=-k,\ \phi_f=\pi/4-\gamma\pmod\pi}$. Choosing the opposite branch would describe compression rather than the tensile field.

Construct the [centred slip-line fan at a traction-free V-notch](../../../../../centred-slip-line-fan-at-a-traction-free-v-notch.md) to connect this surface state to the forward symmetry axis. Near the upper face there is a constant-stress region. It joins a fan bounded by rays

$$
\vartheta_1=\pi/4,\qquad\vartheta_2=3\pi/4-\gamma.
$$

Inside the fan choose $\beta$ lines radial and $\alpha$ lines circular about the tip, so their angle parameter is $\phi=\vartheta-\pi/2$. Along a circular $\alpha$ line the first invariant gives

$$
p(\vartheta)=-k+2k[\phi(\vartheta)-\phi_f]=-k+2k[\vartheta-(3\pi/4-\gamma)].
$$

The second invariant is automatically constant along each radial $\beta$ line because $p,\phi$ are independent of radius. Thus this is an actual equilibrium fan, not just an assumed transport of a surface value. At $\vartheta_2$ it matches the free-face constant state. At $\vartheta_1$ it matches a forward constant-stress region with

$$
\phi=-\pi/4,\qquad p=-k(1+\pi-2\gamma).
$$

Reflect the upper field across the symmetry axis to obtain the lower field. The forward region has zero shear, respects this symmetry, and contains the positive $x_1$ axis. There $\sin2\phi=-1$, and hence

$$
\boxed{\sigma_{22}=-p+k=k(2+\pi-2\gamma)}.
$$

This value holds in the fully plastic notch-tip region described by the field. It is not a uniform stress assertion for the entire axis of an arbitrary finite specimen, including any elastic or far-field region.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
