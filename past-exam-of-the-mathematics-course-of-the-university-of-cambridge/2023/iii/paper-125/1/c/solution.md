<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $\phi$ is a [separable isogeny](../../../../../../separable-isogeny.md),

$$
\phi^*(O_{E_2})=\sum_{T\in E_1[\phi]}(T).
$$

The degree-zero divisor

$$
D=\phi^*(O_{E_2})-d(O_{E_1})
$$

corresponds under $E_1\simeq\operatorname{Pic}^0(E_1)$ to the sum of all elements of the finite abelian group $E_1[\phi]$. Pairing every $T$ with $-T$ shows that this sum is the sum of the elements in $E_1[\phi]\cap E_1[2]$. It vanishes when that intersection has one element and also when it has four elements, since the sum of the four elements of $(\mathbb Z/2\mathbb Z)^2$ is zero. The [principal divisor criterion on an elliptic curve](../../../../../../principal-divisor-criterion-on-an-elliptic-curve.md) therefore gives a rational function $g$ with $\operatorname{div}(g)=D$.

The divisor $D$ is invariant under $[-1]$, so $[-1]^*g/g$ has zero divisor and is constant. Applying $[-1]$ twice shows that this constant has square one; hence $[-1]^*g=\pm g$.

For a short [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md)

$$
E:y^2=x^3+Ax+B,
$$

the multiplication-by-two isogeny has

$$
\operatorname{div}(y)=\sum_{T\in E[2]}(T)-4(O_E)=[2]^*(O_E)-4(O_E).
$$

Thus one may take $g=y$, and $[-1]^*y=-y$. For multiplication by three, the third [division polynomial of an elliptic curve](../../../../../../division-polynomials.md)

$$
\psi_3(x)=3x^4+6Ax^2+12Bx-A^2
$$

vanishes simply at the eight nonzero points of $E[3]$ and has a pole of order eight at $O_E$. Hence $g=\psi_3(x)$ has divisor $[3]^*(O_E)-9(O_E)$ and satisfies $[-1]^*g=g$. Both signs occur.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
