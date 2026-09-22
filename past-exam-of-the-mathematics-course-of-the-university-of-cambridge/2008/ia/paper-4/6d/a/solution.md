<h1 id="6d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $d=\gcd(a,m)$. If the [linear congruence](../../../../../../linear-congruence.md) $ar\equiv b\pmod m$ holds, then $b=ar-ms$ for some [integer](../../../../../../integer.md) $s$, so the [greatest common divisor](../../../../../../greatest-common-divisor.md) $d$ divides $b$. Conversely, [Bézout's identity](../../../../../../bezout-identity.md) gives [integers](../../../../../../integer.md) $u,v$ with $au+mv=d$. If $b=dj$, multiply this identity by $j$ to obtain $a(uj)\equiv b\pmod m$. Hence

$$
\boxed{ar\equiv b\pmod m\text{ has a solution}\iff d\mid b.}
$$

For the number of solutions, write $a=da'$, $m=dm'$ and $b=db'$. The [linear congruence](../../../../../../linear-congruence.md) becomes $a'r\equiv b'\pmod {m'}$, where $a',m'$ are [coprime integers](../../../../../../coprime-integers.md). Multiplication by $a'$ is invertible modulo $m'$ by [Bézout's identity](../../../../../../bezout-identity.md), so the solutions form one [residue class](../../../../../../residue-class.md) $r\equiv r_0\pmod {m'}$. Modulo $m=dm'$, these are exactly

$$
\boxed{r_0,\ r_0+m',\ldots,r_0+(d-1)m'.}
$$

They are distinct: if two have the same [residue class](../../../../../../residue-class.md) modulo $m$, then $dm'$ divides $(j-\ell)m'$, forcing $d\mid j-\ell$; with $0\leq j,\ell<d$, this forces $j=\ell$. Every other solution differs from $r_0$ by a multiple of $m'$, so these exhaust the $d$ solutions.

Finally,

$$
b(m/d)\equiv0\pmod m\iff dm'\mid bm'\iff d\mid b.
$$

Combining this with the existence criterion gives the requested equivalent [modular congruence](../../../../../../modular-congruence.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
