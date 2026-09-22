<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The capacity in this question is [harmonic capacity from infinity in the upper half-plane](../../../../../../harmonic-capacity-from-infinity-in-the-upper-half-plane.md), which has units of length; it is distinct from [half-plane capacity](../../../../../../half-plane-capacity.md), which has units of length squared.

Here is a proof of existence that also works with irregular real attachments. The function

$$
u(z)=\mathbb P_z(B_{T(H)}\in K)
$$

is bounded and [harmonic](../../../../../../harmonic-function.md) on $H$, by the [Strong Markov property](../../../../../../strong-markov-property.md) and the mean-value characterization of [harmonic functions](../../../../../../harmonic-function.md). Therefore $u\circ g_K^{-1}$ is a bounded [harmonic function](../../../../../../harmonic-function.md) on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md), with a [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md) representation

$$
u(g_K^{-1}(w))
=\int_{\mathbb R}\frac{\operatorname{Im}w}
{\pi|t-w|^2}\,f(t)\,dt,\qquad 0\le f\le1.
$$

The boundary function $f$ vanishes outside a bounded interval. Indeed, far enough along either real ray the original domain contains a half-disc neighbourhood, and $g_K$ extends there; the probability of hitting the bounded hull before the real boundary tends to zero as the starting point approaches that ray. Applying the same dominated-limit calculation as in part (i) yields

$$
\boxed{\operatorname{cap}(K)=\int_{\mathbb R}f(t)\,dt<\infty.}
$$

When the intrinsic boundary pieces landing on the hull are identified, $f$ is their indicator almost everywhere and this is the length of their image under $g_K$. For ordinary finite slit hulls this is exactly the image of $\delta H\setminus H_0$, since real attachment endpoints have zero [harmonic measure](../../../../../../harmonic-measure.md). The Poisson representation avoids requiring that boundary identification in the general existence argument.

If $K\subset K'$, couple the two exit events using the same [planar Brownian motion](../../../../../../planar-brownian-motion.md), stopped at its first hit of the real axis. Any path that hits $K$ before the real axis also hits $K'$ before the real axis. Consequently

$$
\mathbb P_{iy}(B_{T(\mathbb H\setminus K)}\in K)
\le
\mathbb P_{iy}(B_{T(\mathbb H\setminus K')}\in K'),
$$

and taking the limits proves **monotonicity of this capacity**.

For a half-disc of radius $r$ centred at $b\in\mathbb R$, the [mapping-out function](../../../../../../mapping-out-function-of-a-compact-h-hull.md) is

$$
g(z)=b+(z-b)+\frac{r^2}{z-b}.
$$

Its semicircular boundary maps onto $[b-2r,b+2r]$, of length $4r$. Hence its [harmonic capacity from infinity in the upper half-plane](../../../../../../harmonic-capacity-from-infinity-in-the-upper-half-plane.md) is $4r$. With

$$
\operatorname{rad}(K)=\inf\{r>0:K\subset\{z:|z-b|\le r\}
\text{ for some }b\in\mathbb R\},
$$

enclose $K$ in such a half-disc and use monotonicity. Letting the enclosing radius decrease to the infimum proves

$$
\boxed{\operatorname{cap}(K)\le4\operatorname{rad}(K).}
$$

The same conclusion holds if radius is instead measured about a specified real centre.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
