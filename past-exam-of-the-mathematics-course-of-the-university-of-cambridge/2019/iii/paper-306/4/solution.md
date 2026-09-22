<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Insert the given [closed-string mode expansion](../../../../../closed-string-mode-expansion.md) into the stress tensor and compare $T(z)=\sum_nL_nz^{-n-2}$. [Normal ordering](../../../../../normal-ordering.md) gives

$$
\boxed{L_n=\frac12\sum_{m\in\mathbb Z}:\alpha_{n-m}\cdot\alpha_m:}.
$$

The inverse of the worldsheet Laplacian gives the free-field operator-product expansion

$$
\boxed{X^\mu(z,\bar z)X^\nu(w,\bar w)\sim-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2}.
$$

Hence

$$
\partial X^\mu(z)\partial X^\nu(w)\sim-\frac{\alpha'}2\frac{\eta^{\mu\nu}}{(z-w)^2}.
$$

Extracting the Laurent modes by contour integration yields the [string oscillator](../../../../../string-oscillator.md) algebra

$$
\boxed{[\alpha_m^\mu,\alpha_n^\nu]=m\eta^{\mu\nu}\delta_{m+n,0}}.
$$

The vanishing of the worldsheet stress tensor becomes the [Virasoro constraints](../../../../../virasoro-constraint.md)

$$
L_n|\text{phys}\rangle=\bar L_n|\text{phys}\rangle=0\quad(n>0),
\qquad (L_0-a)|\text{phys}\rangle=(\bar L_0-a)|\text{phys}\rangle=0.
$$

Since $L_0=\alpha'k^2/4+N$ and the bosonic-string normal-ordering constant is $a=1$, these zero-mode constraints are the target-space [string mass-shell condition](../../../../../string-mass-shell-condition.md)

$$
M^2=\frac4{\alpha'}(N-1)=\frac4{\alpha'}(\bar N-1),
\qquad N=\bar N.
$$

Therefore

$$
\boxed{M_T^2=-\frac4{\alpha'},\qquad M_g^2=0.}
$$

The positive-mode constraints further require

$$
\boxed{k^\mu\epsilon_{\mu\nu}=0,\qquad k^\nu\epsilon_{\mu\nu}=0},
$$

and [null string states](../../../../../null-string-state.md) identify polarizations that differ by momentum-longitudinal terms. The symmetric trace-free, antisymmetric, and trace sectors of $\epsilon_{\mu\nu}$ describe the graviton, [Kalb–Ramond field](../../../../../kalb-ramond-field.md), and [dilaton](../../../../../dilaton.md), respectively.

Finally, the [state–operator correspondence](../../../../../state-operator-correspondence.md) maps $\alpha_{-1}^\mu\bar\alpha_{-1}^\nu|k\rangle$ to

$$
\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}.
$$

Adding its integrated [massless closed-string vertex operator](../../../../../massless-closed-string-vertex-operator.md) to the [string nonlinear sigma model](../../../../../string-nonlinear-sigma-model.md) changes the background coupling by

$$
\delta S\propto\int d^2z\,\delta G_{\mu\nu}(X)\partial X^\mu\bar\partial X^\nu.
$$

Thus a Fourier mode $\delta G_{\mu\nu}(X)=\epsilon_{(\mu\nu)}e^{ik\cdot X}$ is precisely a linearized deformation of the target-space metric. Its transversality, mass-shell condition, and polarization gauge redundancy are the worldsheet statements that the deformation is marginal and is defined up to a linearized spacetime diffeomorphism.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
