<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $\gamma$ be the [real tautological line bundle](../../../../../real-tautological-line-bundle.md) over $\mathbb {RP}^2$. A homogeneous polynomial of degree $a$ defines a section of the real [line bundle](../../../../../line-bundle.md)

$$
L_a=(\gamma^*)^{\otimes a}.
$$

Indeed, on a projective line $\ell\subset\mathbb R^3$ its restriction satisfies $F(rv)=r^aF(v)$, exactly the transformation law for a linear functional on $\ell^{\otimes a}$. Its zero set is well defined without treating an odd-degree polynomial as a global real-valued function on projective space.

Put $u=w_1(\gamma)\in H^1(\mathbb {RP}^2;\mathbb F_2)$. This is the nonzero generator: the tautological line changes sign along the generating projective loop. Dualization preserves this sign, while tensoring multiplies transition signs, so

$$
w_1(L_a)=a u,\qquad w_1(L_b)=b u.
$$

For generic coefficients both polynomial sections are transverse to zero and their zero curves meet transversely. This genericity follows from parametric transversality: at each projective point some coordinate is nonzero, and varying the coefficient of its $a$th power varies the section's value freely; the two polynomial coefficient sets vary the two values independently. The common zero set is consequently a zero-dimensional submanifold of a compact space, and is finite.

We justify the needed [parity of zeros of a real line-bundle section](../../../../../parity-of-zeros-of-a-real-line-bundle-section.md). Along a closed loop transverse to the zero curve, trivialize the pulled-back [line bundle](../../../../../line-bundle.md) on the cut interval. At a simple zero the real component function changes sign. The product of these sign changes equals the sign of the bundle's transition around the loop, which is the evaluation of its first [Stiefel–Whitney class](../../../../../stiefel-whitney-class.md). Therefore the intersection parity of the zero curve with every loop equals the evaluation of $w_1$ on that loop. This says that its mod-two Poincare dual is $w_1$, so

$$
\operatorname{PD}_2[A]=a u,\qquad
\operatorname{PD}_2[B]=b u.
$$

The [mod-two Poincare duality](../../../../../mod-two-poincare-duality.md) intersection rule gives

$$
|A\cap B|\pmod2
=\left\langle\operatorname{PD}_2[A]\smile
\operatorname{PD}_2[B],[\mathbb {RP}^2]_2\right\rangle.
$$

There are no [orientation](../../../../../orientation-of-a-simplex.md) signs in these coefficients, so every transverse intersection contributes one. Two distinct projective lines meet in exactly one point; both have dual class $u$ by the preceding degree-one calculation. Hence $\langle u^2,[\mathbb {RP}^2]_2\rangle=1$, and

$$
\boxed{|A\cap B|\equiv ab\pmod2.}
$$

This proves the [parity of real projective plane-curve intersections](../../../../../parity-of-real-projective-plane-curve-intersections.md).

Equality with $ab$ need not hold. Choose $a=1$, $b=2$, with the line and conic

$$
A=\{z=0\},\qquad B=\{x^2+y^2-z^2=0\}.
$$

On the line, the conic equation becomes $x^2+y^2=0$, which has no nonzero real solution. Thus $\boxed{|A\cap B|=0\ne2=ab}$. Both real curves are smooth and nonempty, and they are disjoint, so their real intersection is transverse vacuously. Even over the complex numbers they meet in two distinct transverse points $[1,i,0]$ and $[1,-i,0]$; the example is not a tangency or shared-component exception. On the unit sphere $F^2+g^2$ has a positive minimum, so disjointness also persists under sufficiently small real coefficient perturbations, so it is compatible with the generic real situation.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
