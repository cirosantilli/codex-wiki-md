<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the assumed [finite-field character approximation](../../../../../../finite-field-character-approximation.md) with error $\epsilon/2$. We obtain $k\leq4q/\epsilon^2$ characters $\gamma_i$ and a function

$$
P=\frac1k\sum_{i=1}^kc_i\gamma_i\,\|\widehat f\|_{\ell^1}
$$

such that $\|f-P\|_{L^q}\leq(\epsilon/2)\|\widehat f\|_{\ell^1}$. Let

$$
W=\bigcap_{i=1}^k\ker\gamma_i.
$$

Each character has a kernel of codimension at most one, so $\operatorname{codim}W\leq k\leq4q/\epsilon^2$. For $x\in W$, $\tau_xP=P$, and translation invariance of the $L^q$ norm gives

$$
\boxed{\|\tau_xf-f\|_{L^q}
\leq\|\tau_x(f-P)\|_{L^q}+\|f-P\|_{L^q}
\leq\epsilon\|\widehat f\|_{\ell^1}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
