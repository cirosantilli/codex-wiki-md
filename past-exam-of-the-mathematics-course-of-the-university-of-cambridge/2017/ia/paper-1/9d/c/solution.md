<h1 id="9d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $h(x)=f(x)-yx$. Then

$$
h'(a)=f'(a)-y\leq0,
\qquad h'(b)=f'(b)-y\geq0.
$$

The [extreme value theorem](../../../../../../extreme-value-theorem.md) gives a minimum of $h$ on $[a,b]$. If it occurs in $(a,b)$, the two-sided difference quotient gives $h'(c)=0$. If it occurs at $a$, either $h'(a)=0$ or a negative right derivative contradicts minimality; the endpoint $b$ is analogous. Hence some $c\in[a,b]$ satisfies

$$
\boxed{f'(c)=y}.
$$

This proves the [Darboux theorem for derivatives](../../../../../../darboux-s-theorem-analysis.md) in the stated case without assuming that $f'$ is continuous.

Because a differentiable function is continuous, define

$$
F(x)=f(x)+\int_a^x f(t)\,dt.
$$

The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives $F'(x)=f'(x)+f(x)$. At the endpoints,

$$
F'(a)=f'(a)+f(a)\leq f'(a)\leq y,
$$

while

$$
F'(b)=f'(b)+f(b)\geq f'(b)\geq y.
$$

Applying the result just proved to $F$ yields $d\in[a,b]$ with

$$
\boxed{f'(d)+f(d)=y}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
