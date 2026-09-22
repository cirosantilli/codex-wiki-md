<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a deterministic localized initial peak in an unbounded $d$-dimensional sample, the mean obeys $\partial_t\langle\phi\rangle=\Gamma\kappa\nabla^2\langle\phi\rangle-\Gamma a\langle\phi\rangle$. The [Gaussian Model A impulse response](../../../../../../gaussian-model-a-impulse-response.md) is therefore the [heat kernel](../../../../../../heat-kernel.md) multiplied by the local relaxation factor:

$$
\boxed{\langle\phi(\mathbf r,t)\rangle=\frac{A e^{-\Gamma at}}{(4\pi\Gamma\kappa t)^{d/2}}\exp\left[-\frac{|\mathbf r-\mathbf r'|^2}{4\Gamma\kappa t}\right],\qquad t>0.}
$$

The peak spreads over a distance of order $\sqrt{\Gamma\kappa t}$ and its central height falls both by spreading and by exponential relaxation. Its integrated mean is $A e^{-\Gamma at}$, rather than $A$: the equation describes [nonconserved order-parameter dynamics](../../../../../../nonconserved-order-parameter-dynamics.md), despite the use of the word “density” in this part.

An individual realization also develops thermal fluctuations; it does not tend pointwise to zero. For an initially deterministic field, the connected [Fourier mode](../../../../../../fourier-mode.md) variance grows as $[k_BT/(a+\kappa q^2)](1-e^{-2r(q)t})$, while the deterministic mean decays. It approaches the zero-mean Gaussian equilibrium field at the coarse-graining cutoff. On a periodic or bounded sample use the corresponding boundary-adapted [heat kernel](../../../../../../heat-kernel.md); at $\kappa=0$ there is no spatial spreading. The [Dirac delta distribution](../../../../../../dirac-delta-function.md) is an ideal initial profile, recovered as a distributional limit; a finite-energy physical peak has a microscopic width.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
