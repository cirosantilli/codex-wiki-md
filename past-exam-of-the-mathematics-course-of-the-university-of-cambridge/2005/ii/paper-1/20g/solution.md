<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

The three quadratic subfields are $\mathbb Q(\sqrt2)$, $\mathbb Q(\sqrt p)$ and $\mathbb Q(\sqrt{2p})$. Their integer rings are respectively $\mathbb Z[\sqrt2]$, $\mathbb Z[\sqrt p]$ and $\mathbb Z[\sqrt{2p}]$, since their squarefree radicands are $2,3,2$ modulo four. Write $\theta=r+s\sqrt2+t\sqrt p+u\sqrt{2p}$. Relative traces to these three fields are $2r+2s\sqrt2$, $2r+2t\sqrt p$ and $2r+2u\sqrt{2p}$. Traces of [algebraic integers](../../../../../algebraic-integer.md) are [integral](../../../../../integral.md), so all four doubled coefficients are integers. Thus

$$
\theta=\tfrac12(a+b\sqrt p)+\tfrac12(c+d\sqrt p)\sqrt2,\qquad a,b,c,d\in\mathbb Z.
$$

The PDF names the wrong quadratic subfield for its next displayed norm coefficients. They are obtained from $k=\mathbb Q(\sqrt p)$, not $\mathbb Q(\sqrt2)$. The relevant conjugation changes the sign of $\sqrt2$, giving

$$
N_{K/\mathbb Q(\sqrt p)}(\theta)=\frac{a^2+pb^2-2c^2-2pd^2+2(ab-2cd)\sqrt p}{4}.
$$

Its membership in $\mathbb Z[\sqrt p]$ proves the requested divisibilities. For comparison, the norm to the printed subfield is $[a^2-pb^2+2c^2-2pd^2+2(ac-pbd)\sqrt2]/4$, a different expression.

The first divisibility modulo two makes $a,b$ have the same parity. The second makes $ab$ even, so they cannot both be odd: **$a$ and $b$ are even**. Substituting this into the first divisibility modulo four shows $c^2+pd^2$ is even, hence **$c\equiv d\pmod2$**. Therefore every [algebraic integer](../../../../../algebraic-integer.md) is an integer linear combination of

$$
\boxed{1,\quad\sqrt2,\quad\sqrt p,\quad w=\frac{(1+\sqrt p)\sqrt2}{2}.}
$$

Indeed the last two half-coefficients are $[(c-d)/2]\sqrt2+dw$. These four elements are rationally independent. They are all [integral](../../../../../integral.md): for $w$, $w^2=(p+1)/2+\sqrt p$, and consequently

$$
w^4-(p+1)w^2+\frac{(p-1)^2}{4}=0
$$

is a monic [polynomial](../../../../../polynomial-split.md) with integer coefficients. Their integer span consists of [algebraic integers](../../../../../algebraic-integer.md) and contains every [algebraic integer](../../../../../algebraic-integer.md) by the preceding argument, proving the [integral basis of a two-prime biquadratic field](../../../../../integral-basis-of-a-two-prime-biquadratic-field.md). This repairs the subfield typo without changing the claimed basis.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
