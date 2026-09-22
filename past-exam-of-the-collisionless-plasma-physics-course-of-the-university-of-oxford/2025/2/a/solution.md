<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [ordinary plasma wave](../../../../ordinary-plasma-wave.md) as

$$
\delta\mathbf E(\mathbf r,t)=\operatorname{Re}\{[\mathbf a_0+\varepsilon\mathbf a_1+\cdots]e^{iS(\mathbf r,t)}\},\qquad
\mathbf k=\nabla S,\quad\omega=-\partial_tS.
$$

The [eikonal function](../../../../eikonal-function.md) $S$ is dimensionless; it varies by order $\varepsilon^{-1}$ across a background scale $L_{\rm bg}$, where $\varepsilon\sim\lambda/L_{\rm bg}\ll1$. The amplitudes and equilibrium [plasma](../../../../plasma-physics.md) parameters vary on $L_{\rm bg}$, so $|\nabla\mathbf a_j|\ll k|\mathbf a_j|$ and $|\nabla k|\ll k^2$. The equilibrium is stationary, so $\omega$ is constant along propagation. Assume infinitesimal fields, negligible [collisions](../../../../collision.md), $kv_{\mathrm{th},s}\ll\omega$, negligible [ion](../../../../ion.md) response, and a fixed [ordinary plasma wave](../../../../ordinary-plasma-wave.md) [polarization](../../../../polarization-waves.md) with $\mathbf B_0\parallel\hat{\mathbf z}$ and spatial variation along $x$. The [WKB approximation](../../../../wkb-approximation.md) is used away from [wave turning points](../../../../wave-turning-point.md) and [plasma wave resonances](../../../../plasma-wave-resonance.md).

Replacing derivatives on the fast factor by $i\mathbf k$ and $-i\omega$ in the [Maxwell equations](../../../../maxwell-equations-split.md) reproduces the local [magnetized cold-plasma dielectric tensor](../../../../magnetized-cold-plasma-dielectric-tensor.md) equation of [b](../../1/b.md). In this one-dimensional [ordinary plasma wave](../../../../ordinary-plasma-wave.md) geometry, the [Maxwell equations](../../../../maxwell-equations-split.md) and the local cold parallel [current density](../../../../current-density.md) in fact give the scalar equation directly:

$$
\boxed{\frac{d^2\delta E_z}{dx^2}+k^2(x)\delta E_z=0,\qquad
k^2(x)=\frac{\omega^2-\omega_{pe}^2(x)}{c^2}.}
$$

For $\delta E_z=a(x)e^{iS(x)}$, substitution gives

$$
a''+2ik a'+ik'a+[k^2(x)-(S')^2]a=0.
$$

The leading [eikonal equation](../../../../eikonal-equation.md) is $(S')^2=k^2(x)$, and the next order gives $2ka'+k'a=0$, hence the [flux-normalized WKB amplitude](../../../../flux-normalized-wkb-amplitude.md) $a\propto k^{-1/2}$. In particular, require $|k'|/|k|^2\ll1$ and $|k''|/|k|^3\ll1$; these fail at the [wave turning points](../../../../wave-turning-point.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
