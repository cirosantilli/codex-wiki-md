<h1 id="9e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove by induction on $n$ that every submodule $N\subseteq R^n$ is free. The case $n=0$ is immediate. Let $\pi:R^n\to R$ be projection onto the first coordinate. Since $R$ is a principal [ideal](../../../../../../../ideal.md) domain,

$$
\pi(N)=dR
$$

for some $d$. If $d=0$, then $N\subseteq R^{n-1}$ and induction applies. Otherwise choose $x\in N$ with $\pi(x)=d$. For every $y\in N$, write $\pi(y)=rd$; then $y-rx\in\ker(\pi|_N)$. Also $Rx\cap\ker(\pi|_N)=0$ because $R$ is a domain and $d\ne0$. Therefore

$$
N=Rx\oplus\ker(\pi|_N).
$$

The kernel is a submodule of $R^{n-1}$ and is free by induction, while $Rx\cong R$. Hence $N$ is free. This is the [submodule theorem for free modules over a principal ideal domain](../../../../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md).

If $P$ is finitely generated and projective, choose a surjection $f:R^n\to P$. Projectivity supplies $h:P\to R^n$ with $f\circ h=\operatorname{id}_P$, so

$$
R^n=\ker f\oplus h(P).
$$

**Thus $P\cong h(P)$ is a submodule of the finitely generated free module $R^n$, and the result just proved shows that $P$ is free.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9E](../../../9e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
