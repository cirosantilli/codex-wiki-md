<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Again put $\alpha=\sqrt{m_1}$ and $\beta=\sqrt{m_2}$. The [ring of integers](../../../../../ring-of-integers.md) of each of the three quadratic subfields has [integral basis](../../../../../integral-basis.md) $1,\alpha$, $1,\beta$, or $1,\alpha\beta$, respectively: their square-free radicands are respectively congruent to $3,2,2$ modulo four. The [field traces](../../../../../field-trace.md) of the [algebraic integer](../../../../../algebraic-integer.md) $\gamma$ to those subfields are

$$
a+b\alpha,\qquad a+c\beta,\qquad a+d\alpha\beta,
\qquad a=2r,\ b=2s,\ c=2t,\ d=2u.
$$

They are [algebraic integers](../../../../../algebraic-integer.md), so comparison with each [integral basis](../../../../../integral-basis.md) gives

$$
\boxed{a,b,c,d\in\mathbb Z}.
$$

This use of all three subfields is needed to control $d$ as well as the other coefficients.

The [field norm](../../../../../field-norm.md) to $\mathbb Q(\alpha)$ is

$$
N_{L/\mathbb Q(\alpha)}(\gamma)
=\frac{a^2+m_1b^2-m_2c^2-m_1m_2d^2}{4}
+\frac{ab-m_2cd}{2}\alpha.
$$

Its two coefficients must be [integers](../../../../../integer-split.md). The second condition says $ab$ is even, since $m_2$ is even. Reducing the numerator of the first coefficient modulo four gives

$$
a^2-b^2-2(c^2+d^2)\equiv0\pmod4.
$$

Reduction modulo two first gives $a\equiv b\pmod2$. Since $ab$ is even, both $a$ and $b$ are even. The same congruence now gives $c^2+d^2\equiv0\pmod2$, or $c\equiv d\pmod2$. Therefore every [algebraic integer](../../../../../algebraic-integer.md) has the form

$$
\gamma=\frac a2+\frac b2\alpha+\frac{c-d}{2}\beta+d w,
\qquad w=\frac{\beta+\alpha\beta}{2},
$$

with four [integer](../../../../../integer-split.md) coefficients.

For the converse, $1,\alpha,\beta$ are [algebraic integers](../../../../../algebraic-integer.md), and

$$
w^2=\frac{m_2(1+m_1)}4+\frac{m_2}2\alpha\in\mathbb Z[\alpha].
$$

Here $4\mid1+m_1$ and $2\mid m_2$, so both coefficients are [integers](../../../../../integer-split.md). The [monic polynomial](../../../../../monic-polynomial.md) $X^2-w^2$ and [integral dependence is transitive](../../../../../integral-dependence-is-transitive.md) show that $w$ is an [algebraic integer](../../../../../algebraic-integer.md). The four displayed generators are rationally [linearly independent](../../../../../linear-independence.md), since their coefficient [matrix](../../../../../matrix.md) in $1,\alpha,\beta,\alpha\beta$ has [determinant](../../../../../determinant.md) $1/2$. Hence the [integral basis for coprime biquadratic radicands congruent to three and two](../../../../../integral-basis-for-coprime-biquadratic-radicands-congruent-to-three-and-two.md) is

$$
\boxed{\left\{1,\sqrt{m_1},\sqrt{m_2},\frac{\sqrt{m_2}+\sqrt{m_1m_2}}2\right\}}.
$$

In this formula $\sqrt{m_1m_2}$ denotes the product $\alpha\beta$ of the chosen square roots; this convention also handles negative radicands.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the algebraic number theory course of the University of Oxford](../../../../split.md)
6. [Algebraic number theory course of the University of Oxford](../../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
