<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [boundary Schauder estimate](../../../../../../../boundary-schauder-estimate.md) is

$$
\|u\|_{C^{2,\alpha}(\overline{B_{1/2}^+})}
\leq C\left(
\|u\|_{C^0(\overline{B_1^+})}
+\|f\|_{C^{0,\alpha}(\overline{B_1^+})}
+\|\varphi\|_{C^{2,\alpha}(\overline{B_1^+})}
\right),
$$

where $C$ depends only on the dimension, $\alpha$, the ellipticity constants, and the coefficient Hölder norms.

Subtract a $C^{2,\alpha}$ extension of $\varphi$ to reduce to a function $v$ with zero data on the flat boundary; this changes the forcing by a controlled $C^{0,\alpha}$ term. The key local estimate is that for every $\delta>0$,

$$
[D^2v]_{\alpha;B_{1/2}^+}
\leq\delta[D^2v]_{\alpha;B_1^+}
+C_\delta\left(\|v\|_{C^2(B_1^+)}+\|Lv\|_{C^{0,\alpha}(B_1^+)}\right).
$$

To prove it, argue by contradiction. A failing normalized sequence has points $x_k,y_k$ at which the second-derivative Hölder quotient stays nonzero. Set $r_k=|x_k-y_k|$, subtract the appropriate second-order [Taylor polynomial](../../../../../../../taylor-polynomial.md), and rescale space by $r_k$ and the functions by $r_k^{2+\alpha}[D^2v_k]_\alpha$. Necessarily $r_k\to0$.

If the rescaled distance to the flat boundary tends to infinity, the domains converge to all of $\mathbb R^n$; otherwise they converge to a half-space. Coefficient compactness freezes the principal matrix, while the normalized right-hand sides converge locally uniformly to zero. A linear change of variables turns every limiting equation into the [Laplace equation](../../../../../../../laplace-equation.md). In the whole-space case the [polynomial-growth Liouville theorem for harmonic functions](../../../../../../../polynomial-growth-liouville-theorem-for-harmonic-functions.md) makes the limit a polynomial of degree at most two. In the half-space case the zero boundary data permit [odd reflection](../../../../../../../odd-reflection.md) across the flat boundary, after which the same theorem applies. The subtracted Taylor normalization forces that polynomial to vanish to second order, contradicting the nonzero limiting Hölder oscillation.

Apply the local estimate on all interior balls and boundary half-balls. The interior and boundary forms of the [Simon absorption lemma](../../../../../../../simon-absorption-lemma.md) absorb the term multiplied by $\delta$, while the [Hölder interpolation inequality](../../../../../../../holder-interpolation-inequality.md) absorbs the remaining lower $C^2$ norm into the top seminorm and the $C^0$ norm. Restoring $\varphi$ yields the displayed estimate.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
