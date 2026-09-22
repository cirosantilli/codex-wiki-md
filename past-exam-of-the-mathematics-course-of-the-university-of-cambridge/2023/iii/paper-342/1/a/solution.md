<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Represent quasiparticle worldlines by conserved currents $j_I^\alpha$ and add the minimal-coupling term

$$
\mathcal L_{\rm src}=-a_{I\alpha}j_I^\alpha.
$$

Up to the corresponding sign convention for charge, variation of the [Abelian Chern--Simons theory](../../../../../../abelian-chern-simons-theory.md) gives

$$
\boxed{
\frac1{2\pi\hbar}K_{IJ}\epsilon^{\alpha\beta\gamma}
\partial_\beta a_{J\gamma}=j_I^\alpha.}
$$

For a static quasiparticle of integer gauge-charge vector $q$, integration over a small surrounding disk yields the [Chern--Simons flux attachment](../../../../../../chern-simons-flux-attachment.md) relation

$$
\boxed{\Phi_I:=\int d^2x\,\epsilon^{0ij}\partial_i a_{Ij}
=2\pi\hbar(K^{-1}q)_I.}
$$

A quasiparticle of charge $q'$ carried once around this flux acquires the [Aharonov--Bohm phase](../../../../../../aharonov-bohm-effect.md)

$$
\frac1\hbar q'^T\Phi
=2\pi q'^TK^{-1}q=2\theta_{q'q},
$$

so

$$
\boxed{\theta_{q'q}=\pi q'^TK^{-1}q,
\qquad
e^{2i\theta_{q'q}}=e^{2\pi i q'^TK^{-1}q}.}
$$

The constituent-particle current has charge vector $t=(1,\ldots,1)^T$. Its integral over the same disk is

$$
\boxed{N=\frac1{2\pi\hbar}t^T\Phi=t^TK^{-1}q.}
$$

For $K=I_n$ and $q=e_J$, this gives $N=1$. The self-exchange angle is $\theta_{qq}=\pi e_J^Te_J=\pi$, so the excitation is a [fermion](../../../../../../fermion.md) with one unit of microscopic particle number and may be identified with an electron.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
