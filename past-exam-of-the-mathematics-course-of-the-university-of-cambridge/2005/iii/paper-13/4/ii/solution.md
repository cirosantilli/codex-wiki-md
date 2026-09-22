<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $P$ be a sphere with $g+1$ disjoint open disks removed, and form its double $S$ by gluing two copies along the boundary. Then $\chi(S)=2\chi(P)=2(1-g)$, so $S$ is an oriented closed surface of genus $g$. The [involution](../../../../../../involution.md) $\iota$ swapping the two halves fixes precisely the $g+1$ seam circles.

Use disjoint collars with coordinates $(s,t)\in\mathbb R/\mathbb Z\times(-\eta,\eta)$, where $\iota(s,t)=(s,-t)$. Choose a smooth even bump function $\chi(t)$ supported inside the collar, with $\chi(0)=1$, and choose $0<\epsilon<1$. Define an orientation-preserving diffeomorphism $R$ on each collar by $R(s,t)=(s+\epsilon\chi(t),t)$ and as the identity outside the collars. Scaling $\epsilon$ from zero gives an isotopy from the identity to $R$, so $F=R\circ\iota$ is homotopic to $\iota$.

A fixed point of $F$ in a collar would satisfy $-t=t$, hence $t=0$. Its other coordinate would then require $s+\epsilon=s$ modulo one, impossible for the chosen $\epsilon$. Outside the collars, $F=\iota$ exchanges the interiors of the halves and has no fixed points. Therefore **$\iota$ has fixed circles but is homotopic to the fixed-point-free map $F$**. This is the [fixed-point-free perturbation of a doubled-surface reflection](../../../../../../fixed-point-free-perturbation-of-a-doubled-surface-reflection.md); the construction includes genus zero, where the double is a sphere.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
