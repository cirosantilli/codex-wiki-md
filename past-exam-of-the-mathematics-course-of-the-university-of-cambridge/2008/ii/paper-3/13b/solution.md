<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

For a small [Fourier mode](../../../../../fourier-mode.md) $u=Ue^{ikx+\sigma t}$, $v=Ve^{ikx+\sigma t}$, the inhibitor equation gives $V=U/(1+k^2)$. The [linearization](../../../../../linearization.md) of the cubic reaction at zero is $-rU$. Thus the [fast-inhibitor cubic activator growth rate](../../../../../fast-inhibitor-cubic-activator-growth-rate.md) is

$$
\boxed{\sigma(k)=-r-Dk^2+\frac{\rho k^2}{1+k^2}.}
$$

It is an [even function](../../../../../even-function.md) of $k$, starts at $\sigma(0)=-r<0$, and tends to $-\infty$ as $|k|\to\infty$. In terms of $q=k^2$, its derivative is $-D+\rho/(1+q)^2$. If $\rho>D$, the maxima occur at $k=\pm\sqrt{\sqrt{\rho/D}-1}$, with

$$
\boxed{\sigma_{\max}=-r+(\sqrt\rho-\sqrt D)^2.}
$$

If $\rho\leq D$, the maximum is $-r$ at $k=0$ and all modes decay. For $\rho>D$, the zero state is unstable when $(\sqrt\rho-\sqrt D)^2>r$, and the stability boundary is

$$
\boxed{\rho=(\sqrt r+\sqrt D)^2,}
$$

where this curve lies in the allowed parameter region.

<a id="13b/image-growth-rate-curves-and-the-zero-state-stability-boundary-of-the-fast-inhibitor-model"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3-growth-rates.png)

**[Figure 1](#13b/image-growth-rate-curves-and-the-zero-state-stability-boundary-of-the-fast-inhibitor-model). Growth-rate curves and the zero-state stability boundary of the fast-inhibitor model**.

Putting $\widetilde u=1-u$, $\widetilde v=1-v$ and $\widetilde r=1-r$ negates both original equations and restores precisely the same form, because $\widetilde u(\widetilde u-\widetilde r)(\widetilde u-1)=-u(u-r)(u-1)$. Therefore the state $u=v=1$ has the corresponding boundary $\boxed{\rho=(\sqrt{1-r}+\sqrt D)^2}$.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
