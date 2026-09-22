<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

Write a member of the [special linear group](../../../../../special-linear-group.md) as $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ with $ad-bc=1$. Its [Möbius transformation](../../../../../mobius-transformation.md) is $z\mapsto(az+b)/(cz+d)$, with the usual values at a pole and at infinity. For nonreal $z$,

$$
\operatorname{Im}(gz)=\frac{\operatorname{Im}z}{|cz+d|^2}.
$$

This follows by multiplying numerator and denominator by $c\bar z+d$. Thus the sign of the imaginary part is preserved, while the extended real line is preserved as a set.

Fixing zero requires $b=0$. Therefore its [stabilizer subgroup](../../../../../stabilizer-subgroup.md) and [group orbit](../../../../../orbit-of-a-group-action.md) are

$$
\boxed{G_0=\left\{\begin{pmatrix}a&0\\c&a^{-1}\end{pmatrix}:a\ne0,\ c\in\mathbb R\right\},\qquad
G0=\mathbb R\cup\{\infty\}.}
$$

Translations send zero to each finite real point, and $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ sends it to infinity.

For $gi=i$, comparing real and imaginary parts gives $a=d$ and $b=-c$, with $a^2+c^2=1$. Exactly the same conditions follow from $g(-i)=-i$. Hence

$$
\boxed{G_i=G_{-i}=SO(2)=\left\{\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}:\theta\in\mathbb R\right\}.}
$$

For any $x\in\mathbb R$ and $y>0$, the upper triangular matrix

$$
h_{x,y}=\begin{pmatrix}\sqrt y&x/\sqrt y\\0&1/\sqrt y\end{pmatrix}
$$

sends $i$ to $x+iy$ and $-i$ to $x-iy$. Therefore the two [group orbits](../../../../../orbit-of-a-group-action.md) are the open [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) and the open lower half-plane respectively. Along with the extended real line they exhaust the [Riemann sphere](../../../../../riemann-sphere.md), so **there are exactly three orbits**, the [real determinant-one Möbius orbits](../../../../../real-determinant-one-mobius-orbits.md).

Every $h\in H$ has the form $\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}$ and acts by $z\mapsto a^2z+ab$. Thus $Hi$ is the entire [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), by the same explicit matrices $h_{x,y}$. Given $g\in G$, choose $h\in H$ such that $hi=gi$. Then $k=h^{-1}g$ fixes $i$, so $k\in SO(2)$ and $g=hk$. This proves the [triangular-rotation factorization of real determinant-one matrices](../../../../../triangular-rotation-factorization-of-real-determinant-one-matrices.md).

For uniqueness, if $h_1k_1=h_2k_2$, then $h_2^{-1}h_1=k_2k_1^{-1}\in H\cap SO(2)$. An upper triangular [rotation matrix](../../../../../rotation-matrix.md) must have $\sin\theta=0$, so

$$
H\cap SO(2)=\{I,-I\}.
$$

There are consequently **exactly two matrix factorizations**, $(h,k)$ and $(-h,-k)$. Restricting the first diagonal entry of $h$ to be positive makes the factorization unique. For example, if $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ and $q=\sqrt{c^2+d^2}$, that unique branch is

$$
h=\begin{pmatrix}1/q&(ac+bd)/q\\0&q\end{pmatrix},\qquad
k=\frac1q\begin{pmatrix}d&-c\\c&d\end{pmatrix}.
$$

Angles are understood modulo $2\pi$ when counting matrices; allowing unrestricted real angle representatives gives infinitely many labels for those same two factorizations.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
