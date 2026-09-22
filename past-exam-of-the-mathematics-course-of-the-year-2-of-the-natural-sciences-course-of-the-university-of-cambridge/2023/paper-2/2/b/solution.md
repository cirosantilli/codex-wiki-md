<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat each angular [Fourier mode](../../../../../fourier-mode.md) independently. Boundedness at the axis excludes the negative radial powers and the logarithm inside; decay at infinity excludes the positive powers, constant and logarithm outside. For the cosine mode write

$$
\Phi_{n,\rm in}=A_nr^n\cos n\theta,\qquad
\Phi_{n,\rm out}=B_nr^{-n}\cos n\theta.
$$

Continuity at $R$ gives $B_n=A_nR^{2n}$. The jump of the [normal derivative](../../../../../normal-derivative.md) is then

$$
-nB_nR^{-n-1}-nA_nR^{n-1}=-2nA_nR^{n-1}=-a_n.
$$

Thus $A_n=a_nR^{1-n}/(2n)$ and $B_n=a_nR^{n+1}/(2n)$. The sine mode has the same relation with $b_n$. Therefore the [potential of a charged cylindrical shell with angular Fourier data](../../../../../potential-of-a-charged-cylindrical-shell-with-angular-fourier-data.md) is

$$
\boxed{\Phi(r,\theta)=\sum_{n=1}^{\infty}\frac R{2n}(a_n\cos n\theta+b_n\sin n\theta)
\begin{cases}(r/R)^n,&0\leq r\leq R,\\(R/r)^n,&r\geq R.\end{cases}}
$$

There is no angular mean term: the given [surface charge density](../../../../../surface-charge-density.md) has zero average. The interior constant is zero because its boundary value must match the vanishing exterior mean. A nonzero mean charge per unit length would instead produce a logarithmic [electrostatic potential](../../../../../electric-potential.md), incompatible with the specified decay at infinity.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
