<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

Write a reduced positive definite [binary quadratic form](../../../../../binary-quadratic-form.md) as $[a,b,c]=ax^2+bxy+cy^2$, with $|b|\leq a\leq c$ and $b\geq0$ on the reduction boundaries. Since $4ac-b^2=20$, reduction gives $3a^2\leq20$, so $a=1$ or two. The middle coefficient is even. For $a=1$, only $b=0$ is possible, yielding $c=5$. For $a=2$, $b=0$ would give a noninteger $c$, while $b=\pm2$ gives $c=3$; the boundary convention selects $b=2$. Thus the two reduced forms are

$$
\boxed{x^2+5y^2,\qquad 2x^2+2xy+3y^2.}
$$

A positive odd integer $n$ is properly represented by some integer form of discriminant $d$ exactly when $b^2\equiv d\pmod{4n}$ has a solution. For a specified proper equivalence class, the more precise criterion is that $[n,b,(b^2-d)/(4n)]$ belong to that class for some such $b$. Indeed, a primitive representing vector extends to an $SL_2(\mathbb Z)$ basis change, making the leading coefficient $n$; conversely that form represents $n$ at the primitive vector $(1,0)$.

For [primes](../../../../../prime-number.md) $p\nmid10$, the existence criterion is $(-20/p)=1$, because the congruence modulo four is compatible with an even middle coefficient. Quadratic reciprocity gives $(-20/p)=(-1/p)(p/5)$, so the split possibilities are $p\equiv1,3,7,9\pmod{20}$. Any proper representing form reduces to one of the two listed forms. Odd values of $x^2+5y^2$ are one modulo four; odd values of $2x^2+2xy+3y^2$ require odd $y$ and are three modulo four. These distinguish the two classes. Consequently

$$
\boxed{p=x^2+5y^2\text{ for a prime }p\ne2,5\iff p\equiv1\text{ or }9\pmod{20}.}
$$

A [representation](../../../../../group-representation.md) of a [prime](../../../../../prime-number.md) is automatically proper: a common divisor of $x,y$ would have its square divide $p$.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
