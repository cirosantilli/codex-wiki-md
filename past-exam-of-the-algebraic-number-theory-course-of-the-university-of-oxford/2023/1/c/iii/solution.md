<h1 id="1/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\alpha=\sqrt{m_1}$, $\beta=\sqrt{m_2}$, and

$$
\omega=\frac{1+\beta}{2}.
$$

The proposed [integral basis for coprime biquadratic radicands congruent to two and one](../../../../../integral-basis-for-coprime-biquadratic-radicands-congruent-to-two-and-one.md) is

$$
\boxed{\{1,\alpha,\omega,\alpha\omega\}}.
$$

Each entry is an [algebraic integer](../../../../../algebraic-integer.md), by the [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) formula and closure under products. Their coefficient [matrix](../../../../../matrix.md) in $1,\alpha,\beta,\alpha\beta$ has [determinant](../../../../../determinant.md) $1/4$, so they are rationally [linearly independent](../../../../../linear-independence.md). It remains to show that they span every [algebraic integer](../../../../../algebraic-integer.md).

Write $\gamma=(a+b\alpha+c\beta+d\alpha\beta)/2$ initially with rational $a,b,c,d$. The [field traces](../../../../../field-trace.md) to $\mathbb Q(\alpha)$ and $\mathbb Q(\alpha\beta)$ are $a+b\alpha$ and $a+d\alpha\beta$. Since $m_1\equiv m_1m_2\equiv2\pmod4$, the corresponding [integral basis](../../../../../integral-basis.md) in each subfield gives $a,b,d\in\mathbb Z$. The [field trace](../../../../../field-trace.md) to $\mathbb Q(\beta)$ is $a+c\beta$. Membership in $\mathbb Z[\omega]$ says that $2a,2c$ are [integers](../../../../../integer-split.md) of equal parity. As $a$ is already an [integer](../../../../../integer-split.md), this forces $c\in\mathbb Z$ too.

Now the [field norm](../../../../../field-norm.md) to $\mathbb Q(\beta)$ is

$$
\frac A4+\frac{ac-m_1bd}{2}\beta,
\qquad A=a^2+m_2c^2-m_1b^2-m_1m_2d^2.
$$

By the [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) formula, $A/2$ is an [integer](../../../../../integer-split.md) and has the same parity as $ac-m_1bd$. Thus $A$ is even, giving $a\equiv c\pmod2$, and

$$
A\equiv2ac-2m_1bd\equiv2ac\pmod4.
$$

Using $m_1\equiv2$, $m_2\equiv1$ and $a\equiv c\pmod2$, this becomes

$$
0\equiv A-2ac\equiv(a-c)^2-2(b^2+d^2)
\equiv-2(b^2+d^2)\pmod4.
$$

Hence $b\equiv d\pmod2$. Finally,

$$
\gamma=\frac{a-c}{2}+\frac{b-d}{2}\alpha+c\omega+d\alpha\omega,
$$

an expression with [integer](../../../../../integer-split.md) coefficients. This proves the asserted [integral basis](../../../../../integral-basis.md) without assuming a general theorem about products of elements of an [integral basis](../../../../../integral-basis.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
