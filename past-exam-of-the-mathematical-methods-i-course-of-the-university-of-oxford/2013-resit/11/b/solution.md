<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $w=(z+1)/(z-1)$, with $z\ne1$. For a nonzero integer $n$, all solutions of $w^n=i$ are

$$
w_k=\exp\left(\frac{i(\pi/2+2\pi k)}n\right),\qquad k=0,\ldots,|n|-1.
$$

This covers negative integers too: $w$ is then nonzero and $w^{|n|}=-i$. No $w_k$ equals one. Inverting the [Möbius transformation](../../../../mobius-transformation.md) and using half-angle identities gives the [cotangent roots of a powered Möbius transformation](../../../../cotangent-roots-of-a-powered-mobius-transformation.md):

$$
\boxed{z_k=\frac{w_k+1}{w_k-1}
=-i\cot\left(\frac{\pi/4+\pi k}{n}\right),\quad k=0,\ldots,|n|-1.}
$$

These $|n|$ solutions are distinct and purely imaginary. For $n=0$ there is no solution: every defined zeroth power is one, not $i$. For negative $n$, $z=-1$ must additionally be excluded from the equation's domain; none of the displayed roots equals it.

For the cubic, direct expansion shows

$$
(1-i)(z^3+3iz^2+3z+i)=(z+1)^3-i(z-1)^3.
$$

Since $z=1$ is not a root, the cubic is precisely the $n=3$ case. Taking $k=0,1,2$ yields

$$
\boxed{z=-i(2+\sqrt3),\qquad -i(2-\sqrt3),\qquad i.}
$$

For an algebraic check, the cubic factors as $(z-i)(z^2+4iz-1)$, which gives the same three distinct roots.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
