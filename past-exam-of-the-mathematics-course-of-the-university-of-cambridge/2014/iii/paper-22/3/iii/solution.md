<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [congruent number elliptic curve](../../../../../../congruent-number-elliptic-curve.md) in the equivalent coordinates

$$
E_{15}:y^2=x^3-225x.
$$

The [rational point](../../../../../../rational-point.md) $P=(25,100)$ lies on it, since $25^3-225\cdot25=10000$. By the preceding [rational torsion of a congruent number curve](../../../../../../rational-torsion-of-a-congruent-number-curve.md) result, every rational [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) has $y=0$ or is $O$. Thus $P$ is not a [torsion point of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md), and its positive multiples give infinitely many distinct [rational points](../../../../../../rational-point.md) with nonzero $y$.

For any such point $(x,y)$, put

$$
\boxed{a=\left|\frac{x^2-225}{y}\right|,\quad
b=\left|\frac{30x}{y}\right|,\quad
c=\left|\frac{x^2+225}{y}\right|.}
$$

The identity $(x^2-225)^2+(30x)^2=(x^2+225)^2$ proves that these positive rational numbers are the sides of a [right triangle](../../../../../../right-triangle.md). Their area is

$$
\frac{ab}{2}=15\left|\frac{x(x^2-225)}{y^2}\right|=15.
$$

All three sides are nonzero because a point with $y\ne0$ has $x\notin\{0,15,-15\}$. For $P$ the construction gives $(a,b,c)=(4,15/2,17/2)$.

It remains to ensure that infinitely many points do not describe only finitely many triangles. Given the ordered positive pair $b,c$, set $r=c/b$. Then $X=|x|$ satisfies

$$
X^2-30rX+225=0.
$$

There are at most two possible $X$, then at most two signs of $x$ and two signs of $y$. Thus each ordered triangle has at most eight preimages; allowing interchange of its legs still gives a finite number. **There are infinitely many distinct rational right triangles of area $15$.** This is the [infinitely many rational right triangles from a nontorsion point](../../../../../../infinitely-many-rational-right-triangles-from-a-nontorsion-point.md) principle.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
