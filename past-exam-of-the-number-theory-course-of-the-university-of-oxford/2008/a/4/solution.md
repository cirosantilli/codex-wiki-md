<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [straightedge and compass construction](../../../../straightedge-and-compass-construction-split.md) uses finitely many steps drawing lines through known points and circles with known centres and constructible radii, and adjoining their intersection points. The coordinates obtained by line–line intersections require only [field](../../../../field.md) operations; line–circle and circle–circle intersections require at most a [quadratic extension](../../../../quadratic-extension.md) after eliminating a linear equation. Thus all coordinates lie in a tower of [quadratic extensions](../../../../quadratic-extension.md) of the initial coordinate [field](../../../../field.md). The degree of any finite intermediate coordinate [field](../../../../field.md) containing that initial [field](../../../../field.md) divides a [power of two](../../../../power-of-two.md) and is therefore $\boxed{2^r}$ for some $r\ge0$.

For the source's notation this assumes $K\supseteq K_0$, as is customary when previously constructed points are retained. If only the coordinates of a final subset are called $K$, replace it by the compositum $K_0K$; otherwise the expression $[K:K_0]$ need not be defined. The power-of-two condition is necessary and is not being asserted as sufficient for an arbitrary algebraic number.

Starting from a unit cube, [doubling its volume](../../../../impossibility-of-doubling-the-cube-by-straightedge-and-compass.md) would construct a length $\sqrt[3]2$. Its [polynomial](../../../../polynomial-split.md) $X^3-2$ is Eisenstein at two, so its degree over $\mathbb Q$ is three, which cannot divide a [power of two](../../../../power-of-two.md). Thus **doubling the cube is impossible by ruler and compass**.

Set $c=\cos\theta$, $s=\sin\theta$. The real part of $(c+is)^5$ is $c^5-10c^3s^2+5cs^4$. Replacing $s^2$ by $1-c^2$ gives

$$
\boxed{\cos5\theta=16c^5-20c^3+5c.}
$$

Choose the given angle to have cosine $5/6$. It is constructible, since its [unit circle](../../../../complex-unit-circle.md) point has coordinates $(5/6,\sqrt{11}/6)$. If a fifth of that angle were constructible and had cosine $c$, the identity would imply

$$
96c^5-120c^3+30c-5=0.
$$

This [polynomial](../../../../polynomial-split.md) is Eisenstein at five: all nonleading coefficients are divisible by five and the constant term is not divisible by 25, while 96 is not divisible by five. Hence $[\mathbb Q(c):\mathbb Q]=5$. But the initial angle [field](../../../../field.md) is $\mathbb Q(\sqrt{11})$, itself of degree two, so adjoining any finite collection of constructible coordinates to it would still give total degree over $\mathbb Q$ a [power of two](../../../../power-of-two.md). It could not contain a degree-five element. Thus **[general angle quintisection is impossible with straightedge and compass](../../../../general-angle-quintisection-is-impossible-with-straightedge-and-compass.md)**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
