<h1 id="39b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expand the two central second-difference operators. The given stencil identity yields

$$
\Gamma_9u=h^2\Delta u+\frac{h^4}{12}\Delta^2u+h^6\left[\frac{u_{xxxxxx}+u_{yyyyyy}}{360}+\frac{u_{xxxxyy}+u_{xxyyyy}}{72}\right]+O(h^8).
$$

Consequently its unnormalized local residual is $\Gamma_9u-h^2f=(h^4/12)\Delta f+O(h^6)$. **The normalized Laplacian approximation has leading error $(h^2/12)\Delta f$ and is second order.** These Taylor statements require the indicated smooth [derivatives](../../../../../../derivative.md); boundary accuracy is a separate matter.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [39B](../../39b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
