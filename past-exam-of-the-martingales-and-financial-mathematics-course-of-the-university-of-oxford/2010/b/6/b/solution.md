<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the auxiliary diffusion with generator $(rS+\delta)\partial_S+(\sigma^2S^2/2)\partial_{SS}$. Applying [Itô's formula](../../../../../ito-s-lemma.md) to $e^{-r(v-t)}V(v,\widehat S_v)$ makes its drift zero by part (a), leaving only $e^{-r(v-t)}\sigma\widehat S_vV_S\,dW_v$. Under the usual integrability conditions, localization and expectation give the [Feynman-Kac formula](../../../../../feynman-kac-formula.md)

$$
\boxed{V(t,S_t)=\mathbb E\left[e^{-r(T-t)}\Psi(\widehat S_T)\mid\widehat S_t=S_t\right],\quad
 d\widehat S_v=(r\widehat S_v+\delta)dv+\sigma\widehat S_vdW_v.}
$$

For polynomial-growth payoffs, the linear diffusion has the finite moments needed for this martingale argument. Its pricing drift includes the cash storage cost as an additive term.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
