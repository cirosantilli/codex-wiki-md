<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Choose the positive [Green function](../../../../green-s-function-split.md) convention

$$
\boxed{-\Delta_xG(x,\xi)=\delta_\xi(x),\quad G=0\text{ on }\partial D,\quad
G(x,\xi)\sim-\frac1{2\pi}\log|x-\xi|\text{ near }\xi.}
$$

Away from its pole, $G$ is harmonic, and the [maximum principle for harmonic functions](../../../../maximum-principle-for-harmonic-functions.md) makes it positive inside $D$. The sign of its [logarithmic singularity](../../../../logarithmic-singularity.md) is important: it is the convention for $-\Delta$, whereas a [Green function](../../../../green-s-function-split.md) for $+\Delta$ has the opposite sign.

[Green's second identity](../../../../green-second-identity.md), justified by removing a small disk about the pole and taking its radius to zero, gives

$$
\int_D(u\Delta G-G\Delta u)\,dx
=\int_{\partial D}(u\partial_nG-G\partial_nu)\,ds.
$$

Since $\Delta u=-f$, $\Delta G=-\delta_\xi$ and $G$ vanishes on the outer boundary, this rearranges to

$$
\boxed{u(\xi)=\int_DG(x,\xi)f(x)\,dx-\int_{\partial D}g(x)\partial_nG(x,\xi)\,ds.}
$$

The local [logarithmic singularity](../../../../logarithmic-singularity.md) is integrable, so continuous $f$ gives a well-defined volume [integral](../../../../integral-split.md).

In [complex coordinates](../../../../complex-coordinate.md) $z=x+iy$, $\zeta=\xi+i\eta$ for the [unit disk](../../../../unit-disk.md), use

$$
G(z,\zeta)=\frac1{2\pi}\log\left|\frac{1-z\bar\zeta}{z-\zeta}\right|.
$$

The numerator has no zeros inside the disk, so its logarithm is harmonic there. On $|z|=1$, the numerator and denominator have equal modulus, giving the required zero boundary value. Differentiating in the outward radial direction at $z=e^{i\theta}$ gives

$$
\boxed{-\partial_nG(e^{i\theta},\zeta)=\frac{1-|\zeta|^2}{2\pi|e^{i\theta}-\zeta|^2}.}
$$

With zero forcing the representation therefore becomes the [Poisson integral](../../../../poisson-integral.md)

$$
\boxed{u(\xi,\eta)=\frac{1-\xi^2-\eta^2}{2\pi}\int_0^{2\pi}
\frac{g(\theta)\,d\theta}{(\xi-\cos\theta)^2+(\eta-\sin\theta)^2}.}
$$

Finally replace $\eta$ by $-\eta$ and change variable $\theta\mapsto2\pi-\theta$. Cosine stays the same, sine changes sign and the assumed boundary symmetry leaves $g$ unchanged. The [integral](../../../../integral-split.md) is therefore invariant, so $\boxed{u(\xi,-\eta)=u(\xi,\eta)}$. Equivalently, [reflection](../../../../reflection-mathematics.md) produces a [harmonic function](../../../../harmonic-function.md) with the same Dirichlet data, and uniqueness identifies it with the original solution.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the differential equations and applications course of the University of Oxford](../../../split.md)
5. [Differential equations and applications course of the University of Oxford](../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
