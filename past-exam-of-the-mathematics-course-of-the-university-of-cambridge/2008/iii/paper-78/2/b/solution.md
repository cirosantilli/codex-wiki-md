<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For repeated small returns, $\xi_{n+1}=O(z_n^\delta)$, so $\rho+\xi_n$ is close to the nonzero constant $\rho$. Retain its leading value in the second component. Combining $c\cos\vartheta+d\sin\vartheta$ into a single cosine, and absorbing the section size and fixed phases, gives the [Shilnikov return map](../../../../../../shilnikov-return-map.md)

$$
\boxed{z_{n+1}=-\mu+Az_n^\delta\cos(\Omega\log z_n+\Phi),\quad z_n>0,\qquad
\Omega=\omega/\lambda_+.}
$$

Changing the sign of the logarithmic angle changes only the phase after using cosine's evenness. A generic reinjection has $A>0$; $\Phi$ can be represented modulo $2\pi$ by a positive value. The original PDF has exponent $\delta$, which the converted TeX mistakenly replaced by $2$.

This is an asymptotic scalar approximation, not an assertion that the full map has an exact one-dimensional invariant quotient. To see why it captures the thin geometry, differentiate the two components in part (a). Their determinant is of order

$$
\det D\Pi_S=C(\rho+\xi)z^{2\delta-1}+\cdots,
$$

where $C$ involves $\Omega$ and the determinant of the global linear map. For $\delta>1/2$ this tends to zero, so the return is strongly area-contracting even when its longitudinal derivative is large. Its global quadratic corrections are $O(z^{2\delta})=o(z)$ in this range. For a small [fixed point](../../../../../../fixed-point.md), also $\xi=O(z^\delta)$, so ignoring $\xi$ contributes that same higher order. Multipassage iterates require all passage coordinates to stay in the small domain; the leading map describes their thin folded return geometry rather than controlling arbitrary points outside it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
