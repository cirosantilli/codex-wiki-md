<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The divergent part follows from the elementary integrals $\int_0^1x\,dx=1/2$ and $\int_0^1dx=1$:

$$
\Sigma_{\rm div}(\not p)=\boxed{\frac{e^2}{8\pi^2\epsilon}(\not p-4m).}
$$

Thus **a wave-function counterterm and a mass counterterm are required**. Write their contribution as

$$
\mathcal L_{\rm ct}=\delta Z_2\bar\psi i\not\partial\psi-\delta m_{\rm coeff}\bar\psi\psi.
$$

In the insertion convention of part (a), the inverse [Dirac propagator](../../../../../../dirac-propagator.md) receives $\delta Z_2\not p-\delta m_{\rm coeff}$. With $\kappa=e^2/(8\pi^2\epsilon)$, cancellation requires

$$
\boxed{\delta Z_2=-\kappa,\qquad\delta m_{\rm coeff}=-4\kappa m.}
$$

To distinguish the coefficient counterterm from the multiplicative mass renormalization, write $m_0=Z_m m$ and $\psi_0=Z_2^{1/2}\psi$. Then $\delta m_{\rm coeff}=m(\delta Z_2+\delta Z_m)$ at this order, giving $\delta Z_m=-3\kappa$. In [modified minimal subtraction](../../../../../../modified-minimal-subtraction-scheme.md), replace $\kappa$ by $e^2\Delta_{\overline{\rm MS}}/(16\pi^2)$. No new derivative structure is needed for this two-point divergence; charge and photon [counterterms](../../../../../../counterterm.md) are determined from other functions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
