<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $z_0\ne0$ be an equality point and set $c=g(z_0)$, so $|c|=1$. For any $|z_0|<r<1$, the same Brownian exit identity gives

$$
1=\operatorname{Re}(\overline c\,g(z_0))
=\mathbb E_{z_0}\operatorname{Re}(\overline c\,g(Z_{T_r})).
$$

Part (i) gives $|g|\leq1$, so the real random variable in the expectation is at most one. Equality of its mean to one forces $g(Z_{T_r})=c$ almost surely. By the scaled version of the exit density from Question 2, every nonempty arc of the exit circle has positive probability. Continuity of $g$ on that circle therefore implies $g=c$ at every boundary point of the radius-$r$ disk.

For any $w$ inside that circle, the Brownian exit identity now gives $g(w)=\mathbb E_wg(Z_{T_r})=c$. Letting $r$ increase to one makes this true throughout $D$. Writing $c=e^{i\theta}$ yields

$$
\boxed{f(w)=we^{i\theta}\quad\text{for all }w\in D.}
$$

This completes the equality case of the [Brownian proof of the Schwarz lemma](../../../../../brownian-proof-of-the-schwarz-lemma.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
