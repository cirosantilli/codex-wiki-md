<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $x=r+s\sqrt d$ with $r,s\in\mathbb Q$. The [field trace](../../../../field-trace.md) and [field norm](../../../../field-norm.md) are

$$
T=2r,\qquad N=r^2-ds^2.
$$

The element is an [algebraic integer](../../../../algebraic-integer.md) if and only if $T,N\in\mathbb Z$: necessity follows from its two conjugates; sufficiency follows from the [monic polynomial](../../../../monic-polynomial.md) $X^2-TX+N$.

Suppose $x$ is an [algebraic integer](../../../../algebraic-integer.md). Set $a=2r\in\mathbb Z$. Then

$$
d(2s)^2=T^2-4N\in\mathbb Z.
$$

Write $2s=h/k$ in lowest terms, with $k>0$. Then $k^2\mid d$, and the hypothesis that $d$ is a [square-free integer](../../../../square-free-integer.md) forces $k=1$. Thus $b=2s\in\mathbb Z$, and the remaining condition is

$$
a^2-db^2\equiv0\pmod4.
$$

The only squares modulo four are zero and one. For $d\equiv2\pmod4$, an odd $b$ is impossible, after which $a$ is even. For $d\equiv3\pmod4$, an odd $b$ would require $a^2\equiv3\pmod4$, again impossible. For $d\equiv1\pmod4$, the condition is precisely $a\equiv b\pmod2$.

Conversely, $\sqrt d$ satisfies $X^2-d$, and when $d\equiv1\pmod4$, the element $\omega=(1+\sqrt d)/2$ satisfies

$$
X^2-X+\frac{1-d}{4}\in\mathbb Z[X].
$$

Their integer spans therefore consist of [algebraic integers](../../../../algebraic-integer.md). In the last case,

$$
\frac{a+b\sqrt d}{2}=\frac{a-b}{2}+b\omega.
$$

This proves the [ring of integers of a quadratic field](../../../../ring-of-integers-of-a-quadratic-field.md) formula. The required [integral basis](../../../../integral-basis.md) is

$$
\boxed{\begin{cases}
\{1,\sqrt d\},&d\equiv2,3\pmod4,\\
\{1,(1+\sqrt d)/2\},&d\equiv1\pmod4.
\end{cases}}
$$

Their rational [linear independence](../../../../linear-independence.md) follows from $\sqrt d\notin\mathbb Q$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
