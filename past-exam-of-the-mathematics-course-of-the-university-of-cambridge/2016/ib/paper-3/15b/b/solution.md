<h1 id="15b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the spatial [Fourier transform](../../../../../../fourier-transform.md) of the [diffusion equation](../../../../../../diffusion-equation-split.md) gives $\widetilde\theta_t=-Dk^2\widetilde\theta$ and $\widetilde\theta(k,0)=\widetilde g(k)$. Hence $\widetilde\theta=e^{-Dk^2t}\widetilde g$. [Fourier inversion](../../../../../../fourier-inversion-theorem.md) and the Gaussian transform from part (a), or direct evaluation of the inverse Gaussian integral, give the [heat kernel](../../../../../../heat-kernel.md)

$$
K_t(x)=\frac1{\sqrt{4\pi Dt}}e^{-x^2/(4Dt)}.
$$

Substituting the integral for $\widetilde g$ and interchanging absolutely integrable terms produces the [convolution](../../../../../../convolution.md) solution

$$
\boxed{\theta(x,t)=\frac1{\sqrt{4\pi Dt}}
\int_{\mathbb R}g(\xi)e^{-(x-\xi)^2/(4Dt)}\,d\xi,\qquad t>0.}
$$

For the stated nonnegative compactly supported data, understood to be nonzero on a set of positive measure, the kernel is strictly positive everywhere. Therefore $\theta(x,t)>0$ for every real $x$ and every $t>0$. **Property P holds: diffusion has [infinite propagation speed](../../../../../../infinite-propagation-speed.md).** The distant value can be extremely small, but is not zero. For continuous initial data, any nontrivial nonnegative $g$ automatically has the required positive-measure set.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15B](../../15b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
