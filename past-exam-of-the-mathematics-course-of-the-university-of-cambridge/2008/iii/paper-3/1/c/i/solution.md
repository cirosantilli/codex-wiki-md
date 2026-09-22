<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In the finite-dimensional setting, let $R(a,b)$ denote the irreducible $\mathfrak{sl}_3$ [highest-weight representation](../../../../../../../highest-weight-representation.md) of highest weight $aL_1-bL_3$, where $a,b$ are nonnegative [integers](../../../../../../../integer.md). Thus $(a,b)$ are its [Dynkin labels](../../../../../../../dynkin-label.md). The target $\lambda=L_1-2L_3$ has labels $(1,2)$. Write the highest-weight difference in [simple roots](../../../../../../../simple-root.md) as

$$
(aL_1-bL_3)-\lambda=r(L_1-L_2)+s(L_2-L_3),\qquad
r=\frac{2a+b-4}{3},\quad s=\frac{a+2b-5}{3}.
$$

The [dominant weight multiplicity formula for sl3](../../../../../../../dominant-weight-multiplicity-formula-for-sl3.md) gives zero unless $r,s$ are nonnegative [integers](../../../../../../../integer.md), and otherwise gives

$$
\dim R(a,b)_\lambda=1+\min(a,b,r,s).
$$

For completeness, this multiplicity is an actual count. In the [sl3 interlacing character formula](../../../../../../../sl3-interlacing-character-formula.md), use top row $(a+b,b,0)$ and bottom entry $s+3$; the target diagonal exponents are $(s+3,s+2,s)$. The middle row $(P,Q)$ obeys $P+Q=2s+5$ and

$$
\max\{b,2s+5-b,s+3\}\leq P\leq\min\{a+b,2s+5\}.
$$

Each allowable integral $P$ gives one [Gelfand–Tsetlin basis](../../../../../../../gelfand-tsetlin-basis.md) vector. Subtracting the lower bound from the upper bound gives the minimum of $a,s,r,r+3,b,s+2$, which reduces to $\min(a,b,r,s)$. This proves the displayed multiplicity formula in the case at hand.

Since both summands have a nonzero [weight space](../../../../../../../weight-space.md) and their dimensions at $\lambda$ sum to three, their multiplicities must be one and two. For multiplicity one, the minimum is zero. The cases $a=0$ and $b=0$ give $(0,4+3j)$ and $(5+3j,0)$; the remaining cases $r=0$ or $s=0$ give $(1,2)$ and $(3,1)$. Hence the full family is

$$
\mathcal C_1=\{R(0,4+3j),R(5+3j,0):j\geq0\}\cup\{R(1,2),R(3,1)\}.
$$

For multiplicity two, the minimum is one. The cases $a=1$ and $b=1$ give $(1,5+3j)$ and $(6+3j,1)$; the remaining cases $r=1$ or $s=1$ give $(2,3)$ and $(4,2)$. Thus

$$
\mathcal C_2=\{R(1,5+3j),R(6+3j,1):j\geq0\}\cup\{R(2,3),R(4,2)\}.
$$

The minimum conditions exhaust all cases and each listed module has the stated multiplicity. **All candidate unordered pairs are $\boxed{\{U,V\}\text{ with }U\in\mathcal C_1,\ V\in\mathcal C_2}$.** There are infinitely many at this stage; the question imposes no upper bound on their highest weights.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
