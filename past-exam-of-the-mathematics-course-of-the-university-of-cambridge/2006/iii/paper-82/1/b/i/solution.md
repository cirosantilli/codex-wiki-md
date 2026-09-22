<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $D_{ij}=T^+_{ij}-T^-_{ij}$, so the [Lighthill stress tensor](../../../../../../../lighthill-stress-tensor.md) is $T^-_{ij}+D_{ij}H(S)$. Write $S_i=\partial_iS$ and $S_{ij}=\partial_i\partial_jS$. The [distributional derivative of the Heaviside step function](../../../../../../../distributional-derivative-of-the-heaviside-step-function.md) gives $\partial_iH(S)=S_i\delta(S)$. Applying the [product rule](../../../../../../../product-rule.md) a second time yields the [surface sources of a discontinuous Lighthill stress tensor](../../../../../../../surface-sources-of-a-discontinuous-lighthill-stress-tensor.md):

$$
\begin{aligned}
\partial_i\partial_jT_{ij}={}&H(S)\partial_i\partial_jT^+_{ij}+H(-S)\partial_i\partial_jT^-_{ij}\\
&+\bigl(D_{ij,i}S_j+D_{ij,j}S_i+D_{ij}S_{ij}\bigr)\delta(S)
+D_{ij}S_iS_j\delta'(S).
\end{aligned}
$$

Repeated indices are summed. The first line gives the two bulk [acoustic quadrupole](../../../../../../../acoustic-quadrupole.md) distributions. The second line consists of additional [surface delta distributions](../../../../../../../surface-delta-distribution.md) and their derivatives, all supported on the [shock wave](../../../../../../../shock-wave.md) $S=0$. For a symmetric [Lighthill stress tensor](../../../../../../../lighthill-stress-tensor.md), the first two coefficients of $\delta(S)$ combine to $2D_{ij,i}S_j$ after relabelling indices.

**A discontinuity therefore adds both a surface-delta source and a surface-delta-derivative source.** The level function need not be a signed distance: retaining its derivatives makes the expression invariant under a smooth reparametrization of the same surface. If the two bulk fields are only continuously differentiable, their second derivatives in the first line are read weakly; no classical second derivative is being assumed. The coefficients multiplying $\delta'(S)$ are kept as extensions, not replaced prematurely by traces.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
