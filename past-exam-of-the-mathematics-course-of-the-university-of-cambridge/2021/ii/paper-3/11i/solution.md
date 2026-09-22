<h1 id="11i/solution">Solution</h1>

↑ **Parent:** [11I](../11i.md)

Two integral binary quadratic forms are properly equivalent when one is obtained from the other by a change of variables in $SL_2(\mathbb Z)$. For a negative discriminant $d\equiv0,1\pmod4$, the [class number of binary quadratic forms](../../../../../class-number-of-a-negative-discriminant.md) $h(d)$ is the number of proper equivalence classes of primitive positive-definite forms of discriminant $d$.

If $f$ properly represents $m$, then $f(r,s)=m$ for coprime $r,s$. Extend $(r,s)^T$ to a matrix in $SL_2(\mathbb Z)$; after the associated variable change, the coefficient of $x^2$ is $m$, so the transformed form is

$$
mx^2+bxy+cy^2.
$$

The converse follows by evaluating this form at $(1,0)$.

Such a form has discriminant $d$ precisely when

$$
b^2-4mc=d,
$$

so it exists exactly when $b^2\equiv d\pmod{4m}$. Thus $m$ is properly represented by some form of discriminant $d$ exactly when $d$ is a square modulo $4m$.

Now let $d=1-4A$. If $n^2+n+A$ is composite for $0\leq n\leq A-2$, it has a prime divisor $p<A$, and

$$
d=(2n+1)^2-4(n^2+n+A)\equiv(2n+1)^2\pmod{4p}.
$$

Conversely, if $d$ is a square modulo $4p$ for a prime $p<A$, choose an odd square root $2n+1$ with $0\leq n<p$. Then $p\mid n^2+n+A$ and $n\leq A-2$, so that value is composite.

Finally, reduction theory says that every nonprincipal positive-definite class of discriminant $1-4A$ has a reduced representative whose leading coefficient has a prime divisor $p<A$ for which $d$ is a square modulo $4p$. Conversely such a prime produces a represented form not equivalent to the principal form $x^2+xy+Ay^2$. Combining this with the preceding equivalence gives

$$
\boxed{h(1-4A)=1\iff n^2+n+A\text{ is prime for }0\leq n\leq A-2}.
$$

## ↑ Ancestors (10)

1. [11I](../11i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
