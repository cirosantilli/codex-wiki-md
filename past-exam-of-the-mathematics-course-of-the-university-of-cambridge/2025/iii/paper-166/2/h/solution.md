<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

For an integer $m>1$, let $\alpha_m$ be a root of

$$
f_m(X)=X^2-2mX+m.
$$

Its roots are

$$
R_m=m+\sqrt{m^2-m}>1,
\qquad
r_m=m-\sqrt{m^2-m}\in(0,1).
$$

The polynomial is [irreducible](../../../../../../irreducible-polynomial.md) over $\mathbb Q$: its discriminant is $4m(m-1)$, and the product of the coprime consecutive integers $m$ and $m-1$ cannot be a square unless both are squares, which is impossible for consecutive positive squares beyond $0,1$.

The [height-Mahler measure formula](../../../../../../height-mahler-measure-formula.md) gives

$$
H(\alpha_m)^2=R_m.
$$

Both [algebraic conjugates](../../../../../../conjugate-element-field-theory.md) of $\alpha_m+1$ exceed $1$, so

$$
H(\alpha_m+1)^2
=(R_m+1)(r_m+1)
=f_m(-1)=3m+1.
$$

Consequently

$$
\frac{H(\alpha_m+1)}{H(\alpha_m)}
=\sqrt{\frac{3m+1}{R_m}}
\longrightarrow\sqrt{\frac32}>1.
$$

Fix, for example, $\delta=1/10$. For all sufficiently large $m$, the ratio is larger than $1+\delta$ by a fixed margin, while $H(\alpha_m)\to\infty$. Hence, for every $C>0$, some sufficiently large $m$ satisfies

$$
\boxed{H(\alpha_m+1)>(1+\delta)H(\alpha_m)+C.}
$$

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
