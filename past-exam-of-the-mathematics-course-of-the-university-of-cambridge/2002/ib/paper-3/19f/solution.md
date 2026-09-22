<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

Use the standard reduced-form convention $|b|\le a\le c$, with $b\ge0$ when $|b|=a$ or $a=c$. To reduce a positive definite integral [binary quadratic form](../../../../../binary-quadratic-form.md), choose a primitive integer vector at which the positive integer value is least. Complete that vector to a unimodular [basis](../../../../../basis.md); it makes the leading coefficient $a$ that least value. A shear of the second [basis](../../../../../basis.md) vector by an integer multiple of the first replaces $b$ by $b+2ka$, allowing $|b|\le a$. The new $c$ is the value at another primitive vector, hence $c\ge a$. If $b=-a$, a shear makes $b=a$ without changing $a,c$; if $a=c$ and $b<0$, the [determinant](../../../../../determinant.md)-one swap $(x,y)\mapsto(-y,x)$ reverses its sign. Thus every form is properly equivalent to a [reduced positive definite binary quadratic form](../../../../../reduced-positive-definite-binary-quadratic-form.md). This argument also gives the [reduction algorithm for a positive definite binary quadratic form](../../../../../reduction-algorithm-for-a-positive-definite-binary-quadratic-form.md) by successively decreasing its positive leading coefficient.

For a negative integral discriminant $d\equiv0$ or $1\pmod4$, a [prime](../../../../../prime-number.md) $p$ is represented by some integral form of discriminant $d$ exactly when

$$
\boxed{b^2\equiv d\pmod{4p}\text{ is soluble}}.
$$

Indeed a representing vector is primitive, since a common divisor of its coordinates would have its square divide $p$. A unimodular change takes it to the first [basis](../../../../../basis.md) vector, giving a form $[p,b,c]$ and $d=b^2-4pc$. Conversely a solution $b$ gives the positive definite form $[p,b,(b^2-d)/(4p)]$, which represents $p$ at $(1,0)$. For odd $p$ this is the [discriminant criterion for prime representation by a binary quadratic form](../../../../../discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form.md): $d$ must be a square modulo $p$, with parity chosen to satisfy the modulo-four condition.

For $d=-32$ and odd $p$, the [Legendre symbol](../../../../../legendre-symbol.md) is $(-32/p)=(-2/p)=(-1/p)(2/p)$. The supplementary laws make it positive exactly for $p\equiv1,3\pmod8$. The [prime](../../../../../prime-number.md) $2$ also works directly, since $[2,0,4]$ has discriminant $-32$ and represents $2$. Therefore

$$
\boxed{p\text{ is represented by some form of discriminant }-32
\iff p\equiv1,2,3\pmod8}.
$$

The class $2\pmod8$ here consists only of the [prime](../../../../../prime-number.md) $2$.

For a reduced form, $32=4ac-b^2\ge3a^2$, so $a\le3$. The integer checks yield the [reduced forms of discriminant minus thirty-two](../../../../../reduced-forms-of-discriminant-minus-thirty-two.md):

$$
\boxed{[1,0,8],\qquad[2,0,4],\qquad[3,2,3]}.
$$

If one omits the boundary sign convention, $[3,-2,3]$ also appears, but is properly equivalent to $[3,2,3]$. The middle form is imprimitive and represents no odd integer. An odd integer represented by $x^2+8y^2$ has $x$ odd and is $1\pmod8$. For $3x^2+2xy+3y^2$ to be odd, one of $x,y$ must be odd and the other even; substitution modulo eight gives $3\pmod8$ in either case. If both are odd or both even, the value is even. Thus a [prime](../../../../../prime-number.md) represented by the last form is necessarily $3\pmod8$.

Conversely, a [prime](../../../../../prime-number.md) $p\equiv3\pmod8$ is represented by some discriminant-$-32$ form, which reduces to one of the three displayed forms without changing its represented integers. The first and second cannot represent it, so the third must. Consequently

$$
\boxed{p=3x^2+2xy+3y^2\text{ for integers }x,y\iff p\equiv3\pmod8}.
$$

The [prime](../../../../../prime-number.md) $2$ is not an exception for this particular form: its minimum positive value is $3$, as also follows from $3x^2+2xy+3y^2=2(x^2+y^2)+(x+y)^2$.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
