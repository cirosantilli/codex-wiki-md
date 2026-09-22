<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a massless Dirac fermion,

$$
\mathcal L=\bar\psi i\gamma^\mu D_\mu\psi,
\qquad D_\mu=\partial_\mu+ieA_\mu.
$$

The local gauge symmetry gives the vector current $J^\mu=e\bar\psi\gamma^\mu\psi$. The global [chiral transformation](../../../../../../chiral-transformation.md) $\psi\mapsto e^{i\beta\gamma^5}\psi$ gives the classical [axial current](../../../../../../axial-current.md)

$$
J_{\rm ax}^\mu=\bar\psi\gamma^\mu\gamma^5\psi.
$$

Using the massless [Dirac equation](../../../../../../dirac-equation.md) and $\{\gamma^5,\gamma^\mu\}=0$ gives $\partial_\mu J_{\rm ax}^\mu=0$ classically.

Quantum mechanically, a gauge-invariant regulator for the fermion measure is not invariant under the axial rotation. In the Fujikawa form, its infinitesimal Jacobian contains

$$
-2i\beta\lim_{\Lambda\to\infty}
\operatorname{tr}\left[\gamma^5e^{-\not D^2/\Lambda^2}\right].
$$

The first nonzero term in the [heat kernel expansion](../../../../../../heat-kernel-expansion.md) is quadratic in $F_{\mu\nu}$. Using

$$
\operatorname{tr}\{\gamma^5[\gamma^\mu,\gamma^\nu]
[\gamma^\rho,\gamma^\sigma]\}=16i\epsilon^{\mu\nu\rho\sigma}
$$

and the Gaussian momentum integral gives the [chiral anomaly](../../../../../../chiral-anomaly.md)

$$
\boxed{\partial_\mu J_{\rm ax}^\mu
=-\frac{e^2}{16\pi^2}\epsilon^{\alpha\beta\gamma\delta}
F_{\alpha\beta}F_{\gamma\delta}}.
$$

The overall sign follows the gamma-matrix, charge, and Levi-Civita conventions stated in the question. The same coefficient is obtained from the one-loop axial-vector-vector triangle diagram.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
