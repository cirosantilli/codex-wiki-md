<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the right [coaction](../../../../../../coaction.md) of the [coordinate Hopf algebra of quantum SL2](../../../../../../coordinate-hopf-algebra-of-quantum-sl2.md) on the [quantum plane](../../../../../../quantum-plane.md) to be

$$
\delta(x)=x\otimes a+y\otimes c,\qquad
\delta(y)=x\otimes b+y\otimes d.
$$

It is extended multiplicatively and sends $1$ to $1\otimes1$. The matrix [comultiplication](../../../../../../comultiplication.md) and [counit](../../../../../../counit.md) verify the [coaction](../../../../../../coaction.md) identities on $x,y$. To check that it descends to the [quantum plane](../../../../../../quantum-plane.md), expand

$$
\delta(y)\delta(x)-q\delta(x)\delta(y)
=x^2\otimes(ba-qab)+y^2\otimes(dc-qcd)
+xy\otimes[bc+q da-q ad-q^2cb]=0.
$$

The last bracket vanishes because $bc=cb$ and $da-ad=(q-q^{-1})bc$.

For the requested calculation, $ca=qac$ and $yx=qxy$ give

$$
\delta(x)^2=x^2\otimes a^2+(1+q^2)xy\otimes ac+y^2\otimes c^2.
$$

Multiply by $\delta(y)$, put all [monomials](../../../../../../monomial.md) into the order $x^ry^s$, and use $bc=cb$. The answer is

$$
\boxed{\begin{aligned}
\delta(x^2y)={}&x^3\otimes a^2b
+x^2y\otimes\bigl(a^2d+(1+q^2)abc\bigr)\\
&+xy^2\otimes\bigl((1+q^2)acd+q^2bc^2\bigr)
+y^3\otimes c^2d.
\end{aligned}}
$$

A left-[coaction](../../../../../../coaction.md) convention transposes where the matrix coefficients occur; the displayed answer fixes the right [coaction](../../../../../../coaction.md) throughout.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
