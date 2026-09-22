<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose first that $x^p+y^p=z^p$ with $x,y,z\in\mathbb Z_p^\times$. Divide by $y^p$ and put $u=x/y$, $w=z/y$. Reduction modulo $p$ gives $w\equiv u+1\pmod p$. Choose an integer $a\equiv u\pmod p$; then $p\nmid a(a+1)$. A unit's $p$th power modulo $p^2$ depends only on its residue modulo $p$, because $(a+pt)^p\equiv a^p\pmod{p^2}$. Therefore

$$
(a+1)^p\equiv w^p=u^p+1\equiv a^p+1\pmod{p^2}.
$$

Conversely, suppose such an integer $a$ exists. The congruence says

$$
\frac{a^p+1}{(a+1)^p}\in1+p^2\mathbb Z_p.
$$

For odd $p$, the $p$th-power map sends $1+p\mathbb Z_p$ onto $1+p^2\mathbb Z_p$: under the [p-adic logarithm](../../../../../../p-adic-logarithm.md) it becomes multiplication by $p$. Hence the displayed ratio is $t^p$ for some $t\in1+p\mathbb Z_p$. Taking

$$
x=a,
\qquad y=1,
\qquad z=(a+1)t
$$

produces the required solution in $\mathbb Z_p^\times$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
