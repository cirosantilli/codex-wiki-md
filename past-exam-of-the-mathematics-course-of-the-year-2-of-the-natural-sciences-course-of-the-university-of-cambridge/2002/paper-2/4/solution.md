<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Definitions.** In a punctured neighborhood of $z_0$, let the [Laurent series](../../../../laurent-series.md) be $f(z)=\sum_{j=-\infty}^{\infty}c_j(z-z_0)^j$. The point is a [pole](../../../../pole.md) of order $m\geq1$ if $c_{-m}\ne0$ and every coefficient with index less than $-m$ vanishes. Its [residue](../../../../residue.md) is $\boxed{\operatorname{Res}_{z_0}f=c_{-1}}$. A [simple pole](../../../../simple-pole.md) has $m=1$.

**Poles for $0<a<1$.** Denote the bracket in the denominator by $D(z)$. Factoring gives

$$
D(z)=[(a-1)z^2+(a+1)][(a+1)z^2+(a-1)].
$$

Put $q=\sqrt{(1-a)/(1+a)}$, so $0<q<1$. The finite [poles](../../../../pole.md) are $0,\pm q,\pm q^{-1}$, all simple; the numerator is nonzero at each. At zero,

$$
\operatorname{Res}_0f=\frac1{a^2-1}=-\frac1{1-a^2}.
$$

At a nonzero simple root $r$ of $D$, the [residue](../../../../residue.md) formula gives

$$
\operatorname{Res}_rf=\frac{(r^2+1)^2}{rD'(r)},\qquad D'(r)=4r[a^2(r^2+1)-(r^2-1)].
$$

For $r^2=q^2$, $D'(r)=8ar$; for $r^2=q^{-2}$, $D'(r)=-8ar$. Substitution yields

$$
\boxed{\begin{array}{c|c|c}\text{point}&\text{pole order}&\text{residue}\\\hline
0&1&-1/(1-a^2)\\
+q,-q&1&1/[2a(1-a^2)]\\
+q^{-1},-q^{-1}&1&-1/[2a(1-a^2)]
\end{array}\quad(0<a<1).}
$$

The two [zeros of a function](../../../../zero-of-a-function.md) at $z=\pm i$ do not cause additional [poles](../../../../pole.md): there $D=-4$ and the numerator vanishes.

**The case $a=1$.** Simplify before using any formulas that divide by $1-a^2$:

$$
D(z)=(z^2+1)^2-(z^2-1)^2=4z^2,\qquad f(z)=\frac14\left(z+\frac2z+\frac1{z^3}\right).
$$

Thus its only finite [pole](../../../../pole.md) is

$$
\boxed{z=0:\quad\text{order }3,\qquad\operatorname{Res}_0f=\tfrac12\quad(a=1).}
$$

As $a\uparrow1$, the two inner [poles](../../../../pole.md) merge with zero while the outer two escape to infinity. If one also considers the [Riemann sphere](../../../../riemann-sphere.md), $f$ at $a=1$ has a simple [pole](../../../../pole.md) at infinity because $f(z)\sim z/4$; the requested unit-circle calculation only uses finite [poles](../../../../pole.md).

**Unit-circle integral.** Set $z=e^{i\theta}$. Then

$$
\tan\theta=\frac{z^2-1}{i(z^2+1)},\qquad d\theta=\frac{dz}{iz},\qquad\frac{d\theta}{a^2+\tan^2\theta}=\frac1i f(z)\,dz.
$$

At the two angles where the tangent is undefined, the real integrand has continuous limiting value zero. Thus the substitution is valid for the [improper integral](../../../../improper-integral.md), or after that continuous extension. No [pole](../../../../pole.md) lies on $|z|=1$ for any allowed $a$.

For $0<a<1$, the sum of the enclosed [residues](../../../../residue.md) is

$$
-\frac1{1-a^2}+\frac1{a(1-a^2)}=\frac1{a(1+a)}.
$$

The [residue theorem](../../../../residue-theorem.md) therefore gives

$$
\boxed{I=\frac1i\oint_{|z|=1}f(z)\,dz=\frac{2\pi}{a(1+a)},\qquad0<a\leq1.}
$$

At $a=1$ the enclosed [residue](../../../../residue.md) is $1/2$, giving $I=\pi$, exactly the same formula. The direct simplification $1/(1+\tan^2\theta)=\cos^2\theta$ provides an independent check of that endpoint.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
