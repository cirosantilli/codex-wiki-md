<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

Use the [reduction algorithm for a positive definite binary quadratic form](../../../../../reduction-algorithm-for-a-positive-definite-binary-quadratic-form.md). A determinant-one shear $(x,y)\mapsto(x+ky,y)$ puts the middle coefficient in $[-a,a]$. If the resulting last coefficient is smaller than $a$, the determinant-one substitution $(x,y)\mapsto(-y,x)$ decreases the positive integer leading coefficient. Repeating terminates with a [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md) satisfying $|b|\leq a\leq c$. These substitutions preserve [proper equivalence of binary quadratic forms](../../../../../proper-equivalence-of-binary-quadratic-forms.md) and the [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md).

The [enumeration of reduced binary quadratic forms](../../../../../enumeration-of-reduced-binary-quadratic-forms.md) gives

$$
163=4ac-b^2\geq3a^2,\qquad1\leq a\leq7.
$$

Since $b^2\equiv-163\equiv1\pmod4$, $b$ is odd. For $|b|=1,3,5,7$, the possible values of $(b^2+163)/4$ are respectively $41,43,47,53$. Each is a [prime number](../../../../../prime-number.md) greater than seven. But $ac=(b^2+163)/4$, so its positive divisor $a\leq7$ must be one. Then $|b|\leq a$ forces $b=\pm1$ and $c=41$. The two signs are properly equivalent: substituting $x\mapsto x-y$ in $x^2+xy+41y^2$ gives $x^2-xy+41y^2$. Thus every form in question is properly equivalent to

$$
\boxed{x^2+xy+41y^2.}
$$

## ↑ Ancestors (11)

1. [1I](../1i.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
