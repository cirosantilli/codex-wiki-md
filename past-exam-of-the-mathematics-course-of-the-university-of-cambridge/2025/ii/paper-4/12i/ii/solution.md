<h1 id="12i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n\geq0$, put

$$
S_n=\{x\in\mathbb R:F^{(n)}(x)=0\},
\qquad E_n=\operatorname{int}S_n.
$$

Each $S_n$ is closed, the hypothesis gives $\mathbb R=\bigcup_nS_n$, and $E_n\subset E_{n+1}$ because a function that vanishes on an open set has derivative zero there.

The open set

$$
\Omega=\bigcup_{n\geq0}E_n
$$

is dense. Indeed, inside any nonempty [open interval](../../../../../../open-interval.md) choose a [nondegenerate](../../../../../../nondegenerate-interval.md) closed subinterval $J$. The [complete metric space](../../../../../../complete-metric-space.md) $J$ is covered by the [closed sets](../../../../../../closed-set.md) $J\cap S_n$, so the [Baire's theorem](../../../../../../baire-category-theorem.md) makes one of them contain a relative open interval, which lies in some $E_n$.

On each connected component $I$ of $\Omega$, the function $F$ is one polynomial. To see this, any compact subinterval $K\subset I$ is covered by the increasing family $(E_n)$. A finite subcover therefore gives $K\subset E_N$ for some $N$, and $F^{(N)}=0$ on $K$. Hence $F$ is polynomial on $K$; overlapping compact intervals force these polynomials to agree throughout $I$.

Let $D=\mathbb R\setminus\Omega$. This closed set has no isolated points. Otherwise, on the two sides of an isolated point $x$, $F$ would equal polynomials. Smoothness makes all their one-sided derivatives agree at $x$, so the two polynomials are identical and extend across $x$. Some derivative would then vanish on a neighborhood of $x$, contrary to $x\in D$.

Suppose that $D$ is nonempty. It is complete and

$$
D=\bigcup_{n\geq0}(D\cap S_n)
$$

is a countable closed cover. A second application of Baire's theorem gives an index $k$ and an open interval $U_0$ such that

$$
\varnothing\ne D\cap U_0\subset S_k.
$$

Choose $x_0\in D\cap U_0$ and a bounded open interval $U$ centred at $x_0$ whose closure lies in $U_0$.

Because $D$ has no isolated points, every $x\in D\cap U$ is approached by distinct points of $D\cap U$. Difference quotients first give $F^{(k+1)}(x)=0$, and induction gives

$$
F^{(m)}(x)=0\qquad(m\geq k, x\in D\cap U).
$$

No component of $\Omega$ meeting $U$ can cross $x_0$, so it has an endpoint in $D\cap U$. If its polynomial had degree $d\geq k$, then its $d$th derivative would approach a nonzero constant at that endpoint, contradicting the preceding display. Its degree is therefore less than $k$, so $F^{(k)}$ also vanishes on the part of that component in $U$. We conclude that $F^{(k)}=0$ throughout $U$, which says $U\subset E_k\subset\Omega$ and contradicts $D\cap U\ne\varnothing$.

**Thus $D$ is empty. The whole line is the single component of $\Omega$, and the argument above shows that $F$ is one polynomial on $\mathbb R$. This is the [smooth function with a pointwise vanishing derivative](../../../../../../smooth-function-with-a-pointwise-vanishing-derivative.md) theorem.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12I](../../12i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
