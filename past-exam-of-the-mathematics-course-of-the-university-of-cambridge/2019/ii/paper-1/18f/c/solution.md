<h1 id="18f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The actions on the ordered pair $(x,y)$ satisfy

$$
\sigma^4=1,
\qquad
\tau^2=1,
\qquad
\tau\sigma\tau=\sigma^{-1}.
$$

Thus every element of $G$ has the form $\sigma^i$ or $\tau\sigma^i$ for $0\leq i<4$, so $|G|\leq8$. Their actions are

$$
\begin{array}{c|cccccccc}
g&1&\sigma&\sigma^2&\sigma^3&\tau&\tau\sigma&\tau\sigma^2&\tau\sigma^3\\ \hline
(g(x),g(y))
&(x,y)&(y,-x)&(-x,-y)&(-y,x)
&(x,-y)&(-y,-x)&(-x,y)&(y,x).
\end{array}
$$

Because $x,y$ are [algebraically independent elements](../../../../../../algebraically-independent-elements.md) over $\mathbb Q$, these eight substitutions are distinct. Hence

$$
\boxed{|G|=8},
$$

and the presentation identifies $G$ with the [dihedral group](../../../../../../dihedral-group.md) $D_8$.

Put

$$
u=x^2+y^2,
\qquad
v=x^2y^2.
$$

Both generators $\sigma$ and $\tau$ fix $u$ and $v$, so for $F=\mathbb Q(u,v)$,

$$
F\subseteq K^G.
$$

The elements $x^2$ and $y^2$ are the two roots of

$$
T^2-uT+v,
$$

so $[F(x^2,y^2):F]\leq2$. Adjoining first $x$ and then $y$ takes at most two quadratic extensions, and the [tower law](../../../../../../tower-law.md) gives

$$
[K:F]\leq2\cdot2\cdot2=8.
$$

Part (b) gives $8=|G|\leq[K:K^G]$. Since $F\subseteq K^G\subseteq K$, another use of the tower law gives

$$
8\leq[K:K^G]\leq[K:F]\leq8.
$$

All inequalities are equalities and $[K^G:F]=1$. Therefore

$$
\boxed{K^G=\mathbb Q(x^2+y^2,x^2y^2)},
$$

the [dihedral fixed field of a two-variable rational function field](../../../../../../dihedral-fixed-field-of-a-two-variable-rational-function-field.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18F](../../18f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
