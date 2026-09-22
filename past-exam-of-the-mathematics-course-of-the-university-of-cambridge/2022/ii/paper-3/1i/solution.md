<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

The [Lagrange theorem for polynomial congruences](../../../../../lagrange-theorem-for-polynomial-congruences.md) says that if $p$ is prime and $f\in\mathbb Z[X]$ has degree $d$ with at least one coefficient not divisible by $p$, then

$$
f(x)\equiv0\pmod p
$$

has at most $d$ incongruent solutions modulo $p$.

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) states that for pairwise coprime $m_1,\ldots,m_r$, every system

$$
x\equiv a_i\pmod{m_i}
\qquad(1\leq i\leq r)
$$

has exactly one solution modulo $M=\prod_i m_i$. For two moduli, choose $u,v$ with $um+vn=1$ by [Bezout identity](../../../../../bezout-identity.md). Then

$$
x=a\,vn+b\,um
$$

is congruent to $a$ modulo $m$ and to $b$ modulo $n$. If $x,y$ are two solutions, both $m$ and $n$ divide $x-y$; coprimality makes $mn$ divide $x-y$. This proves existence and uniqueness for two factors, and induction proves the general statement.

Now

$$
1729=7\cdot13\cdot19
$$

and $12^3+1=1729$, so $x=12$ is a solution. For $1\leq x<12$, one has $0<x^3+1<1729$, so no such positive integer can satisfy the congruence. Hence the smallest is

$$
\boxed{x=12}.
$$

Modulo $7,13,19$, the roots are respectively

$$
\{3,5,6\},\qquad
\{4,10,12\},\qquad
\{8,12,18\}.
$$

Each list has three elements, and the Chinese remainder theorem combines the choices independently. Therefore the number of solutions with $1\leq x\leq1729$ is

$$
\boxed{3^3=27}.
$$

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
