<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First, equality of two $U_0$ values forces equality of the corresponding $V_0$ values: neither strict comparison holds for $U_0$, and the same is then true for $V_0$ in both directions. Thus $V_0=g\circ U_0$ for a well-defined [strictly increasing function](../../../../../../strictly-increasing-function.md) $g$ on $J=U_0(\mathcal P)$. Since $\mathcal P$ is a [convex set](../../../../../../convex-set.md) and $U_0,V_0$ are [affine functions](../../../../../../affine-function.md), $J$ is a [real interval](../../../../../../interval-mathematics.md) and

$$
g(pu+(1-p)v)=pg(u)+(1-p)g(v),\qquad u,v\in J,\quad0\leq p\leq1.
$$

If $J$ contains $u<v$, let $a=[g(v)-g(u)]/(v-u)>0$ and $b=g(u)-au$. The mixture identity gives $g(w)=aw+b$ for $w\in[u,v]$. For $w>v$, express $v$ as a [convex combination](../../../../../../convex-combination.md) of $u$ and $w$ and solve the same identity for $g(w)$; for $w<u$, express $u$ as a mixture of $w$ and $v$. Hence the formula holds on all of $J$, not merely between the chosen anchors. We obtain [positive affine uniqueness of affine preference representations](../../../../../../positive-affine-uniqueness-of-affine-preference-representations.md):

$$
\boxed{V_0(\lambda)=aU_0(\lambda)+b\quad\text{for every }\lambda\in\mathcal P,\qquad a>0.}
$$

If $U_0$ is constant, the same comparisons force $V_0$ to be constant; choose $a=1$ and the appropriate $b$. If the probability-measure set is empty, the assertion is vacuous. These degenerate cases do not require distinct anchors.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
