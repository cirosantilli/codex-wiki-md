<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With zero seed, both [Bäcklund transformation](../../../../../../backlund-transformation.md) equations concern $\phi_a/2$. On a nonconstant branch, separation of variables uses $d\log|\tan(\phi_a/4)|=d\phi_a/[2\sin(\phi_a/2)]$, giving

$$
\tan\frac{\phi_a}{4}=C\exp(a x_++a^{-1}x_-),\qquad a\ne0.
$$

For $C>0$, absorb its magnitude into an additive constant $c=\log C$ in the exponent. A convenient smooth representative is

$$
\boxed{\phi_a(x,t)=4\arctan\exp\left[\frac{a+a^{-1}}2x+\frac{a-a^{-1}}2t+c\right].}
$$

The constant-phase condition for this traveling profile determines its [velocity](../../../../../../velocity.md):

$$
\boxed{v_a=\frac{1-a^2}{1+a^2},\qquad\gamma_a=\frac{|a+a^{-1}|}{2}=\frac1{\sqrt{1-v_a^2}}.}
$$

**The profile is a traveling [soliton](../../../../../../soliton.md) with [velocity](../../../../../../velocity.md) $v_a=(1-a^2)/(1+a^2)$, strictly between $-1$ and $1$.** The [scalar-field vacua](../../../../../../scalar-field-vacuum.md) on the two sides differ by $2\pi$. With the [topological charge](../../../../../../topological-charge.md) convention $Q=[\phi(+\infty)-\phi(-\infty)]/(2\pi)$, this branch has $Q=\operatorname{sgn}a$: it is a [Sine-Gordon kink](../../../../../../sine-gordon-kink.md) for $a>0$ and an [antikink](../../../../../../antikink.md) for $a<0$. Its width is proportional to $\gamma_a^{-1}$, and its derivative decays exponentially away from its center, giving a [finite-energy field configuration](../../../../../../finite-energy-field-configuration.md).

For completeness, the classical rest [mass](../../../../../../mass.md) in this paper's coupling convention is $8m/\beta$, as derived in Question 2; a [Lorentz boost](../../../../../../lorentz-boost.md) gives energy $8m\gamma_a/\beta$. This localized, topologically protected traveling field is the required [classical field-theory soliton](../../../../../../classical-field-theory-soliton-split.md). A negative $C$ reverses the field and hence the [topological charge](../../../../../../topological-charge.md); $C=0$ gives the vacuum rather than a [soliton](../../../../../../soliton.md). Vacuum shifts by $4\pi$ can be made without changing the displayed [Bäcklund transformation](../../../../../../backlund-transformation.md) equations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
