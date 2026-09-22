<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [isotropic turbulence](../../../../../../isotropic-turbulence.md) with [incompressible flow](../../../../../../incompressible-flow.md), use the spectral [velocity correlation tensor](../../../../../../velocity-correlation-tensor.md)

$$
\Phi_{ij}(\boldsymbol k)=\frac{E(k)}{4\pi k^2}
\left(\delta_{ij}-\frac{k_ik_j}{k^2}\right),\qquad
Q_{ij}(\boldsymbol r)=\int\Phi_{ij}(\boldsymbol k)e^{i\boldsymbol k\cdot\boldsymbol r}d^3k.
$$

Choose the polar axis along $\boldsymbol r$ and put $\mu=\widehat{\boldsymbol k}\cdot\widehat{\boldsymbol r}$. The [longitudinal velocity correlation](../../../../../../longitudinal-velocity-correlation.md) becomes

$$
Q_{LL}(r)=\frac12\int_0^\infty E(k)dk\int_{-1}^1(1-\mu^2)e^{ikr\mu}d\mu.
$$

Starting with $\int_{-1}^1e^{ix\mu}d\mu=2\sin x/x$ and differentiating twice in $x$ evaluates the weighted angular integral:

$$
\int_{-1}^1(1-\mu^2)e^{ix\mu}d\mu
=\frac{4(\sin x-x\cos x)}{x^3}.
$$

Therefore $Q_{LL}(r)=2\int E(k)(\sin(kr)-kr\cos(kr))/(kr)^3dk$. At zero separation $Q_{LL}(0)=(2/3)\int E(k)dk$. Using $S_2=2[Q_{LL}(0)-Q_{LL}(r)]$ proves the exact [structure-function spectral filter](../../../../../../structure-function-spectral-filter.md):

$$
\boxed{\frac34S_2(r)=\int_0^\infty E(k)H(kr)dk,\qquad
H(x)=1+\frac{3\cos x}{x^2}-\frac{3\sin x}{x^3}.}
$$

The apparent singularity is removable: expansion gives $H(x)=x^2/10+O(x^4)$ at zero, while $H(x)\to1$ at infinity. Substitute the given approximate filter and split the integral at $k_c=\pi/r$. This gives

$$
\boxed{\frac34S_2(r)\simeq\int_{\pi/r}^\infty E(k)dk
+\frac{r^2}{\pi^2}\int_0^{\pi/r}k^2E(k)dk.}
$$

The second term is the contribution of larger eddies: their common [velocity](../../../../../../velocity.md) cancels, but their [velocity](../../../../../../velocity.md) [gradient](../../../../../../gradient.md) creates an increment proportional to $r$. Their squared [gradient](../../../../../../gradient.md) contributes the $k^2$ weight. The integral $\int k^2E(k)dk$ is the [enstrophy](../../../../../../enstrophy.md) in the convention $\langle|\boldsymbol\omega|^2\rangle/2$, so the increment contains both small-scale energy and cumulative larger-scale enstrophy.

This makes the [longitudinal structure function](../../../../../../longitudinal-velocity-structure-function.md) a poor diagnostic of a finite [inertial range](../../../../../../inertial-range.md). With a limited range of $k^{-5/3}$ spectrum, the two integrals retain outer-scale and dissipation-scale contributions, leading schematically to a mixture $a_0+a_2r^2+a_{2/3}r^{2/3}$. The local logarithmic slope need not then equal $2/3$, even if the spectral inertial interval exhibits a clearer $-5/3$ slope. This finite-range effect was demonstrated in [Davidson and Krogstad's 2008 controlled-field study](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/on-the-deficiency-of-evenorder-structure-functions-as-inertialrange-diagnostics/20C72BC567F69524E1F25A1E6AEA19A5). It challenges interpreting $S_2(r)$ as energy exclusively at scale $r$; it does not refute the formal infinite-inertial-range two-thirds law, since inserting an ideal $k^{-5/3}$ spectrum into the exact transform does produce $r^{2/3}$ scaling.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
