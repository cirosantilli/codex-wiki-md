<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The variable $t$ is central. To prove the [leading-coefficient proof for a central polynomial extension](../../../../../leading-coefficient-proof-for-a-central-polynomial-extension.md), let $I$ be any [right ideal](../../../../../right-ideal.md) of $R[t]$ and set

$$
L_d=\left\{a_d:\sum_{i=0}^d a_it^i\in I\right\}\subseteq R.
$$

Zero leading coefficients are allowed. Addition and right multiplication by constants show that $L_d$ is a [right ideal](../../../../../right-ideal.md). Multiplication by $t$ gives $L_d\subseteq L_{d+1}$. Since $R$ is a [right Noetherian ring](../../../../../right-noetherian-ring.md), this chain stabilizes, say at $L_N$, and each $L_d$ for $d\le N$ has finitely many generators $a_{dj}$. Choose $f_{dj}\in I$ of degree at most $d$ lifting these coefficients.

These finitely many polynomial lifts generate $I$ on the right. Indeed, for $f\in I$ of degree $m$, let $d=\min(m,N)$. Write its leading coefficient as $\sum_j a_{dj}r_j$. Then

$$
f-\sum_j f_{dj}\,r_jt^{m-d}
$$

belongs to $I$ and has degree less than $m$, because $L_m=L_d$ when $m>N$. Induction on degree reduces $f$ to a right linear combination of the chosen lifts. This proves finite generation of every [right ideal](../../../../../right-ideal.md), and hence

$$
\boxed{R\text{ right Noetherian}\Longrightarrow R[t]\text{ right Noetherian}.}
$$

Centrality matters: it is what permits the displayed leading-coefficient cancellation without twisting the coefficients.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 85](../../paper-85-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
