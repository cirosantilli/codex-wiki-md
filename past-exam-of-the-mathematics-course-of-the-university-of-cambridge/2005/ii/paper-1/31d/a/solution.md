<h1 id="31d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $C(z)=(2\pi i)^{-1}\int_L\phi(\tau)/(\tau-z)\,d\tau$, with interior and exterior boundary values $C_+,C_-$. The [Sokhotski–Plemelj formula](../../../../../../sokhotski-plemelj-theorem.md) gives $\phi=C_+-C_-$ and $C_++C_-=(\pi i)^{-1}\operatorname{PV}\int_L\phi(\tau)/(\tau-t)\,d\tau$. Write $K=(\pi i)^{-1}\int_L(\tau+1/\tau)\phi(\tau)\,d\tau$ for the nonlocal scalar moment. Substitution into the [integral](../../../../../../integral.md) equation yields

$$
2tC_+-2(t^2-1)C_-=t-1+K.
$$

Thus the associated scalar [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md) is

$$
\boxed{C_+(t)=\frac{t^2-1}{t}C_-(t)+\frac{t-1+K}{2t},\qquad C_-(z)=O(z^{-1})\text{ at infinity}.}
$$

The functions are analytic in their respective interior/exterior domains, and $K$ must ultimately equal the moment of the recovered jump; it is not an independently specified free constant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31D](../../31d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
