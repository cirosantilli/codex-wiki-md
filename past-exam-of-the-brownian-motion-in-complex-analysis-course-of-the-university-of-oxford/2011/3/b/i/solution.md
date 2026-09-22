<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Since $f(0)=0$, the function $g(z)=f(z)/z$ extends analytically to zero by $g(0)=f'(0)$. It is bounded on the disk: outside $|z|<1/2$, $|g(z)|\leq2$, while on the closed half-radius disk its analytic extension is continuous and hence bounded.

Fix $z\ne0$ and choose $|z|<r<1$. Let $T_r$ be the first exit time of Brownian motion started at $z$ from the radius-$r$ disk. The bounded analytic martingale identity in part (a) gives

$$
g(z)=\mathbb E_z[g(Z_{T_r})].
$$

On this exit circle, $|g(Z_{T_r})|=|f(Z_{T_r})|/r\leq1/r$. The triangle inequality gives $|g(z)|\leq1/r$. Letting $r\uparrow1$ proves $|g(z)|\leq1$, and therefore

$$
\boxed{|f(z)|\leq|z|\quad\text{for all }z\in D.}
$$

At zero the claim holds by the assumed zero value. This is the [Schwarz lemma](../../../../../schwarz-lemma.md), obtained from Brownian optional stopping rather than an analytic maximum principle.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Brownian motion in complex analysis course of the University of Oxford](../../../../../brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
