<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $D=\{(\omega,t):\omega\geq t\}$ and let $\mathcal C$ denote the proposed family of [sets](../../../../../../set-split.md). This is a [sigma-algebra](../../../../../../sigma-algebra.md): complements replace $T$ and $A$ by their complements, and countable unions replace them by their unions. For a generating [predictable rectangle](../../../../../../predictable-rectangle.md) $B\times(s,u]$, part (a) says either $B\subseteq(0,s)$ or $B^c\subseteq(0,s)$. In the first case its trace on $D$ is empty; in the second it is exactly $D\cap(\Omega\times(s,u])$. Its trace on $D^c$ is always product-Borel. Hence $\mathcal P\subseteq\mathcal C$.

For the reverse inclusion, $X$ is left-continuous and adapted, so $D=\{X=1\}$ belongs to the [predictable sigma-algebra](../../../../../../predictable-sigma-algebra.md). Every deterministic [Borel set](../../../../../../borel-set.md) in time also belongs to that [sigma-algebra](../../../../../../sigma-algebra.md), hence $D\cap(\Omega\times T)$ is predictable. For a product rectangle $E\times T$,

$$
(E\times T)\cap D^c=\bigcup_{s\in\mathbb Q_{>0}}\bigl((E\cap(0,s))\times(s,\infty)\bigr)\cap(\Omega\times T).
$$

Each term is predictable because $E\cap(0,s)\in\mathcal F_s$. Every pair with $\omega<t$ lies in such a term by choosing $\omega<s<t$. The class of product-Borel [sets](../../../../../../set-split.md) $A$ for which $A\cap D^c$ is predictable is a [sigma-algebra](../../../../../../sigma-algebra.md) containing the product rectangles, so it contains $\mathcal F\otimes\mathcal F$. Thus

$$
\boxed{\mathcal P=\{(D\cap(\Omega\times T))\cup(D^c\cap A):T\in\mathcal F,\ A\in\mathcal F\otimes\mathcal F\}.}
$$

This [survival-observation predictable sigma-algebra](../../../../../../survival-observation-predictable-sigma-algebra.md) expresses a sharp distinction: before and at the lifetime the only observable coordinate is time, whereas strictly after it the lifetime is known.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
