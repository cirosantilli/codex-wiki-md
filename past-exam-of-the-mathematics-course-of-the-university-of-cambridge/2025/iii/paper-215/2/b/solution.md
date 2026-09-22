<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The graph has $\asymp n^4$ vertices, bounded degrees, and stationary masses $\asymp n^{-4}$. Split any set into components that do not communicate in one step and use part (a)(ii). A connected component of stationary mass $r\leq1/2$ has $O(rn^4)$ vertices. The planar grid isoperimetric bound supplies at least $c\sqrt{rn^4}$ boundary edges unless the component fills most of one layer; in that case the $\asymp n^2$ interlayer edges give the same order. Thus

$$
\Phi_*(r)\gtrsim\frac1{n^2\sqrt r}.
$$

The conductance-profile mixing bound for a lazy chain now gives

$$
t_{\mathrm{mix}}
\lesssim\int_{4\pi_{\min}}^{1/2}
\frac{du}{u\Phi_*(u)^2}+t_{\mathrm{rel}}
\lesssim n^4.
$$

Here $\Phi_*\gtrsim n^{-2}$ also gives $t_{\mathrm{rel}}\lesssim n^4$ by [Cheeger inequality](../../../../../../cheeger-inequality.md). Hence $t_{\mathrm{mix}}\lesssim n^4$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
