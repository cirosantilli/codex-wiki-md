<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the final low steady value $Z_s=\beta_{\rm low}/\alpha$, the first crossing of $Z_s/2$ occurs during high production if $F(1-e^{-\alpha d})\ge1/2$. Solving $F(1-e^{-\alpha t_{1/2}})=1/2$ then gives, for either motif,

$$
\boxed{t_{1/2}=\frac1\alpha\ln\frac{2F}{2F-1}
\simeq\frac1{2\alpha F}\quad(F\gg1).}
$$

This [half-final response of a graded incoherent feed-forward loop](../../../../half-final-response-of-a-graded-incoherent-feed-forward-loop.md) is a first-crossing measure. A simple output produced at the final low rate from zero would instead take $(\ln2)/\alpha$. This comparison explains the acceleration of the first half-final response, not the time needed to settle after a potentially large overshoot.

The condition matters because the source does not fix $K_{yz}/Y_s$. Define $\delta=1-e^{-\alpha d}$, equal to $h$ for [I1 incoherent feed-forward loop](../../../../i1-incoherent-feed-forward-loop.md) and $1-h$ for [I4 incoherent feed-forward loop](../../../../i4-incoherent-feed-forward-loop.md). If the high phase ends before half-final output is reached, solve the second branch of part (a) instead:

$$
\boxed{t_{1/2}=\begin{cases}
\alpha^{-1}\ln[2F/(2F-1)],&F\delta\ge1/2,\\
d+\alpha^{-1}\ln[2(1-F\delta)],&F\delta<1/2.
\end{cases}}
$$

The expressions agree at the boundary. The $F$-only answer is therefore valid for both motifs when $F\min(h,1-h)\ge1/2$, as holds for large F and a fixed interior threshold. Merely saying $F\gg1$ does not cover a threshold that approaches zero or one even faster. If the Y threshold is never crossed, the assumed final low state itself changes and one must reconsider the [steady state](../../../../steady-state.md) before using this response-time definition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
