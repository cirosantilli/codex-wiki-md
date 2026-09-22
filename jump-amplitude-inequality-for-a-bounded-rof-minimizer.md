# Jump-amplitude inequality for a bounded ROF minimizer

↑ **Parent:** [Jump-amplitude inequality for total variation denoising](jump-amplitude-inequality-for-total-variation-denoising.md)

Assume $w\in BV\cap L^\infty$ minimizes scalar [total variation denoising](total-variation-denoising.md) for $g\in BV\cap L^2$. The data $g$ may be unbounded. For the [local flow](local-flow.md) of $\varphi e_j$, use $(1-\theta)w+\theta w\circ\Phi_{\pm t}$ as two competitors. The [total variation under opposite smooth flows](total-variation-under-opposite-smooth-flows.md) and convexity of the [total variation seminorm](total-variation-seminorm-on-a-domain.md) bound the sum of regularizer changes by $O(t^2)$. Minimality and the [opposite-flow fidelity identity for quadratic data](opposite-flow-fidelity-identity-for-quadratic-data.md), evaluated using the [BV jump-product limit with one bounded factor](bv-jump-product-limit-with-one-bounded-factor.md), imply

$$
\int_{J_w}([g][w]-(1-\theta)[w]^2)\varphi|\nu_w\cdot e_j|\,d\mathcal H^{n-1}\ge0.
$$

Let $\theta\downarrow0$. The integrands define finite signed [Radon measures](radon-measure.md), since $w$ is bounded and the jump variation of $g$ is finite. Arbitrary nonnegative smooth $\varphi$ make their densities nonnegative. Testing every coordinate direction removes the factor $|\nu_w\cdot e_j|$ and proves the stated inequality.

## ↑ Ancestors (10)

1. [Jump-amplitude inequality for total variation denoising](jump-amplitude-inequality-for-total-variation-denoising.md)
2. [Total variation denoising](total-variation-denoising.md)
3. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
4. [Variational regularization](variational-regularization.md)
5. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
6. [Inverse problem](inverse-problem-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Jump-amplitude inequality for total variation denoising](jump-amplitude-inequality-for-total-variation-denoising.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64/2/iii/solution.md)
