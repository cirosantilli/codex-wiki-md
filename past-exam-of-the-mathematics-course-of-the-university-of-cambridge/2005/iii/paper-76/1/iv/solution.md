<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A field in a circulation plane has components crossing circular streamlines. [Magnetic flux freezing](../../../../../../magnetic-flux-freezing.md) carries those lines with [fluid elements](../../../../../../fluid-element.md) at different [angular speeds](../../../../../../angular-speed.md): the lines become spirals, their azimuthal components are stretched, and neighboring turns acquire increasingly small separations. This is a nonaxisymmetric winding and phase-mixing problem.

For illustration, in the ideal limit take the initial horizontal field along $x$ and fix a horizontal plane. With $\chi=\phi-\omega(s,z)t$, the induction equations give

$$
B_s=B_0\cos\chi,\qquad B_\phi=-B_0\sin\chi+s\,t\,\partial_s\omega\,B_0\cos\chi,\qquad B_z=0.
$$

The first term describes advection around a circle; the term proportional to $t\partial_s\omega$ is the stretching by [differential rotation](../../../../../../differential-rotation.md). Spatial variation of $\omega$ also produces phase gradients proportional to $t\nabla\omega$. A rigidly rotating region merely turns the horizontal field, whereas a shearing region progressively winds it up.

Even small [magnetic diffusivity](../../../../../../magnetic-diffusivity.md) becomes important once these gradients are large. Locally a phase mode of azimuthal order $m$ has damping rate of order $\eta m^2|\nabla\omega|^2t^2$, leading to attenuation of order $\exp[-\eta m^2|\nabla\omega|^2t^3/3]$. The associated [magnetic phase mixing under differential rotation](../../../../../../magnetic-phase-mixing-under-differential-rotation.md) time is

$$
t_{\mathrm{mix}}\sim[\eta m^2|\nabla\omega|^2]^{-1/3}.
$$

For a horizontal uniform seed, $m=1$; if $|\nabla\omega|\sim\Omega/\ell$, this is $\Omega^{-1}R_m^{1/3}$, much shorter than the ordinary diffusion time at large $R_m$. Resistive smoothing cancels the closely spaced oppositely directed field and, in persistent circulation regions with an imposed surrounding field, drives [flux expulsion](../../../../../../flux-expulsion.md) from the interiors toward their boundaries. The detailed final distribution depends on the geometry and boundary forcing. Winding alone does not supply a self-sustaining poloidal–toroidal regeneration loop, and magnetic feedback can again limit the kinematic process.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
