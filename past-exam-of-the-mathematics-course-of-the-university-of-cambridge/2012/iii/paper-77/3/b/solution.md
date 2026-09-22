<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the intended nontrivial interface, take the limiting amplitude at the patterned end to be $R_->0$; the identically zero solution is otherwise a trivial exception. Splitting the stationary [real-coefficient cubic-quintic amplitude equation](../../../../../../real-coefficient-cubic-quintic-amplitude-equation.md) into real and imaginary parts gives

$$
R''-R(\phi')^2+\mu R+\alpha R^3-R^5=0,\qquad 2R'\phi'+R\phi''=0.
$$

The imaginary equation implies $R^2\phi'=J$, a constant. The radial first integral is

$$
\frac12(R')^2+\frac{J^2}{2R^2}+V(R)=E,\qquad V(R)=\frac\mu2R^2+\frac\alpha4R^4-\frac16R^6.
$$

A regular solution has finite $E$. As $R\to0$, the nonnegative $J^2/(2R^2)$ term would diverge unless $J=0$. Hence **$\phi'=0$ wherever the nontrivial front has positive amplitude**. This conclusion does not assume in advance that the patterned end has no phase gradient.

For a [heteroclinic orbit](../../../../../../heteroclinic-orbit.md) connecting two constant states, $R'$ tends to zero at both ends. Thus $E=V(0)=0$, while the nonzero end must obey both $\mu+\alpha q-q^2=0$ and $V(\sqrt q)=0$. Eliminating $\mu$ gives

$$
0=\frac{q^3}{3}-\frac{\alpha q^2}{4},\qquad \boxed{q=\frac{3\alpha}{4},\quad\mu_M=-\frac{3\alpha^2}{16}<0.}
$$

This is the [stationary front of a cubic-quintic amplitude equation](../../../../../../stationary-front-of-a-cubic-quintic-amplitude-equation.md): a unique equal-potential parameter in the bistable interval.

Existence, not just a necessary condition, follows from the first integral. At $\mu_M$, $V(R)=-R^2(R^2-q)^2/6$. The descending solution obeys $R'=-R(q-R^2)/\sqrt3$, which integrates to

$$
\boxed{A(x)=e^{i\phi_0}\sqrt{\frac{3\alpha/4}{1+\exp[\sqrt3\alpha(x-x_0)/2]}}.}
$$

It connects the stable upper pattern at $x\to-\infty$ to conduction at $x\to+\infty$, with arbitrary translation $x_0$ and constant phase $\phi_0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Section II](../../section-ii.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
