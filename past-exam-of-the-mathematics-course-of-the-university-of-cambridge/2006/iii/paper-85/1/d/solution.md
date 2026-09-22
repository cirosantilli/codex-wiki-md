<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The rescaling resolves the small, nearby nonzero saddles while retaining the weak non-Hamiltonian terms. It allows the global [stable manifold](../../../../../../stable-manifold.md)/[unstable manifold](../../../../../../unstable-manifold.md) connection to be studied as a [perturbation](../../../../../../perturbation.md) of the explicit [heteroclinic cycle](../../../../../../heteroclinic-cycle.md), rather than searched for only in the original variables.

Differentiate the [first integral](../../../../../../first-integral.md) using the first-order [perturbation](../../../../../../perturbation.md) from part (c):

$$
H'=\varepsilon(\mu-v^2/2)\bigl(2u^2+sv^2-v^4/2\bigr)+O(\varepsilon^2).
$$

On the positive unperturbed connecting branch, $u=(2s-v^2)/(2\sqrt2)$, so

$$
2u^2+sv^2-v^4/2=(s-v^2/2)(s+v^2/2),\qquad
 d\tau=\frac{dv}{\sqrt2(s-v^2/2)}.
$$

Integrating the [energy](../../../../../../energy.md) change from one [saddle equilibrium](../../../../../../saddle-equilibrium.md) to the other therefore gives

$$
\boxed{\Delta H=\frac{\varepsilon}{\sqrt2}M(\mu,s)+O(\varepsilon^2),\quad
M=\int_{-\sqrt{2s}}^{\sqrt{2s}}(\mu-v^2/2)(s+v^2/2)\,dv.}
$$

This is the [heteroclinic Melnikov integral for a quartic Hamiltonian](../../../../../../heteroclinic-melnikov-integral-for-a-quartic-hamiltonian.md). It measures the first-order [energy](../../../../../../energy.md) mismatch, equivalently the transverse splitting between the outgoing [unstable manifold](../../../../../../unstable-manifold.md) and the incoming [stable manifold](../../../../../../stable-manifold.md). A nonzero value means that the [heteroclinic orbit](../../../../../../heteroclinic-orbit.md) has broken. A simple zero supplies the leading connection condition; smooth [perturbation](../../../../../../perturbation.md) then shifts the curve by higher-order terms. The central inversion [symmetry](../../../../../../symmetry-physics.md) makes the two connections have the same condition, so both can be restored on one parameter curve.

For fixed $s>0$, $\partial M/\partial\mu=\int_{-\sqrt{2s}}^{\sqrt{2s}}(s+v^2/2)dv>0$. The coefficient is affine in $\mu$, has a unique simple zero, and changes sign across it. No explicit evaluation is necessary. [Energy](../../../../../../energy.md) drift on the nearby closed [Hamiltonian](../../../../../../hamiltonian.md) levels can similarly determine a [periodic orbit](../../../../../../periodic-orbit.md) and its stability; the cycle born at the supercritical [Hopf bifurcation](../../../../../../hopf-bifurcation.md) grows towards the [separatrix](../../../../../../separatrix.md) and can terminate at this [global bifurcation](../../../../../../global-bifurcation.md) through a [heteroclinic orbit](../../../../../../heteroclinic-orbit.md). Translating the resulting balance curve back with $\mu_{\rm old}=\varepsilon^2\mu$, $\sigma-1=\varepsilon^2s$ places it near the original double-zero point.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
