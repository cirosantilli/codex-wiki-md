<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Use the usual positive-definite convention for [binary quadratic forms](../../../../../binary-quadratic-form.md) with negative [discriminant](../../../../../discriminant.md). Reduction by integral changes of variables of [determinant](../../../../../determinant.md) one produces a form $ax^2+bxy+cy^2$ with $|b|\le a\le c$, and with $b\ge0$ on the boundary. For completeness, replacing $x$ by $x+ny$ makes $|b|\le a$; if then $c<a$, interchange the variables, reversing one sign to keep [determinant](../../../../../determinant.md) one. The new positive [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) is smaller. Repeating terminates and gives a reduced form.

For [discriminant](../../../../../discriminant.md) $-7$, $4ac-b^2=7$ and the reduction inequalities give $3a^2\le7$. Thus $a=1$, $b$ is odd and $|b|\le1$, and $c=2$. The boundary convention chooses $b=1$. Hence there is exactly one positive-definite [equivalence class](../../../../../equivalence-class.md), represented by $x^2+xy+2y^2$.

For an [odd prime](../../../../../odd-prime.md) $p\ne7$ represented by this form, the identity $4p=(2x+y)^2+7y^2$ shows that $-7$ is a square modulo $p$. Here $p\nmid y$, because otherwise $p\mid x$ and $p^2$ would divide the represented number. Conversely, if $-7$ is a square modulo $p$, choose odd $b$ with $b^2\equiv-7\pmod p$. Then $(p,b,(b^2+7)/(4p))$ is an integral positive-definite form of [discriminant](../../../../../discriminant.md) $-7$. By the preceding reduction it is equivalent to the given form, so its value $p$ at $(1,0)$ is represented by that form. [Quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives $(-7/p)=(p/7)$, whose value is one precisely for $p\equiv1,2,4\pmod7$. The exceptional [primes](../../../../../prime-number.md) are represented: $2=Q(0,1)$ and $7=Q(1,-2)$. Therefore

$$
\boxed{p\text{ is represented}\iff p=7\text{ or }p\equiv1,2,4\pmod7.}
$$

Without the positive-definite convention, the first printed assertion is false: $-x^2-xy-2y^2$ also has [discriminant](../../../../../discriminant.md) $-7$ but cannot be equivalent to a positive-definite form, because an invertible [change of variables](../../../../../change-of-variables-formula.md) preserves its sign.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
