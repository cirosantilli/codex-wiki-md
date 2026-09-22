<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two differentiated [linear integral equations](../../../../../../linear-integral-equation.md) have now supplied both equations of the [Lax pair](../../../../../../lax-pair.md). To verify the nonlinear consequence explicitly, put $D=\partial_x$ and take the operator [commutator](../../../../../../commutator.md) in the order $[N,M]=NM-MN$. The product rule gives

$$
[N,M]=-3q_xD^2+3ikq_xD+(q_t+q_{xxx}+3qq_x)
=-3q_xM+(q_t+q_{xxx}+6qq_x).
$$

For example, $[D^3,q]=3q_xD^2+3q_{xx}D+q_{xxx}$ and $[3qD,D^2]=-6q_xD^2-3q_{xx}D$, which explain the cancellations. Acting on $\varphi$ yields

$$
(q_t+q_{xxx}+6qq_x)\varphi(k,x,t)=0.
$$

The integral equation has the large-real-$k$ normalization $\varphi/E_k=1+O(k^{-1})$ under the stated contour regularity, so its eigenfunction is not zero for every $k$ at a fixed $(x,t)$. Consequently **$q_t+q_{xxx}+6qq_x=0$**.

Thus a time-independent contour and measure determine $\varphi$ through a linear spectral integral equation; $q=-\partial_x\int_L\varphi\,d\lambda$ then reconstructs the nonlinear solution. This is the asserted linearisation. It does not assert that sums of reconstructed nonlinear solutions are again solutions, and it depends on the given uniqueness and differentiability hypotheses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
