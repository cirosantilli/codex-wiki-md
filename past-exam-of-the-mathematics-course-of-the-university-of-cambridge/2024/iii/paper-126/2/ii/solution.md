<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $X=U\cup V$, the [Mayer-Vietoris sequence for sheaf cohomology](../../../../../../mayer-vietoris-sequence-for-sheaf-cohomology.md) is the long exact sequence

$$
0\to H^0(X,\mathcal F)\to H^0(U,\mathcal F)\oplus H^0(V,\mathcal F)\to H^0(U\cap V,\mathcal F)\to H^1(X,\mathcal F)\to\cdots.
$$

We prove the required vanishing by induction on the number $m$ of open sets. The case $m=1$ is an assumption. Put $U=U_1\cup\cdots\cup U_{m-1}$ and $V=U_m$. The induction hypothesis gives $H^p(U,\mathcal F)=0$ for every $p$. The intersections $U_i\cap U_m$ cover $U\cap V$, and every nonempty finite intersection among them is one of the intersections in the hypothesis, so the same induction gives $H^p(U\cap V,\mathcal F)=0$. We also have $H^p(V,\mathcal F)=0$. Exactness of the Mayer-Vietoris sequence now yields

$$
\boxed{H^p(X,\mathcal F)=0\quad\text{for every }p\ge0.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
