<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $a=\mathbb E_pM_m=\sum_{|x|=m}\tau_p(x)$. If $|u|\geq m$, an open self-avoiding path from $0$ to $u$ first meets the $\ell^1$ sphere of radius $m$ at some $x$. Its portions from $0$ to $x$ and from $x$ to $u$ use disjoint edge sets. The [Van den Berg-Kesten inequality](../../../../../../van-den-berg-kesten-inequality.md) and translation invariance therefore give

$$
\tau_p(u)
\leq\sum_{|x|=m}\tau_p(x)\tau_p(u-x).
$$

Let $s_k=\sup_{|u|\geq km}\tau_p(u)$. Since $|u-x|\geq|u|-m$, the last inequality gives $s_k\leq a s_{k-1}$ and $s_0\leq1$. Induction yields

$$
\boxed{\mathbb P_p(0\longleftrightarrow u)=\tau_p(u)
\leq a^{\lfloor|u|/m\rfloor}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 212](../../../paper-212-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
