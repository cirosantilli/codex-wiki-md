<h1 id="3/iii/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $a=x^{p^{n-1}}$ and $b=y^{p^{n-1}}$, both in $U_{n-1}$. The collection formula gives

$$
(ab)^p\equiv a^pb^p\pmod{U_{2n}}.
$$

Indeed the weight-two [group commutator](../../../../../../../group-commutator.md) lies in $[U_{n-1},U_{n-1}]\le U_{2n-1}$, and its coefficient $\binom p2$ is divisible by $p$ since $p$ is odd, moving it into $U_{2n}$. A [group commutator](../../../../../../../group-commutator.md) of weight $j\ge3$ in $a,b$ lies in $U_{jn-1}\le U_{2n}$; all higher terms are therefore harmless as well. This also covers $n=1$.

Let $v=x+_{n-1}y$ and $u=x+_ny$. Their powers satisfy $v^{p^n}=(ab)^p$ and $u^{p^n}=a^pb^p$. Taking $p^n$th roots of the collected congruence gives $u\equiv v\pmod{U_n}$. Since $U_n=P_{n+1}\le P_n$, this proves the requested, slightly weaker, result

$$
\boxed{x+_ny\equiv x+_{n-1}y\pmod{P_n(G)}.}
$$

For $n=1$ the definition $+_0=$ ordinary multiplication makes the comparison meaningful.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
