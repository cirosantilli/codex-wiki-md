# Kernel of localization away from one plus an ideal

↑ **Parent:** [Localization of a module](localization-of-a-module.md)

Let $R$ be [Noetherian](noetherian-ring.md), $I\subseteq R$ an ideal, $S=1+I$, and $M$ a finitely generated $R$-module. Then

$$
\ker(M\longrightarrow S^{-1}M)=\bigcap_{j\geq1}I^jM.
$$

If $(1+a)m=0$ with $a\in I$, then $m=(-a)^jm\in I^jM$ for every $j$. Conversely, apply the [Artin-Rees lemma](artin-rees-lemma.md) to $Rm\subseteq M$. For sufficiently large $c$ it gives

$$
m\in I^{c+1}M\cap Rm=I(I^cM\cap Rm)\subseteq I(Rm),
$$

so $m=am$ for some $a\in I$ and $(1-a)m=0$.

**Table of contents**

- [Non-Noetherian failure of the intersection formula for localization](non-noetherian-failure-of-the-intersection-formula-for-localization.md)

## ↑ Ancestors (7)

1. [Localization of a module](localization-of-a-module.md)
2. [Localization of a ring](localization-of-a-ring.md)
3. [Commutative algebra](commutative-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
