<h1 id="11i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By [Fermat's little theorem](../../../../../../fermat-little-theorem.md),

$$
g(x,y,z)=1-f(x,y,z)^{p-1}\equiv
\begin{cases}
1&\text{if }f(x,y,z)\equiv0\pmod p,\\
0&\text{otherwise}.
\end{cases}
$$

Thus the sum of $g$ over $\mathbb F_p^3$ counts, modulo $p$, the triples on which the [ternary quadratic form](../../../../../../ternary-quadratic-form.md) $f$ vanishes.

Expand $f^{p-1}$ with the [multinomial theorem](../../../../../../multinomial-theorem.md). A term indexed by $r+s+t=p-1$ contributes a constant multiple of

$$
S_{2r}S_{2s}S_{2t}.
$$

At least one of $r,s,t$ is strictly less than $(p-1)/2$. Its corresponding exponent is therefore in $\{0,1,\ldots,p-2\}$, so part (b), including its $k=0$ case, makes that power sum zero modulo $p$. Every term in the expansion consequently vanishes after summation. The constant term contributes $p^3\equiv0$, and therefore

$$
\boxed{\sum_{x,y,z\in\mathbb F_p}g(x,y,z)\equiv0\pmod p.}
$$

The zero triple is one solution of $f=0$. If it were the only solution, the displayed sum would be congruent to $1$ rather than $0$. Hence there is another triple $(x,y,z)$, not all divisible by $p$, satisfying

$$
\boxed{a x^2+b y^2+c z^2\equiv0\pmod p.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11I](../../11i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
