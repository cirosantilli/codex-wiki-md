<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Give the generator $p$ weight one and $g-1$ weight $\omega(g)$. For $\lambda\geq0$, let $\mathbb Z_p[G]_\lambda$ be the $\mathbb Z_p$-span of

$$
p^r(g_1-1)\cdots(g_s-1)
\quad\text{with}\quad
r+\sum_{i=1}^s\omega(g_i)\geq\lambda.
$$

The identities

$$
gh-1=(g-1)+(h-1)+(g-1)(h-1)
$$

and

$$
(g-1)(h-1)-(h-1)(g-1)=gh-hg
$$

together with the filtration inequalities show that the definition is independent of how an element is expanded and that

$$
\mathbb Z_p[G]_\lambda\mathbb Z_p[G]_\mu
\subseteq\mathbb Z_p[G]_{\lambda+\mu}.
$$

Completeness and an [Ordered basis of a complete p-valued group](../../../../../ordered-basis-of-a-complete-p-valued-group.md) give separatedness through unique noncommutative power-series expansions. This is the [Lazard filtration on a group algebra](../../../../../lazard-filtration-on-a-group-algebra.md).

Multiplication by $p$ induces a central degree-one element $t$, so $\operatorname{gr}\mathbb Z_p[G]$ is a graded $\mathbb F_p[t]$-algebra. Sending the initial form of $g$ to the initial form of $g-1$ respects the Lie bracket, since the displayed algebra commutator has leading term represented by $[g,h]-1$. The universal property of the [universal enveloping algebra](../../../../../universal-enveloping-algebra.md) therefore gives the [Lazard enveloping-algebra map](../../../../../lazard-enveloping-algebra-map.md)

$$
\boxed{U_{\mathbb F_p[t]}(\operatorname{gr}G)
\twoheadrightarrow\operatorname{gr}\mathbb Z_p[G].}
$$

It is surjective because the defining filtered pieces are spanned by products of $p$ and the elements $g-1$.

For the principal congruence subgroup of $\operatorname{SL}_2(\mathbb Z_p)$, let $e=E-1$, $f=F-1$, and $h=H-1$. In the group algebra,

$$
ef-fe=EF-FE=FE\bigl([E,F]-1\bigr).
$$

The factor $FE$ is congruent to one in filtration degree zero. Direct matrix multiplication, now applied to the group commutator, gives

$$
[E,F]\equiv
\begin{pmatrix}1+p^2&0\\0&1-p^2\end{pmatrix}
\equiv H^p\pmod{G_3}.
$$

Consequently $ef-fe\equiv H^p-1\equiv p(H-1)=ph$ modulo $\mathbb Z_p[G]_3$. The same argument starts from

$$
he-eh=EH\bigl([H,E]-1\bigr),
\qquad
hf-fh=FH\bigl([H,F]-1\bigr).
$$

Using $(1+p)^{-1}=1-p+p^2+O(p^3)$ in the two matrix commutators gives

$$
[H,E]-1\equiv2p(E-1),
\qquad
[H,F]-1\equiv-2p(F-1)
\pmod{G_3}.
$$

Since the prefactors $EH,FH$ may again be replaced by one at this precision, we obtain  
Therefore

$$
\boxed{ef-fe\equiv ph,\qquad he-eh\equiv2pe,\qquad hf-fh\equiv-2pf
\pmod{\mathbb Z_p[G]_3}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 145](../../paper-145-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
