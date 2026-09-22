<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a nonconstant [meromorphic](../../../../../meromorphic-function.md) map, write $T_f(R)=m(R,f)+N(R;\infty)$ in the usual normalization, where $m=(2\pi)^{-1}\int\log^+|f(Re^{i\theta})|\,d\theta$. Let $N(R;a)$ count $a$-points with their local degrees, and let $\overline N(R;a)$ count each distinct point once, using the same integrated logarithmic weights. At infinity the local degree is the [pole](../../../../../pole.md) order. The [Nevanlinna deficiency](../../../../../nevanlinna-deficiency.md) and [Nevanlinna ramification index](../../../../../nevanlinna-ramification-index.md) are

$$
\boxed{\delta_f(a)=1-\limsup_{R\to\infty}\frac{N(R;a)}{T_f(R)},\qquad
\theta_f(a)=\liminf_{R\to\infty}\frac{N(R;a)-\overline N(R;a)}{T_f(R)}.}
$$

The latter is an asymptotic excess-multiplicity index, not the integer local ramification degree. The [Nevanlinna first main theorem](../../../../../nevanlinna-first-main-theorem.md) gives $N(R;a)\le T_f(R)+O(1)$ and identifies deficiency with the lower limiting normalized proximity. The target $a$ ranges over the [Riemann sphere](../../../../../riemann-sphere.md), not just the real line.

The exponential is entire and has no [poles](../../../../../pole.md). Consequently

$$
T_e(R)=\frac1{2\pi}\int_0^{2\pi}\max(0,R\cos\theta)\,d\theta
=\boxed{\frac R\pi}.
$$

Thus $c=1/\pi$ in this normalization.

To obtain the rational-composition growth, represent the nonconstant degree-$d$ sphere map by relatively prime homogeneous [polynomials](../../../../../polynomial-split.md) $(P,Q)$ of degree $d$. Their joint norm on the unit sphere in $\mathbb C^2$ has a positive minimum and finite maximum: simultaneous vanishing would contradict relative primeness on the projective line. Homogeneity therefore gives constants $0<A\le B<\infty$ with

$$
A\|(w,s)\|^d\le\|(P(w,s),Q(w,s))\|\le B\|(w,s)\|^d.
$$

Apply this to the entire nonvanishing lift $(e^z,1)$. The logarithmic joint norm differs from $d\log\|(e^z,1)\|$ by a bounded function. Its circular mean minus the value at zero is the spherical characteristic. It differs from the ordinary characteristic by $O(1)$: [Jensen's formula](../../../../../jensen-s-formula.md) applied to the entire denominator counts its zeros, while

$$
0\le\tfrac12\log(1+x^2)-\log^+x\le\tfrac12\log2
$$

controls the proximity replacement. If the denominator vanishes at zero, factor its zero and use its leading coefficient in [Jensen's formula](../../../../../jensen-s-formula.md); the discrepancy is still a basepoint-dependent constant. This proves the [rational composition law for the Nevanlinna characteristic](../../../../../rational-composition-law-for-the-nevanlinna-characteristic.md) here and gives

$$
\boxed{T_{U\circ e}(R)=\frac d\pi R+O(1)\sim\frac d\pi R.}
$$

If $U$ is constant, $d=0$ and its characteristic is bounded instead.

For a simultaneous nonzero deficiency and ramification example choose

$$
f(z)=e^z(e^z-1)^2,
$$

a degree-three [polynomial](../../../../../polynomial-split.md) composed with the exponential. Its characteristic is $3R/\pi+O(1)$. Its only zeros are $2\pi i n$, $n\in\mathbb Z$, all of [multiplicity](../../../../../multiplicity-mathematics.md) two. The number of distinct such points in a large disc is $R/\pi+O(1)$, so integration of their count gives

$$
\overline N(R;0)=R/\pi+O(\log R),\qquad N(R;0)=2R/\pi+O(\log R).
$$

The origin contribution is handled by its usual logarithmic counting term. Therefore

$$
\boxed{\delta_f(0)=\tfrac13,\qquad\theta_f(0)=\tfrac13.}
$$

This is [simultaneous deficiency and ramification for an exponential polynomial](../../../../../simultaneous-deficiency-and-ramification-for-an-exponential-polynomial.md): the missing exponential value contributes a deficit, while the attained value is attained with double [multiplicity](../../../../../multiplicity-mathematics.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
