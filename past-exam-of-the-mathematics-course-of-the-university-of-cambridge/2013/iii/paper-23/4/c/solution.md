<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $D_0=|D|$. The reference to part (c) in the printed hint is a reference to the positive-coefficient function from part (b). For $\sigma>1$ close to one, the preceding positivity and the supplied partial-fraction expansion give

$$
0\le\frac1{\sigma-1}+C\log D_0-\sum_{\substack{\beta\text{ real}\text{near }1}}\frac1{\sigma-\beta}.
$$

All omitted zero terms have nonnegative real parts because their real parts are at most one. The $O(1)$ zeta-pole remainder is included in $C\log D_0$, increasing the absolute constant if needed; a nonprincipal primitive real [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) is at least three.

Suppose there were two real zeros, counted with multiplicity, with $\beta\ge1-c/\log D_0$. Set $\sigma=1+a/\log D_0$. Division by $\log D_0$ gives

$$
0\le\frac1a+C-\frac2{a+c}.
$$

Choose $C\ge1$, $a=1/(4C)$ and $c=a/4$. The right side is strictly negative. Thus

$$
\boxed{\text{at most one real zero, necessarily simple, in }[1-c/\log|D|,1].}
$$

This is the [uniqueness of a possible exceptional real Dirichlet zero](../../../../../../uniqueness-of-a-possible-exceptional-real-dirichlet-zero.md). It proves uniqueness, rather than existence of such a zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
