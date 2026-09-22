<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $X=\mathbb R$, $U=(0,1)$, and let $\mathcal F$ be the [skyscraper sheaf](../../../../../../skyscraper-sheaf.md) with value a nonzero abelian group $A$ at $p=3/4$. Cover $V=(-1,1)$ by $V_1=(-1,2/3)$ and $V_2=(1/2,1)$. The presheaf gives $(j^p\mathcal F)(V)=0=(j^p\mathcal F)(V_1)$ and $(j^p\mathcal F)(V_2)=A$. A nonzero section on $V_2$ and the zero section on $V_1$ agree on the overlap, whose skyscraper sections vanish, but cannot be glued on $V$. Thus $j^p\mathcal F$ need not be a sheaf.

[Sheafification](../../../../../../sheafification.md) preserves [stalks](../../../../../../stalk-of-a-sheaf.md). If $P\in U$, neighborhoods contained in $U$ are cofinal, so $(j^p\mathcal F)_P=\mathcal F_P$. If $P\notin U$, no neighborhood of $P$ lies in $U$, so every term defining the presheaf stalk is zero. Therefore

$$
(j_!\mathcal F)_P\cong
\begin{cases}
\mathcal F_P,&P\in U,\\
0,&P\notin U.
\end{cases}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
